---
title: Пенсиониране на наследените инструменти за откриване на електронни данни
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
ms.openlocfilehash: af9a0bd8ff4294575ac68f37d4997bb50b132ce7
ms.sourcegitcommit: 9ab422063e5a474c92ed956d42d222b90336fecb
ms.translationtype: MT
ms.contentlocale: bg-BG
ms.lasthandoff: 03/11/2020
ms.locfileid: "42600347"
---
# <a name="retirement-of-legacy-ediscovery-tools"></a><span data-ttu-id="5d775-102">Пенсиониране на наследените инструменти за откриване на електронни данни</span><span class="sxs-lookup"><span data-stu-id="5d775-102">Retirement of Legacy eDiscovery Tools</span></span>

<span data-ttu-id="5d775-103">В резултат на новите и подобрени функции за откриване на електронни данни в центъра за съответствие на Microsoft 365, следните стари инструменти и командни елементи ще се оттеглеят през следващите месеци:</span><span class="sxs-lookup"><span data-stu-id="5d775-103">As a result of the new and improved eDiscovery functionality in Microsoft 365 Compliance center, the following legacy eDiscovery tools and commandlets will be retired in the coming months:</span></span>

- <span data-ttu-id="5d775-104">[Откриването на електронни данни](https://docs.microsoft.com/exchange/security-and-compliance/in-place-ediscovery/in-place-ediscovery) на място и [задържането на място](https://docs.microsoft.com/exchange/security-and-compliance/create-or-remove-in-place-holds) в центъра за администриране на Exchange.</span><span class="sxs-lookup"><span data-stu-id="5d775-104">[In-Place eDiscovery](https://docs.microsoft.com/exchange/security-and-compliance/in-place-ediscovery/in-place-ediscovery) and [In-Place Holds](https://docs.microsoft.com/exchange/security-and-compliance/create-or-remove-in-place-holds) in the Exchange admin center.</span></span>

- <span data-ttu-id="5d775-105">Кратки команди на Exchange Online PowerShell, които поддържат на място eDiscovery и задържа.</span><span class="sxs-lookup"><span data-stu-id="5d775-105">The Exchange Online PowerShell cmdlets that support In-Place eDiscovery and In-Place Holds.</span></span> <span data-ttu-id="5d775-106">(Тези кратки команди са общо идентифицирани като \*-MailboxSearch кратки команди.) Това включва следните кратки команди:</span><span class="sxs-lookup"><span data-stu-id="5d775-106">(These cmdlets are collectively identified as \*-MailboxSearch cmdlets.) This includes the following cmdlets:</span></span>

    - [<span data-ttu-id="5d775-107">Търсене на нова пощенска кутия</span><span class="sxs-lookup"><span data-stu-id="5d775-107">New-MailboxSearch</span></span>](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance-content-search/new-mailboxsearch)
    - [<span data-ttu-id="5d775-108">Търсене на начална пощенска кутия</span><span class="sxs-lookup"><span data-stu-id="5d775-108">Start-MailboxSearch</span></span>](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance-content-search/start-mailboxsearch)
    - [<span data-ttu-id="5d775-109">Търсене на стоп-пощенска кутия</span><span class="sxs-lookup"><span data-stu-id="5d775-109">Stop-MailboxSearch</span></span>](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance-content-search/stop-mailboxsearch)
    - [<span data-ttu-id="5d775-110">Търсене на set-пощенска кутия</span><span class="sxs-lookup"><span data-stu-id="5d775-110">Set-MailboxSearch</span></span>](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance-content-search/set-mailboxsearch)

- <span data-ttu-id="5d775-111">Пощенска [кутия за търсене](https://docs.microsoft.com/powershell/module/exchange/mailboxes/search-mailbox?view=exchange-ps) команда в Exchange Онлайн PowerShell.</span><span class="sxs-lookup"><span data-stu-id="5d775-111">The [Search-Mailbox](https://docs.microsoft.com/powershell/module/exchange/mailboxes/search-mailbox?view=exchange-ps) cmdlet in Exchange Online PowerShell.</span></span>
- <span data-ttu-id="5d775-112">Следните операции в API на уеб услуги на Exchange:</span><span class="sxs-lookup"><span data-stu-id="5d775-112">The following operations in the Exchange Web Services API:</span></span>
    - [<span data-ttu-id="5d775-113">Получаване на пощенски кутии за търсене</span><span class="sxs-lookup"><span data-stu-id="5d775-113">GetSearchableMailboxes</span></span>](https://docs.microsoft.com/exchange/client-developer/web-service-reference/getsearchablemailboxes-operation)
    - [<span data-ttu-id="5d775-114">Задаване на пощенски кутии</span><span class="sxs-lookup"><span data-stu-id="5d775-114">SetHoldOnMailboxes</span></span>](https://docs.microsoft.com/exchange/client-developer/web-service-reference/setholdonmailboxes-operation)
    - [<span data-ttu-id="5d775-115">Пощенски кутии</span><span class="sxs-lookup"><span data-stu-id="5d775-115">GetHoldOnMailboxes</span></span>](https://docs.microsoft.com/exchange/client-developer/web-service-reference/getholdonmailboxes-operation)

- [<span data-ttu-id="5d775-116">Разширено откриване на електронни данни v1.0 на Office 365</span><span class="sxs-lookup"><span data-stu-id="5d775-116">Office 365 Advanced eDiscovery v1.0</span></span>](https://docs.microsoft.com/microsoft-365/compliance/office-365-advanced-ediscovery)

<span data-ttu-id="5d775-117">**Времева линия за пенсиониране:**</span><span class="sxs-lookup"><span data-stu-id="5d775-117">**Timeline for retirement**:</span></span>
- <span data-ttu-id="5d775-118">1 април 2020 г.: Няма да можете да създавате нови търсения и задържания, но все още можете да изпълнявате, редактирате и изтривате съществуващи търсения на свой собствен риск.</span><span class="sxs-lookup"><span data-stu-id="5d775-118">April 1, 2020: You won't be able to create new searches and holds, but you can still run, edit, and delete existing searches at your own risk.</span></span> <span data-ttu-id="5d775-119">Поддръжката на Microsoft вече няма да поддържа на място & за откриване на електронни данни в EAC.</span><span class="sxs-lookup"><span data-stu-id="5d775-119">Microsoft Support will no longer support In-Place eDiscovery & Holds in the EAC.</span></span>

- <span data-ttu-id="5d775-120">1 юли 2020 г.: & за откриване на електронни данни на място притежава функции в EAC ще бъдат поставени в режим само за четене.</span><span class="sxs-lookup"><span data-stu-id="5d775-120">July 1, 2020: The In-Place eDiscovery & Holds functionality in the EAC will be placed in a read-only mode.</span></span> <span data-ttu-id="5d775-121">Това означава, че ще можете да премахвате само съществуващи търсения и задържания.</span><span class="sxs-lookup"><span data-stu-id="5d775-121">This means you'll only be able to remove existing searches and holds.</span></span>

<span data-ttu-id="5d775-122">**За повече информация вижте:**</span><span class="sxs-lookup"><span data-stu-id="5d775-122">**For more information, see**:</span></span>

 - [<span data-ttu-id="5d775-123">Мигриране на следене на откриването на електронни данни и задържане в центъра за съответствие на Microsoft 365</span><span class="sxs-lookup"><span data-stu-id="5d775-123">Migrate legacy eDiscovery searches and holds to the Microsoft 365 compliance center</span></span>](https://docs.microsoft.com/microsoft-365/compliance/migrate-legacy-ediscovery-searches-and-holds)
 - [<span data-ttu-id="5d775-124">Пенсиониране на наследените инструменти за откриване на електронни данни</span><span class="sxs-lookup"><span data-stu-id="5d775-124">Retirement of legacy eDiscovery tools</span></span>](https://docs.microsoft.com/microsoft-365/compliance/legacy-ediscovery-retirement)
 - [<span data-ttu-id="5d775-125">Често задавани въпроси за откриването на електронни данни на място и задържанията на място</span><span class="sxs-lookup"><span data-stu-id="5d775-125">FAQs about In-Place eDiscovery and In-Place Holds</span></span>](https://docs.microsoft.com/microsoft-365/compliance/legacy-ediscovery-retirement#faqs-about-in-place-ediscovery-and-in-place-holds)



