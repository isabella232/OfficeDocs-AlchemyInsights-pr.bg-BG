---
title: Оттегляне на стари инструменти за откриване на електронни данни
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9001487"
- "3523"
ms.openlocfilehash: c4632b52dde579b7d5b2e6e15f1583300a0bd136
ms.sourcegitcommit: a7c17217c170ead24571421baaf5a14f1525b1a6
ms.translationtype: MT
ms.contentlocale: bg-BG
ms.lasthandoff: 02/20/2020
ms.locfileid: "42157508"
---
# <a name="retirement-of-legacy-ediscovery-tools"></a><span data-ttu-id="aec9b-102">Оттегляне на стари инструменти за откриване на електронни данни</span><span class="sxs-lookup"><span data-stu-id="aec9b-102">Retirement of Legacy eDiscovery Tools</span></span>

<span data-ttu-id="aec9b-103">В резултат на новата и подобрена функционалност за откриване на електронни данни в Центъра за съответствие на Microsoft 365, следните стари инструменти и команди за откриване на електронни данни ще бъдат оттеглени през следващите месеци:</span><span class="sxs-lookup"><span data-stu-id="aec9b-103">As a result of the new and improved eDiscovery functionality in Microsoft 365 Compliance center, the following legacy eDiscovery tools and commandlets will be retired in the coming months:</span></span>

