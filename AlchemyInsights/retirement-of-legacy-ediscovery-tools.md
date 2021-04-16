---
title: Оттегляне на наследените инструменти за откриване на електронни данни
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9001487"
- "3523"
ms.openlocfilehash: 986c78f20e7b8c303c302913d63d817a56ce2896
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: bg-BG
ms.lasthandoff: 04/15/2021
ms.locfileid: "51798538"
---
# <a name="retirement-of-legacy-ediscovery-tools"></a><span data-ttu-id="9e11b-102">Оттегляне на наследените инструменти за откриване на електронни данни</span><span class="sxs-lookup"><span data-stu-id="9e11b-102">Retirement of Legacy eDiscovery Tools</span></span>

<span data-ttu-id="9e11b-103">В резултат на новата и подобрена функционалност за откриване на електронни данни в центъра за съответствие на Microsoft 365 следните стари инструменти и командни команди за откриване на електронни данни ще бъдат оттеглени през следващите месеци:</span><span class="sxs-lookup"><span data-stu-id="9e11b-103">As a result of the new and improved eDiscovery functionality in Microsoft 365 Compliance center, the following legacy eDiscovery tools and commandlets will be retired in the coming months:</span></span>

- <span data-ttu-id="9e11b-104">[Откриване на електронни данни на](https://docs.microsoft.com/exchange/security-and-compliance/in-place-ediscovery/in-place-ediscovery) място и задържане на място [в](https://docs.microsoft.com/exchange/security-and-compliance/create-or-remove-in-place-holds) центъра за администриране на Exchange.</span><span class="sxs-lookup"><span data-stu-id="9e11b-104">[In-Place eDiscovery](https://docs.microsoft.com/exchange/security-and-compliance/in-place-ediscovery/in-place-ediscovery) and [In-Place Holds](https://docs.microsoft.com/exchange/security-and-compliance/create-or-remove-in-place-holds) in the Exchange admin center.</span></span>

- <span data-ttu-id="9e11b-105">Кратките команди на PowerShell на Exchange Online, които поддържат In-Place откриване на електронни данни и In-Place задържа.</span><span class="sxs-lookup"><span data-stu-id="9e11b-105">The Exchange Online PowerShell cmdlets that support In-Place eDiscovery and In-Place Holds.</span></span> <span data-ttu-id="9e11b-106">(Тези кратки команди се идентифицират колективно като кратки команди \*-MailboxSearch.) Това включва следните кратки команди:</span><span class="sxs-lookup"><span data-stu-id="9e11b-106">(These cmdlets are collectively identified as \*-MailboxSearch cmdlets.) This includes the following cmdlets:</span></span>

    - [<span data-ttu-id="9e11b-107">New-MailboxSearch</span><span class="sxs-lookup"><span data-stu-id="9e11b-107">New-MailboxSearch</span></span>](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance-content-search/new-mailboxsearch)
    - [<span data-ttu-id="9e11b-108">Start-MailboxSearch</span><span class="sxs-lookup"><span data-stu-id="9e11b-108">Start-MailboxSearch</span></span>](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance-content-search/start-mailboxsearch)
    - [<span data-ttu-id="9e11b-109">Stop-MailboxSearch</span><span class="sxs-lookup"><span data-stu-id="9e11b-109">Stop-MailboxSearch</span></span>](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance-content-search/stop-mailboxsearch)
    - [<span data-ttu-id="9e11b-110">Set-MailboxSearch</span><span class="sxs-lookup"><span data-stu-id="9e11b-110">Set-MailboxSearch</span></span>](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance-content-search/set-mailboxsearch)

- <span data-ttu-id="9e11b-111">Кратката [команда "Пощенска кутия](https://docs.microsoft.com/powershell/module/exchange/mailboxes/search-mailbox?view=exchange-ps) за търсене" в Exchange Online PowerShell.</span><span class="sxs-lookup"><span data-stu-id="9e11b-111">The [Search-Mailbox](https://docs.microsoft.com/powershell/module/exchange/mailboxes/search-mailbox?view=exchange-ps) cmdlet in Exchange Online PowerShell.</span></span>
- <span data-ttu-id="9e11b-112">Следните операции в API на Exchange Web Services:</span><span class="sxs-lookup"><span data-stu-id="9e11b-112">The following operations in the Exchange Web Services API:</span></span>
    - [<span data-ttu-id="9e11b-113">GetSearchableMailboxes</span><span class="sxs-lookup"><span data-stu-id="9e11b-113">GetSearchableMailboxes</span></span>](https://docs.microsoft.com/exchange/client-developer/web-service-reference/getsearchablemailboxes-operation)
    - [<span data-ttu-id="9e11b-114">SetHoldOnMailboxes</span><span class="sxs-lookup"><span data-stu-id="9e11b-114">SetHoldOnMailboxes</span></span>](https://docs.microsoft.com/exchange/client-developer/web-service-reference/setholdonmailboxes-operation)
    - [<span data-ttu-id="9e11b-115">GetHoldOnMailboxes</span><span class="sxs-lookup"><span data-stu-id="9e11b-115">GetHoldOnMailboxes</span></span>](https://docs.microsoft.com/exchange/client-developer/web-service-reference/getholdonmailboxes-operation)

- [<span data-ttu-id="9e11b-116">Advanced eDiscovery v1.0</span><span class="sxs-lookup"><span data-stu-id="9e11b-116">Advanced eDiscovery v1.0</span></span>](https://docs.microsoft.com/microsoft-365/compliance/office-365-advanced-ediscovery)

<span data-ttu-id="9e11b-117">**Времева линия за пенсиониране:**</span><span class="sxs-lookup"><span data-stu-id="9e11b-117">**Timeline for retirement**:</span></span>
- <span data-ttu-id="9e11b-118">**1 юли 2020 г.** Вече не можете да създавате нови търсения и задържания, но можете да изпълнявате, редактирате и изтривате съществуващи търсения на свой собствен риск.</span><span class="sxs-lookup"><span data-stu-id="9e11b-118">**July 1, 2020** You can no longer create new searches and holds, but you can run, edit, and delete existing searches at your own risk.</span></span> <span data-ttu-id="9e11b-119">Поддръжката на Microsoft вече не In-Place откриване на електронни данни & задържа в EAC.</span><span class="sxs-lookup"><span data-stu-id="9e11b-119">Microsoft Support no longer supports In-Place eDiscovery & Holds in the EAC.</span></span>
    
- <span data-ttu-id="9e11b-120">**1 октомври 2020** г. In-Place откриване на електронни данни & Има функционалност в EAC ще бъде поставена в режим само за четене, така че можете да премахвате само съществуващи търсения и задържания.</span><span class="sxs-lookup"><span data-stu-id="9e11b-120">**October 1, 2020** In-Place eDiscovery & Holds functionality in the EAC will be placed in read-only mode, so you can only remove existing searches and holds.</span></span>

<span data-ttu-id="9e11b-121">**За повече информация вижте**:</span><span class="sxs-lookup"><span data-stu-id="9e11b-121">**For more information, see**:</span></span>

 - [<span data-ttu-id="9e11b-122">Мигриране на стари търсения за откриване на електронни данни и задържане в центъра за съответствие на Microsoft 365</span><span class="sxs-lookup"><span data-stu-id="9e11b-122">Migrate legacy eDiscovery searches and holds to the Microsoft 365 compliance center</span></span>](https://docs.microsoft.com/microsoft-365/compliance/migrate-legacy-ediscovery-searches-and-holds)
 - [<span data-ttu-id="9e11b-123">Оттегляне на стари инструменти за откриване на електронни данни</span><span class="sxs-lookup"><span data-stu-id="9e11b-123">Retirement of legacy eDiscovery tools</span></span>](https://docs.microsoft.com/microsoft-365/compliance/legacy-ediscovery-retirement)
 - [<span data-ttu-id="9e11b-124">Често задавани въпроси за In-Place откриване на електронни и In-Place задържания</span><span class="sxs-lookup"><span data-stu-id="9e11b-124">FAQs about In-Place eDiscovery and In-Place Holds</span></span>](https://docs.microsoft.com/microsoft-365/compliance/legacy-ediscovery-retirement#faqs-about-in-place-ediscovery-and-in-place-holds)



