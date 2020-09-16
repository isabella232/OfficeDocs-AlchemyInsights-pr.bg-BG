---
title: Оттегляне на стари инструменти за откриване на електронни данни
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9001487"
- "3523"
ms.openlocfilehash: 2315c4c651a83f0ecc78c0171f32aba13bc93f8c
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: bg-BG
ms.lasthandoff: 09/14/2020
ms.locfileid: "47727772"
---
# <a name="retirement-of-legacy-ediscovery-tools"></a><span data-ttu-id="ad5a0-102">Оттегляне на стари инструменти за откриване на електронни данни</span><span class="sxs-lookup"><span data-stu-id="ad5a0-102">Retirement of Legacy eDiscovery Tools</span></span>

<span data-ttu-id="ad5a0-103">Като резултат от новата и усъвършенстваната функционалност на откриването на електронни данни в центъра за съответствие на Microsoft 365, следните инструменти за откриване на електронни данни и кратки команди ще бъдат оттеглени през следващите месеци:</span><span class="sxs-lookup"><span data-stu-id="ad5a0-103">As a result of the new and improved eDiscovery functionality in Microsoft 365 Compliance center, the following legacy eDiscovery tools and commandlets will be retired in the coming months:</span></span>

- <span data-ttu-id="ad5a0-104">[Откриване](https://docs.microsoft.com/exchange/security-and-compliance/in-place-ediscovery/in-place-ediscovery) на електронни данни и [задържане](https://docs.microsoft.com/exchange/security-and-compliance/create-or-remove-in-place-holds) на места в центъра за администриране на Exchange.</span><span class="sxs-lookup"><span data-stu-id="ad5a0-104">[In-Place eDiscovery](https://docs.microsoft.com/exchange/security-and-compliance/in-place-ediscovery/in-place-ediscovery) and [In-Place Holds](https://docs.microsoft.com/exchange/security-and-compliance/create-or-remove-in-place-holds) in the Exchange admin center.</span></span>

- <span data-ttu-id="ad5a0-105">Кратките команди на PowerShell на Exchange Online, които поддържат откриването на електронни данни и задържане на места.</span><span class="sxs-lookup"><span data-stu-id="ad5a0-105">The Exchange Online PowerShell cmdlets that support In-Place eDiscovery and In-Place Holds.</span></span> <span data-ttu-id="ad5a0-106">(Тези кратки команди се идентифицират общо като \*-MailboxSearch кратки команди.) Това включва следните кратки команди:</span><span class="sxs-lookup"><span data-stu-id="ad5a0-106">(These cmdlets are collectively identified as \*-MailboxSearch cmdlets.) This includes the following cmdlets:</span></span>

    - [<span data-ttu-id="ad5a0-107">New-MailboxSearch</span><span class="sxs-lookup"><span data-stu-id="ad5a0-107">New-MailboxSearch</span></span>](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance-content-search/new-mailboxsearch)
    - [<span data-ttu-id="ad5a0-108">Start-MailboxSearch</span><span class="sxs-lookup"><span data-stu-id="ad5a0-108">Start-MailboxSearch</span></span>](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance-content-search/start-mailboxsearch)
    - [<span data-ttu-id="ad5a0-109">Стоп-MailboxSearch</span><span class="sxs-lookup"><span data-stu-id="ad5a0-109">Stop-MailboxSearch</span></span>](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance-content-search/stop-mailboxsearch)
    - [<span data-ttu-id="ad5a0-110">Set-MailboxSearch</span><span class="sxs-lookup"><span data-stu-id="ad5a0-110">Set-MailboxSearch</span></span>](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance-content-search/set-mailboxsearch)

- <span data-ttu-id="ad5a0-111">Кратката команда [търсене – пощенска кутия](https://docs.microsoft.com/powershell/module/exchange/mailboxes/search-mailbox?view=exchange-ps) в Exchange Online PowerShell.</span><span class="sxs-lookup"><span data-stu-id="ad5a0-111">The [Search-Mailbox](https://docs.microsoft.com/powershell/module/exchange/mailboxes/search-mailbox?view=exchange-ps) cmdlet in Exchange Online PowerShell.</span></span>
- <span data-ttu-id="ad5a0-112">Следните операции в API на уеб услугите на Exchange:</span><span class="sxs-lookup"><span data-stu-id="ad5a0-112">The following operations in the Exchange Web Services API:</span></span>
    - [<span data-ttu-id="ad5a0-113">GetSearchableMailboxes</span><span class="sxs-lookup"><span data-stu-id="ad5a0-113">GetSearchableMailboxes</span></span>](https://docs.microsoft.com/exchange/client-developer/web-service-reference/getsearchablemailboxes-operation)
    - [<span data-ttu-id="ad5a0-114">SetHoldOnMailboxes</span><span class="sxs-lookup"><span data-stu-id="ad5a0-114">SetHoldOnMailboxes</span></span>](https://docs.microsoft.com/exchange/client-developer/web-service-reference/setholdonmailboxes-operation)
    - [<span data-ttu-id="ad5a0-115">GetHoldOnMailboxes</span><span class="sxs-lookup"><span data-stu-id="ad5a0-115">GetHoldOnMailboxes</span></span>](https://docs.microsoft.com/exchange/client-developer/web-service-reference/getholdonmailboxes-operation)

- [<span data-ttu-id="ad5a0-116">Разширено откриване на електронни данни v 1.0</span><span class="sxs-lookup"><span data-stu-id="ad5a0-116">Advanced eDiscovery v1.0</span></span>](https://docs.microsoft.com/microsoft-365/compliance/office-365-advanced-ediscovery)

<span data-ttu-id="ad5a0-117">**Времева линия за пенсиониране**:</span><span class="sxs-lookup"><span data-stu-id="ad5a0-117">**Timeline for retirement**:</span></span>
- <span data-ttu-id="ad5a0-118">**1 юли 2020 г.** Вече не можете да създавате нови търсения и трюмове, но можете да изпълнявате, редактирате и изтривате съществуващи търсения на свой собствен риск.</span><span class="sxs-lookup"><span data-stu-id="ad5a0-118">**July 1, 2020** You can no longer create new searches and holds, but you can run, edit, and delete existing searches at your own risk.</span></span> <span data-ttu-id="ad5a0-119">Поддръжката на Microsoft вече не поддържа откриване на електронни данни на места & съдържа в EAC.</span><span class="sxs-lookup"><span data-stu-id="ad5a0-119">Microsoft Support no longer supports In-Place eDiscovery & Holds in the EAC.</span></span>
    
- <span data-ttu-id="ad5a0-120">**1 октомври 2020 г.** Откриване на електронни данни на място & съдържа функционалност в EAC ще бъдат поставени в режим само за четене, така че да можете да премахвате съществуващите търсения и съдържания.</span><span class="sxs-lookup"><span data-stu-id="ad5a0-120">**October 1, 2020** In-Place eDiscovery & Holds functionality in the EAC will be placed in read-only mode, so you can only remove existing searches and holds.</span></span>

<span data-ttu-id="ad5a0-121">**За повече информация вижте**:</span><span class="sxs-lookup"><span data-stu-id="ad5a0-121">**For more information, see**:</span></span>

 - [<span data-ttu-id="ad5a0-122">Мигриране на стари търсения на откриване на електронни данни и задържане в центъра за съответствие на Microsoft 365</span><span class="sxs-lookup"><span data-stu-id="ad5a0-122">Migrate legacy eDiscovery searches and holds to the Microsoft 365 compliance center</span></span>](https://docs.microsoft.com/microsoft-365/compliance/migrate-legacy-ediscovery-searches-and-holds)
 - [<span data-ttu-id="ad5a0-123">Оттегляне на стари инструменти за откриване на електронни данни</span><span class="sxs-lookup"><span data-stu-id="ad5a0-123">Retirement of legacy eDiscovery tools</span></span>](https://docs.microsoft.com/microsoft-365/compliance/legacy-ediscovery-retirement)
 - [<span data-ttu-id="ad5a0-124">ЧЗВ за откриване на електронни данни на места и задържане на места</span><span class="sxs-lookup"><span data-stu-id="ad5a0-124">FAQs about In-Place eDiscovery and In-Place Holds</span></span>](https://docs.microsoft.com/microsoft-365/compliance/legacy-ediscovery-retirement#faqs-about-in-place-ediscovery-and-in-place-holds)



