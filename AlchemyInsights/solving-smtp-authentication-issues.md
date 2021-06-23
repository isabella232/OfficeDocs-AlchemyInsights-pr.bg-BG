---
title: Разрешаване на SMTP удостоверяване и отстраняване на неизправности
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "3000003"
- "5652"
ms.openlocfilehash: 4695a2f111823739c4d87fa2b262a5e64e080955
ms.sourcegitcommit: 2103d706492ad7ee9596344714c0520569ebd6af
ms.translationtype: MT
ms.contentlocale: bg-BG
ms.lasthandoff: 06/23/2021
ms.locfileid: "53077640"
---
# <a name="enable-smtp-authentication-and-troubleshooting"></a><span data-ttu-id="23e0b-102">Разрешаване на SMTP удостоверяване и отстраняване на неизправности</span><span class="sxs-lookup"><span data-stu-id="23e0b-102">Enable SMTP authentication and troubleshooting</span></span>

<span data-ttu-id="23e0b-103">Ако искате да разрешите SMTP удостоверяване за пощенска кутия или получавате грешка "Клиентът не е удостоверен", "Неуспешно удостоверяване" или "SmtpClientAuthentication" с код 5.7.57 или 5.7.3 или 5.7.139, когато се опитате да препредавате имейл чрез удостоверяване на устройство или приложение с Microsoft 365, изпълнете тези три действия, за да разрешите проблема:</span><span class="sxs-lookup"><span data-stu-id="23e0b-103">If you want to enable SMTP authentication for a mailbox or you're getting a "Client not authenticated", "Authentication unsuccessful", or "SmtpClientAuthentication" error with code 5.7.57 or 5.7.3 or 5.7.139 when you try to relay email by authenticating a device or application with Microsoft 365, perform these three actions to resolve the issue:</span></span>

1. <span data-ttu-id="23e0b-104">[Забранете настройките за защита на Azure по подразбиране,](/azure/active-directory/fundamentals/concept-fundamentals-security-defaults) като превключвате **разрешаването на защита по подразбиране** на **Не**.</span><span class="sxs-lookup"><span data-stu-id="23e0b-104">Disable the [Azure security defaults](/azure/active-directory/fundamentals/concept-fundamentals-security-defaults) by toggling **Enable security defaults** to **No**.</span></span>

    <span data-ttu-id="23e0b-105">a.</span><span class="sxs-lookup"><span data-stu-id="23e0b-105">a.</span></span> <span data-ttu-id="23e0b-106">Влезте в портала на Azure като администратор на защитата, администратор на условен достъп или глобален администратор.</span><span class="sxs-lookup"><span data-stu-id="23e0b-106">Sign in to the Azure portal as a Security administrator, Conditional Access administrator, or global administrator.</span></span><BR/>
    <span data-ttu-id="23e0b-107">б.</span><span class="sxs-lookup"><span data-stu-id="23e0b-107">b.</span></span> <span data-ttu-id="23e0b-108">Отидете до Azure Active Directory > **свойства**.</span><span class="sxs-lookup"><span data-stu-id="23e0b-108">Browse to Azure Active Directory > **Properties**.</span></span><BR/>
    <span data-ttu-id="23e0b-109">в.</span><span class="sxs-lookup"><span data-stu-id="23e0b-109">c.</span></span> <span data-ttu-id="23e0b-110">Изберете **Управление на настройките по подразбиране за защита**.</span><span class="sxs-lookup"><span data-stu-id="23e0b-110">Select **Manage security defaults**.</span></span><BR/>
    <span data-ttu-id="23e0b-111">г.</span><span class="sxs-lookup"><span data-stu-id="23e0b-111">d.</span></span> <span data-ttu-id="23e0b-112">Задайте **Разрешаване на настройките по подразбиране за защита** на **Не**.</span><span class="sxs-lookup"><span data-stu-id="23e0b-112">Set **Enable security defaults** to **No**.</span></span><BR/>
    <span data-ttu-id="23e0b-113">д.</span><span class="sxs-lookup"><span data-stu-id="23e0b-113">e.</span></span> <span data-ttu-id="23e0b-114">Изберете **Записване**.</span><span class="sxs-lookup"><span data-stu-id="23e0b-114">Select **Save**.</span></span>