- <span data-ttu-id="aec9b-104">[Откриване на електронни данни](https://docs.microsoft.com/exchange/security-and-compliance/in-place-ediscovery/in-place-ediscovery) на място и [задържане на място](https://docs.microsoft.com/exchange/security-and-compliance/create-or-remove-in-place-holds) в центъра за администриране на Exchange.</span><span class="sxs-lookup"><span data-stu-id="aec9b-104">[In-Place eDiscovery](https://docs.microsoft.com/exchange/security-and-compliance/in-place-ediscovery/in-place-ediscovery) and [In-Place Holds](https://docs.microsoft.com/exchange/security-and-compliance/create-or-remove-in-place-holds) in the Exchange admin center.</span></span>

- <span data-ttu-id="aec9b-105">Кратки команди на Exchange онлайн PowerShell, които поддържат откриване на електронни данни на място и задържане на място.</span><span class="sxs-lookup"><span data-stu-id="aec9b-105">The Exchange Online PowerShell cmdlets that support In-Place eDiscovery and In-Place Holds.</span></span> <span data-ttu-id="aec9b-106">(Тези кратки команди са общо определени като \*-MailboxSearch кратки команди.) Това включва следните кратки команди:</span><span class="sxs-lookup"><span data-stu-id="aec9b-106">(These cmdlets are collectively identified as \*-MailboxSearch cmdlets.) This includes the following cmdlets:</span></span>

    - [<span data-ttu-id="aec9b-107">Търсене на нова пощенска кутия</span><span class="sxs-lookup"><span data-stu-id="aec9b-107">New-MailboxSearch</span></span>](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance-content-search/new-mailboxsearch)
    - [<span data-ttu-id="aec9b-108">Търсене в стартова пощенска кутия</span><span class="sxs-lookup"><span data-stu-id="aec9b-108">Start-MailboxSearch</span></span>](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance-content-search/start-mailboxsearch)
    - [<span data-ttu-id="aec9b-109">Търсене на пощенски кутии</span><span class="sxs-lookup"><span data-stu-id="aec9b-109">Stop-MailboxSearch</span></span>](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance-content-search/stop-mailboxsearch)
    - [<span data-ttu-id="aec9b-110">Търсене в пощенски кутии</span><span class="sxs-lookup"><span data-stu-id="aec9b-110">Set-MailboxSearch</span></span>](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance-content-search/set-mailboxsearch)

- <span data-ttu-id="aec9b-111">Кратката команда [за търсене пощенска кутия](https://docs.microsoft.com/powershell/module/exchange/mailboxes/search-mailbox?view=exchange-ps) в Exchange онлайн PowerShell.</span><span class="sxs-lookup"><span data-stu-id="aec9b-111">The [Search-Mailbox](https://docs.microsoft.com/powershell/module/exchange/mailboxes/search-mailbox?view=exchange-ps) cmdlet in Exchange Online PowerShell.</span></span>
- <span data-ttu-id="aec9b-112">Следните операции в API на уеб услуги на Exchange:</span><span class="sxs-lookup"><span data-stu-id="aec9b-112">The following operations in the Exchange Web Services API:</span></span>
    - [<span data-ttu-id="aec9b-113">Получаване на пощенски кутии с възможност за търсене</span><span class="sxs-lookup"><span data-stu-id="aec9b-113">GetSearchableMailboxes</span></span>](https://docs.microsoft.com/exchange/client-developer/web-service-reference/getsearchablemailboxes-operation)
    - [<span data-ttu-id="aec9b-114">SetHoldOnMailboxes</span><span class="sxs-lookup"><span data-stu-id="aec9b-114">SetHoldOnMailboxes</span></span>](https://docs.microsoft.com/exchange/client-developer/web-service-reference/setholdonmailboxes-operation)
    - [<span data-ttu-id="aec9b-115">Вземи пощенски кутии</span><span class="sxs-lookup"><span data-stu-id="aec9b-115">GetHoldOnMailboxes</span></span>](https://docs.microsoft.com/exchange/client-developer/web-service-reference/getholdonmailboxes-operation)

- [<span data-ttu-id="aec9b-116">Office 365 разширено откриване на електронни данни v1.0</span><span class="sxs-lookup"><span data-stu-id="aec9b-116">Office 365 Advanced eDiscovery v1.0</span></span>](https://docs.microsoft.com/en-us/microsoft-365/compliance/office-365-advanced-ediscovery)

<span data-ttu-id="aec9b-117">**Време в пенсия:**</span><span class="sxs-lookup"><span data-stu-id="aec9b-117">**Timeline for retirement**:</span></span>
- <span data-ttu-id="aec9b-118">1 април 2020 г.: Няма да можете да създавате нови търсения и задържания, но все още можете да изпълнявате, редактирате и изтривате съществуващи търсения на свой собствен риск.</span><span class="sxs-lookup"><span data-stu-id="aec9b-118">April 1, 2020: You won't be able to create new searches and holds, but you can still run, edit, and delete existing searches at your own risk.</span></span> <span data-ttu-id="aec9b-119">Поддръжката на Microsoft вече няма да поддържа откриване на електронни данни на място & притежава в EAC.</span><span class="sxs-lookup"><span data-stu-id="aec9b-119">Microsoft Support will no longer support In-Place eDiscovery & Holds in the EAC.</span></span>

- <span data-ttu-id="aec9b-120">1 юли 2020 г.: функцията "откриване на електронни данни на място" & притежава функционалност в EAC ще бъде поставена в режим само за четене.</span><span class="sxs-lookup"><span data-stu-id="aec9b-120">July 1, 2020: The In-Place eDiscovery & Holds functionality in the EAC will be placed in a read-only mode.</span></span> <span data-ttu-id="aec9b-121">Това означава, че ще можете да премахвате само съществуващи търсения и задържания.</span><span class="sxs-lookup"><span data-stu-id="aec9b-121">This means you'll only be able to remove existing searches and holds.</span></span>

<span data-ttu-id="aec9b-122">**За повече информация вижте:**</span><span class="sxs-lookup"><span data-stu-id="aec9b-122">**For more information, see**:</span></span>

 - [<span data-ttu-id="aec9b-123">Мигриране на стари eDiscovery търсения и задържа в центъра за съответствие на Microsoft 365</span><span class="sxs-lookup"><span data-stu-id="aec9b-123">Migrate legacy eDiscovery searches and holds to the Microsoft 365 compliance center</span></span>](https://docs.microsoft.com/en-us/microsoft-365/compliance/migrate-legacy-ediscovery-searches-and-holds)
 - [<span data-ttu-id="aec9b-124">Оттегляне на наследените инструменти за откриване на електронни данни</span><span class="sxs-lookup"><span data-stu-id="aec9b-124">Retirement of legacy eDiscovery tools</span></span>](https://docs.microsoft.com/en-us/microsoft-365/compliance/legacy-ediscovery-retirement)
 - [<span data-ttu-id="aec9b-125">Често задавани въпроси за откриване то на място и за задържане на място</span><span class="sxs-lookup"><span data-stu-id="aec9b-125">FAQs about In-Place eDiscovery and In-Place Holds</span></span>](https://docs.microsoft.com/en-us/microsoft-365/compliance/legacy-ediscovery-retirement#faqs-about-in-place-ediscovery-and-in-place-holds)



