---
title: 1336 RecoverAbleItems папка е пълна
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
ms.openlocfilehash: 4f0cba480fcc05114abd8f370b84e9a37e5f2804
ms.sourcegitcommit: bc7d6f4f3c9f7060d073f5130e1ec856e248d020
ms.translationtype: MT
ms.contentlocale: bg-BG
ms.lasthandoff: 06/02/2020
ms.locfileid: "44510741"
---
# <a name="the-recoverable-items-folder-is-full"></a><span data-ttu-id="885f4-102">Папката "Елементи за възстановяване" е пълна</span><span class="sxs-lookup"><span data-stu-id="885f4-102">The Recoverable Items folder is full</span></span>

<span data-ttu-id="885f4-103">За пощенски кутии на Exchange Online ограничението по подразбиране за папката за възстановяване на елементи е 30 GB.</span><span class="sxs-lookup"><span data-stu-id="885f4-103">For Exchange Online mailboxes, the default storage limit for the Recoverable Items folder is 30 GB.</span></span> <span data-ttu-id="885f4-104">Ограничението за съхранение за папката за елементи на възстановяване автоматично се увеличава до 100 GB, ако пощенската кутия е поставен на задържане, eDiscovery задържане или е присвоена на правила за задържане.</span><span class="sxs-lookup"><span data-stu-id="885f4-104">The storage limit for the Recoverable Items folder is automatically increased to 100 GB if the mailbox is placed on Litigation Hold, eDiscovery hold, or is assigned to a retention policy.</span></span>

<span data-ttu-id="885f4-105">Когато папката за възстановяване на елементи достигне ограничението за съхранение, функции на пощенска кутия е засегната по следните начини:</span><span class="sxs-lookup"><span data-stu-id="885f4-105">When the Recoverable Items folder reaches the storage limit, mailbox functionality is affected in the following ways:</span></span>

- <span data-ttu-id="885f4-106">Потребителят не може да изтрие елементи от пощенската кутия.</span><span class="sxs-lookup"><span data-stu-id="885f4-106">The user can't delete items from the mailbox.</span></span>

- <span data-ttu-id="885f4-107">Помощникът за управлявани папки не може да изтрие елементи въз основа на етикет за задържане или настройки на управляваните папки.</span><span class="sxs-lookup"><span data-stu-id="885f4-107">The Managed Folder Assistant can't delete items based on retention tag or managed folder settings.</span></span>

- <span data-ttu-id="885f4-108">За пощенски кутии, които имат един елемент възстановяване разрешено или са поставени на задържане, процесът на защита на страница копие при запис не може да поддържа версии на елементи, редактирани от потребителя.</span><span class="sxs-lookup"><span data-stu-id="885f4-108">For mailboxes that have Single Item Recovery enabled or are placed on hold, the copy-on-write page protection process can't maintain versions of items edited by the user.</span></span>

- <span data-ttu-id="885f4-109">За пощенски кутии, които имат пощенска кутия проверка регистриране разрешено пощенска кутия проверка регистрационни записи могат да бъдат записани в подпапка проверки в папката елементи за възстановяване.</span><span class="sxs-lookup"><span data-stu-id="885f4-109">For mailboxes that have mailbox audit logging enabled, no mailbox audit log entries can be saved in the Audits subfolder in the Recoverable Items folder.</span></span>

<span data-ttu-id="885f4-110">За пощенски кутии, които не са на задържане, администраторите могат да използват `Search-Mailbox -SearchDumpsterOnly -DeleteContent` командата в Exchange Online PowerShell за изтриване на елементи в папката за елементи за възстановяване.</span><span class="sxs-lookup"><span data-stu-id="885f4-110">For mailboxes that aren't on hold, admins can use the `Search-Mailbox -SearchDumpsterOnly -DeleteContent` command in Exchange Online PowerShell to delete items in the Recoverable Items folder.</span></span> <span data-ttu-id="885f4-111">За още информация вижте следните теми:</span><span class="sxs-lookup"><span data-stu-id="885f4-111">For more information, see the following topics:</span></span>

- [<span data-ttu-id="885f4-112">Търсене и изтриване на съобщения</span><span class="sxs-lookup"><span data-stu-id="885f4-112">Search for and delete messages</span></span>](https://docs.microsoft.com/microsoft-365/compliance/search-for-and-delete-messagesadmin-help)

- [<span data-ttu-id="885f4-113">Пощенска кутия за търсене</span><span class="sxs-lookup"><span data-stu-id="885f4-113">Search-Mailbox</span></span>](https://docs.microsoft.com/powershell/module/exchange/mailboxes/Search-Mailbox)

<span data-ttu-id="885f4-114">За пощенски кутии, които са на задържане администраторите трябва да премахнете задържане преди те да могат да изтрити елементи от папката за възстановяване на елементи.</span><span class="sxs-lookup"><span data-stu-id="885f4-114">For mailboxes that are on hold, admins have to remove the hold before they can deleted items from the Recoverable Items folder.</span></span> <span data-ttu-id="885f4-115">За повече информация вижте [Изтриване на елементи в папката на папките за възстановяване на облак базирани пощенски кутии на задържане](https://docs.microsoft.com/microsoft-365/compliance/delete-items-in-the-recoverable-items-folder-of-mailboxes-on-hold).</span><span class="sxs-lookup"><span data-stu-id="885f4-115">For more information, see [Delete items in the Recoverable Items folder of cloud-based mailboxes on hold](https://docs.microsoft.com/microsoft-365/compliance/delete-items-in-the-recoverable-items-folder-of-mailboxes-on-hold).</span></span>

<span data-ttu-id="885f4-116">За да предотвратите папката за възстановяване елементи стават пълни, администраторите могат да увеличат ограничението за съхранение на папката за пощенски кутии на задържане и задаване на пощенска кутия за съхранение, която премества елементи от папката за възстановяване на елементи на потребителя архивна пощенска кутия.</span><span class="sxs-lookup"><span data-stu-id="885f4-116">To help prevent the Recoverable Items folder from becoming full, admins can increase the storage limit of the Recoverable Items folder for mailboxes on hold and set up a mailbox retention policy that moves items from the Recoverable Items folder to the user's archive mailbox.</span></span> <span data-ttu-id="885f4-117">Вижте [Увеличаване на квотата за възстановяване на елементи за пощенски кутии на задържане](https://docs.microsoft.com/microsoft-365/compliance/increase-the-recoverable-quota-for-mailboxes-on-hold).</span><span class="sxs-lookup"><span data-stu-id="885f4-117">See [Increase the Recoverable Items quota for mailboxes on hold](https://docs.microsoft.com/microsoft-365/compliance/increase-the-recoverable-quota-for-mailboxes-on-hold).</span></span>
