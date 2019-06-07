---
title: 1336 RecoverableItems папка е пълна
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 11/5/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom: 1336
ms.assetid: a3a923e8-fece-4a26-b8b6-00970d75275e
ms.openlocfilehash: cfcc69c1b3a59c73037d9a493af4ece86b7b7208
ms.sourcegitcommit: 4b7e478ce700c0b781efec3857ac4dce5bdf00c6
ms.translationtype: MT
ms.contentlocale: bg-BG
ms.lasthandoff: 06/07/2019
ms.locfileid: "34762069"
---
# <a name="the-recoverable-items-folder-is-full"></a><span data-ttu-id="158ba-102">Папката е пълна</span><span class="sxs-lookup"><span data-stu-id="158ba-102">The Recoverable Items folder is full</span></span>

<span data-ttu-id="158ba-103">За Exchange Online кутии в Office 365 ограничението за съхранение по подразбиране за папката "Възстановими елементи" е 30 GB.</span><span class="sxs-lookup"><span data-stu-id="158ba-103">For Exchange Online mailboxes in Office 365, the default storage limit for the Recoverable Items folder is 30 GB.</span></span> <span data-ttu-id="158ba-104">За съхранение граница за папката "Възстановими елементи" автоматично се увеличава до 100 GB, ако пощенската кутия се поставя върху процесуално държат, eDiscovery държат, или е присвоен на политика за задържане на Office 365.</span><span class="sxs-lookup"><span data-stu-id="158ba-104">The storage limit for the Recoverable Items folder is automatically increased to 100 GB if the mailbox is placed on Litigation Hold, eDiscovery hold, or is assigned to an Office 365 retention policy.</span></span>

<span data-ttu-id="158ba-105">Когато запълненият достигне лимита за съхранение, пощенска кутия функционалност е засегната по следните начини:</span><span class="sxs-lookup"><span data-stu-id="158ba-105">When the Recoverable Items folder reaches the storage limit, mailbox functionality is affected in the following ways:</span></span>

- <span data-ttu-id="158ba-106">Потребителят не може да изтрива елементи от пощенската кутия.</span><span class="sxs-lookup"><span data-stu-id="158ba-106">The user can't delete items from the mailbox.</span></span>

- <span data-ttu-id="158ba-107">Помощникът за управлявани папки не може да изтриете елементи, въз основа на етикет за съхранение или настройки за управлявани папки.</span><span class="sxs-lookup"><span data-stu-id="158ba-107">The Managed Folder Assistant can't delete items based on retention tag or managed folder settings.</span></span>

- <span data-ttu-id="158ba-108">За пощенски кутии, които са разрешени за възстановяване на един елемент или са поставени на задържане копие на пиша страница защита процес не може да поддържа версии на елементи, които се редактират от потребителя.</span><span class="sxs-lookup"><span data-stu-id="158ba-108">For mailboxes that have Single Item Recovery enabled or are placed on hold, the copy-on-write page protection process can't maintain versions of items edited by the user.</span></span>

- <span data-ttu-id="158ba-109">За пощенски кутии, които имат пощенска кутия одит разрешено регистриране не пощенска кутия одит записи могат да бъдат записани в одитите подпапка в папката "Възстановими елементи".</span><span class="sxs-lookup"><span data-stu-id="158ba-109">For mailboxes that have mailbox audit logging enabled, no mailbox audit log entries can be saved in the Audits subfolder in the Recoverable Items folder.</span></span>

<span data-ttu-id="158ba-110">За пощенски кутии, които не са задържани, администраторите могат да използват `Search-Mailbox -SearchDumpsterOnly -DeleteContent` команда в Exchange Online PowerShell да изтриете елементи в папката "Възстановими елементи".</span><span class="sxs-lookup"><span data-stu-id="158ba-110">For mailboxes that aren't on hold, admins can use the `Search-Mailbox -SearchDumpsterOnly -DeleteContent` command in Exchange Online PowerShell to delete items in the Recoverable Items folder.</span></span> <span data-ttu-id="158ba-111">За още информация вижте следните теми:</span><span class="sxs-lookup"><span data-stu-id="158ba-111">For more information, see the following topics:</span></span> 

- [<span data-ttu-id="158ba-112">Търсене и изтриване на съобщения</span><span class="sxs-lookup"><span data-stu-id="158ba-112">Search for and delete messages</span></span>](https://docs.microsoft.com/office365/securitycompliance/search-for-and-delete-messagesadmin-help)

- [<span data-ttu-id="158ba-113">Търсене-пощенска кутия</span><span class="sxs-lookup"><span data-stu-id="158ba-113">Search-Mailbox</span></span>](https://docs.microsoft.com/powershell/module/exchange/mailboxes/Search-Mailbox)

<span data-ttu-id="158ba-114">За пощенски кутии, които са задържани администраторите трябва да премахнете трюма, преди те да могат изтритите елементи от папката "Възстановими елементи".</span><span class="sxs-lookup"><span data-stu-id="158ba-114">For mailboxes that are on hold, admins have to remove the hold before they can deleted items from the Recoverable Items folder.</span></span> <span data-ttu-id="158ba-115">За повече информация вижте [Изтриване на елементи в Възстановими елементи папка на облака на задръжте](https://docs.microsoft.com/office365/securitycompliance/delete-items-in-the-recoverable-items-folder-of-mailboxes-on-hold).</span><span class="sxs-lookup"><span data-stu-id="158ba-115">For more information, see [Delete items in the Recoverable Items folder of cloud-based mailboxes on hold](https://docs.microsoft.com/office365/securitycompliance/delete-items-in-the-recoverable-items-folder-of-mailboxes-on-hold).</span></span>

<span data-ttu-id="158ba-116">За да предотвратите запълненият от стават пълна, администраторите могат да увеличат ограничението за съхранение на Възстановими елементи папка за пощенски кутии на задръжте и създаване на пощенска кутия правило, което премества елементи от папката "Възстановими елементи" на потребителя Архив пощенска кутия.</span><span class="sxs-lookup"><span data-stu-id="158ba-116">To help prevent the Recoverable Items folder from becoming full, admins can increase the storage limit of the Recoverable Items folder for mailboxes on hold and set up a mailbox retention policy that moves items from the Recoverable Items folder to the user's archive mailbox.</span></span> <span data-ttu-id="158ba-117">Вижте [увеличи запълненият квота за пощенски кутии на задръжте](https://docs.microsoft.com/office365/securitycompliance/increase-the-recoverable-quota-for-mailboxes-on-hold).</span><span class="sxs-lookup"><span data-stu-id="158ba-117">See [Increase the Recoverable Items quota for mailboxes on hold](https://docs.microsoft.com/office365/securitycompliance/increase-the-recoverable-quota-for-mailboxes-on-hold).</span></span>