2. <span data-ttu-id="23e0b-115">[Разрешаване на изпращането на SMTP на](/exchange/clients-and-mobile-in-exchange-online/authenticated-client-smtp-submission#enable-smtp-auth-for-specific-mailboxes) клиента в лицензираната пощенска кутия.</span><span class="sxs-lookup"><span data-stu-id="23e0b-115">[Enable Client SMTP submission](/exchange/clients-and-mobile-in-exchange-online/authenticated-client-smtp-submission#enable-smtp-auth-for-specific-mailboxes) on the licensed mailbox.</span></span>

    <span data-ttu-id="23e0b-116">a.</span><span class="sxs-lookup"><span data-stu-id="23e0b-116">a.</span></span> <span data-ttu-id="23e0b-117">От Център за администриране на Microsoft 365 отидете на **Активни потребители** и изберете потребителя.</span><span class="sxs-lookup"><span data-stu-id="23e0b-117">From the Microsoft 365 admin center, go to **Active Users**, and select the user.</span></span><BR/>
    <span data-ttu-id="23e0b-118">б.</span><span class="sxs-lookup"><span data-stu-id="23e0b-118">b.</span></span> <span data-ttu-id="23e0b-119">Отидете в раздела Поща и под Приложения **за имейл изберете** Управление на имейл **приложения**.</span><span class="sxs-lookup"><span data-stu-id="23e0b-119">Go to Mail tab, and under **Email apps**, select **Manage email apps**.</span></span><BR/>
    <span data-ttu-id="23e0b-120">г.</span><span class="sxs-lookup"><span data-stu-id="23e0b-120">d.</span></span> <span data-ttu-id="23e0b-121">Уверете се, **че удостоверен SMTP** е отметнато (разрешено).</span><span class="sxs-lookup"><span data-stu-id="23e0b-121">Make sure **Authenticated SMTP** is checked (enabled).</span></span><BR/>
    <span data-ttu-id="23e0b-122">д.</span><span class="sxs-lookup"><span data-stu-id="23e0b-122">e.</span></span> <span data-ttu-id="23e0b-123">Изберете **Запиши промените**.</span><span class="sxs-lookup"><span data-stu-id="23e0b-123">Select **Save changes**.</span></span><BR/>

3. <span data-ttu-id="23e0b-124">[Забраняване на многофакторното удостоверяване (MFA)](/microsoft-365/admin/security-and-compliance/set-up-multi-factor-authentication#turn-off-legacy-per-user-mfa) в лицензираната пощенска кутия.</span><span class="sxs-lookup"><span data-stu-id="23e0b-124">[Disable Multi-Factor Authentication (MFA)](/microsoft-365/admin/security-and-compliance/set-up-multi-factor-authentication#turn-off-legacy-per-user-mfa) on the licensed mailbox.</span></span>

    <span data-ttu-id="23e0b-125">a.</span><span class="sxs-lookup"><span data-stu-id="23e0b-125">a.</span></span> <span data-ttu-id="23e0b-126">Отидете на Център за администриране на Microsoft 365 и в менюто за навигация отляво изберете **Потребители**  >  **Активни потребители**.</span><span class="sxs-lookup"><span data-stu-id="23e0b-126">Go to the Microsoft 365 admin center, and in the left navigation menu select **Users** > **Active users**.</span></span><BR/>
    <span data-ttu-id="23e0b-127">б.</span><span class="sxs-lookup"><span data-stu-id="23e0b-127">b.</span></span> <span data-ttu-id="23e0b-128">Изберете **Многофакторно удостоверяване**.</span><span class="sxs-lookup"><span data-stu-id="23e0b-128">Select **Multi-factor authentication**.</span></span><BR/>
    <span data-ttu-id="23e0b-129">в.</span><span class="sxs-lookup"><span data-stu-id="23e0b-129">c.</span></span> <span data-ttu-id="23e0b-130">Изберете потребителя и **забранете многофакторното удостоверяване**.</span><span class="sxs-lookup"><span data-stu-id="23e0b-130">Select the user and disable **Multi-Factor auth**.</span></span><BR/>
