---
title: 1336 Папката "Възстановими елементи" е пълна
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1336"
- "3700003"
ms.assetid: a3a923e8-fece-4a26-b8b6-00970d75275e
ms.openlocfilehash: fb10b792981040bdcf4661b8aff30733c2438212
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: bg-BG
ms.lasthandoff: 04/22/2020
ms.locfileid: "43720241"
---
# <a name="the-recoverable-items-folder-is-full"></a><span data-ttu-id="82070-102">Папката "Възстановими елементи" е пълна</span><span class="sxs-lookup"><span data-stu-id="82070-102">The Recoverable Items folder is full</span></span>

<span data-ttu-id="82070-103">За пощенски кутии на Exchange Online ограничението за съхранение по подразбиране за папката за възстановяване на елементи е 30 ГБ.</span><span class="sxs-lookup"><span data-stu-id="82070-103">For Exchange Online mailboxes, the default storage limit for the Recoverable Items folder is 30 GB.</span></span> <span data-ttu-id="82070-104">Ограничението за съхранение на папката за възстановяване на елементи автоматично се увеличава до 100 ГБ, ако пощенската кутия е поставен на задържане, задържане на електронни данни или е присвоен на правила за задържане.</span><span class="sxs-lookup"><span data-stu-id="82070-104">The storage limit for the Recoverable Items folder is automatically increased to 100 GB if the mailbox is placed on Litigation Hold, eDiscovery hold, or is assigned to a retention policy.</span></span>

<span data-ttu-id="82070-105">Когато папката за възстановяване на елементи достигне ограничението за съхранение, функционалността на пощенската кутия е засегната по следните начини:</span><span class="sxs-lookup"><span data-stu-id="82070-105">When the Recoverable Items folder reaches the storage limit, mailbox functionality is affected in the following ways:</span></span>

- <span data-ttu-id="82070-106">Потребителят не може да изтриете елементи от пощенската кутия.</span><span class="sxs-lookup"><span data-stu-id="82070-106">The user can't delete items from the mailbox.</span></span>

- <span data-ttu-id="82070-107">Помощникът за управлявани папки не може да изтрива елементи въз основа на етикет аг лаг или настройки на управлявана папка.</span><span class="sxs-lookup"><span data-stu-id="82070-107">The Managed Folder Assistant can't delete items based on retention tag or managed folder settings.</span></span>

- <span data-ttu-id="82070-108">За пощенски кутии, които имат един елемент възстановяване разрешено или са поставени на задържане, процесът на защита на страницата за копиране не може да поддържа версии на елементи, редактирани от потребителя.</span><span class="sxs-lookup"><span data-stu-id="82070-108">For mailboxes that have Single Item Recovery enabled or are placed on hold, the copy-on-write page protection process can't maintain versions of items edited by the user.</span></span>

- <span data-ttu-id="82070-109">За пощенски кутии, които имат пощенска кутия проверка регистриране разрешено не пощенска кутия проверка регистрационните записи могат да бъдат записани в подпапка проверки в папката за възстановяване на елементи.</span><span class="sxs-lookup"><span data-stu-id="82070-109">For mailboxes that have mailbox audit logging enabled, no mailbox audit log entries can be saved in the Audits subfolder in the Recoverable Items folder.</span></span>

<span data-ttu-id="82070-110">За пощенски кутии, които не са задържат `Search-Mailbox -SearchDumpsterOnly -DeleteContent` администраторите могат да използват командата в Exchange Online PowerShell да изтриете елементи в папката за възстановяване на елементи.</span><span class="sxs-lookup"><span data-stu-id="82070-110">For mailboxes that aren't on hold, admins can use the `Search-Mailbox -SearchDumpsterOnly -DeleteContent` command in Exchange Online PowerShell to delete items in the Recoverable Items folder.</span></span> <span data-ttu-id="82070-111">За още информация вижте следните теми:</span><span class="sxs-lookup"><span data-stu-id="82070-111">For more information, see the following topics:</span></span>

- [<span data-ttu-id="82070-112">Търсене и изтриване на съобщения</span><span class="sxs-lookup"><span data-stu-id="82070-112">Search for and delete messages</span></span>](https://docs.microsoft.com/office365/securitycompliance/search-for-and-delete-messagesadmin-help)

- [<span data-ttu-id="82070-113">Пощенска кутия за търсене</span><span class="sxs-lookup"><span data-stu-id="82070-113">Search-Mailbox</span></span>](https://docs.microsoft.com/powershell/module/exchange/mailboxes/Search-Mailbox)

<span data-ttu-id="82070-114">За пощенски кутии, които са задържат администраторите трябва да премахнете задържане, преди те да изтриете елементи от папката за възстановяване на елементи.</span><span class="sxs-lookup"><span data-stu-id="82070-114">For mailboxes that are on hold, admins have to remove the hold before they can deleted items from the Recoverable Items folder.</span></span> <span data-ttu-id="82070-115">За повече информация вижте Изтриване на елементи в папката За възстановяване на елементи на облак базирани [пощенски кутии на изчакване](https://docs.microsoft.com/office365/securitycompliance/delete-items-in-the-recoverable-items-folder-of-mailboxes-on-hold).</span><span class="sxs-lookup"><span data-stu-id="82070-115">For more information, see [Delete items in the Recoverable Items folder of cloud-based mailboxes on hold](https://docs.microsoft.com/office365/securitycompliance/delete-items-in-the-recoverable-items-folder-of-mailboxes-on-hold).</span></span>

<span data-ttu-id="82070-116">За да предотвратите възстановяване на елементи папка става пълен, администраторите може да увеличи температза съхранение на папката за задържи пощенски кутии и настройка на правило за задържане на пощенска кутия, която премества елементи от папката за възстановяване на елементи в архивната пощенска кутия на потребителя.</span><span class="sxs-lookup"><span data-stu-id="82070-116">To help prevent the Recoverable Items folder from becoming full, admins can increase the storage limit of the Recoverable Items folder for mailboxes on hold and set up a mailbox retention policy that moves items from the Recoverable Items folder to the user's archive mailbox.</span></span> <span data-ttu-id="82070-117">Вижте [Увеличаване на квотата за възстановими елементи за пощенски кутии на задържане](https://docs.microsoft.com/office365/securitycompliance/increase-the-recoverable-quota-for-mailboxes-on-hold).</span><span class="sxs-lookup"><span data-stu-id="82070-117">See [Increase the Recoverable Items quota for mailboxes on hold](https://docs.microsoft.com/office365/securitycompliance/increase-the-recoverable-quota-for-mailboxes-on-hold).</span></span>
