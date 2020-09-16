---
title: папката 1336 RecoverableItems е пълна
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1336"
- "3700003"
ms.assetid: a3a923e8-fece-4a26-b8b6-00970d75275e
ms.openlocfilehash: 6ae608b776332402fe333315f5e4ff6072b0a651
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: bg-BG
ms.lasthandoff: 09/14/2020
ms.locfileid: "47741256"
---
# <a name="the-recoverable-items-folder-is-full"></a><span data-ttu-id="11e6b-102">Папката "Възстановими елементи" е пълна</span><span class="sxs-lookup"><span data-stu-id="11e6b-102">The Recoverable Items folder is full</span></span>

<span data-ttu-id="11e6b-103">За пощенски кутии на Exchange Online, ограничението за място за съхранение по подразбиране за папката "Възстановими елементи" е 30 ГБ.</span><span class="sxs-lookup"><span data-stu-id="11e6b-103">For Exchange Online mailboxes, the default storage limit for the Recoverable Items folder is 30 GB.</span></span> <span data-ttu-id="11e6b-104">Ограничението за място за съхранение за папката "Възстановими елементи" се увеличава автоматично на 100 ГБ, ако пощенската кутия е поставена в задържане за съдебен процес, в откриване на откриването на електронни данни или е присвоено на правила за съхранение.</span><span class="sxs-lookup"><span data-stu-id="11e6b-104">The storage limit for the Recoverable Items folder is automatically increased to 100 GB if the mailbox is placed on Litigation Hold, eDiscovery hold, or is assigned to a retention policy.</span></span>

<span data-ttu-id="11e6b-105">Когато папката "Възстановими елементи" достигне ограничението за място за съхранение, функцията за пощенска кутия се влияе по следния начин:</span><span class="sxs-lookup"><span data-stu-id="11e6b-105">When the Recoverable Items folder reaches the storage limit, mailbox functionality is affected in the following ways:</span></span>

- <span data-ttu-id="11e6b-106">Потребителят не може да изтрие елементи от пощенската кутия.</span><span class="sxs-lookup"><span data-stu-id="11e6b-106">The user can't delete items from the mailbox.</span></span>

- <span data-ttu-id="11e6b-107">Помощникът за управление на папки не може да изтрие елементи на базата на етикет за съхранение или настройки на управляваната папка.</span><span class="sxs-lookup"><span data-stu-id="11e6b-107">The Managed Folder Assistant can't delete items based on retention tag or managed folder settings.</span></span>

- <span data-ttu-id="11e6b-108">За пощенските кутии, които имат разрешено възстановяване на единичен елемент или са поставени в очакване, процесът на защита при копиране на страница за извличане не може да поддържа версии на елементи, редактирани от потребителя.</span><span class="sxs-lookup"><span data-stu-id="11e6b-108">For mailboxes that have Single Item Recovery enabled or are placed on hold, the copy-on-write page protection process can't maintain versions of items edited by the user.</span></span>

- <span data-ttu-id="11e6b-109">За пощенски кутии, на които е разрешено регистрирането на пощенските кутии, не могат да се запишат записи от регистрационния файл за проверка на пощенска кутия в подпапката "проверки"</span><span class="sxs-lookup"><span data-stu-id="11e6b-109">For mailboxes that have mailbox audit logging enabled, no mailbox audit log entries can be saved in the Audits subfolder in the Recoverable Items folder.</span></span>

<span data-ttu-id="11e6b-110">За пощенските кутии, които не са задържани, администраторите могат да използват `Search-Mailbox -SearchDumpsterOnly -DeleteContent` командата в Exchange Online PowerShell за изтриване на елементи в папката "Възстановими елементи".</span><span class="sxs-lookup"><span data-stu-id="11e6b-110">For mailboxes that aren't on hold, admins can use the `Search-Mailbox -SearchDumpsterOnly -DeleteContent` command in Exchange Online PowerShell to delete items in the Recoverable Items folder.</span></span> <span data-ttu-id="11e6b-111">За още информация вижте следните теми:</span><span class="sxs-lookup"><span data-stu-id="11e6b-111">For more information, see the following topics:</span></span>

- [<span data-ttu-id="11e6b-112">Търсене и изтриване на съобщения</span><span class="sxs-lookup"><span data-stu-id="11e6b-112">Search for and delete messages</span></span>](https://docs.microsoft.com/microsoft-365/compliance/search-for-and-delete-messagesadmin-help)

- [<span data-ttu-id="11e6b-113">Търсене – пощенска кутия</span><span class="sxs-lookup"><span data-stu-id="11e6b-113">Search-Mailbox</span></span>](https://docs.microsoft.com/powershell/module/exchange/mailboxes/Search-Mailbox)

<span data-ttu-id="11e6b-114">За пощенските кутии, които са задържани, администраторите трябва да премахнат задържането, преди да могат да изтриват елементи от папката "Възстановими елементи".</span><span class="sxs-lookup"><span data-stu-id="11e6b-114">For mailboxes that are on hold, admins have to remove the hold before they can deleted items from the Recoverable Items folder.</span></span> <span data-ttu-id="11e6b-115">За повече информация вижте [Изтриване на елементи от папката "Възстановими елементи" на базирани на облака пощенски кутии в очакване](https://docs.microsoft.com/microsoft-365/compliance/delete-items-in-the-recoverable-items-folder-of-mailboxes-on-hold).</span><span class="sxs-lookup"><span data-stu-id="11e6b-115">For more information, see [Delete items in the Recoverable Items folder of cloud-based mailboxes on hold](https://docs.microsoft.com/microsoft-365/compliance/delete-items-in-the-recoverable-items-folder-of-mailboxes-on-hold).</span></span>

<span data-ttu-id="11e6b-116">За да попречите на папката "Възстановими елементи" да се запълни, администраторите могат да увеличат ограничението за място за съхранение на папката "Възстановими елементи" за пощенските кутии, които са в очакване и да настроят правила за съхранение на пощенски кутии, които преместват елементи от папката "Възстановими елементи" в пощенската кутия на потребителя.</span><span class="sxs-lookup"><span data-stu-id="11e6b-116">To help prevent the Recoverable Items folder from becoming full, admins can increase the storage limit of the Recoverable Items folder for mailboxes on hold and set up a mailbox retention policy that moves items from the Recoverable Items folder to the user's archive mailbox.</span></span> <span data-ttu-id="11e6b-117">Вижте [увеличаване на квотата за Възстановими елементи за пощенските кутии](https://docs.microsoft.com/microsoft-365/compliance/increase-the-recoverable-quota-for-mailboxes-on-hold), които са в режим на задържане.</span><span class="sxs-lookup"><span data-stu-id="11e6b-117">See [Increase the Recoverable Items quota for mailboxes on hold](https://docs.microsoft.com/microsoft-365/compliance/increase-the-recoverable-quota-for-mailboxes-on-hold).</span></span>
