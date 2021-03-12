---
title: Правила за пароли
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 03/11/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004595"
- "9277"
ms.openlocfilehash: 826e266d08aa68c0d4213d8058a0244f404fe965
ms.sourcegitcommit: 186281d0b87d67f041c127d4334faa937da9a48a
ms.translationtype: MT
ms.contentlocale: bg-BG
ms.lasthandoff: 03/11/2021
ms.locfileid: "50743182"
---
# <a name="password-policies"></a><span data-ttu-id="11393-102">Правила за пароли</span><span class="sxs-lookup"><span data-stu-id="11393-102">Password policies</span></span>

<span data-ttu-id="11393-103">**Имам проблеми с правилата за парола за потребител**</span><span class="sxs-lookup"><span data-stu-id="11393-103">**I'm having problems with the password policy for a user**</span></span>

- <span data-ttu-id="11393-104">Правилата за пароли за един потребител зависят от това дали потребителят е само в облака, или локален.</span><span class="sxs-lookup"><span data-stu-id="11393-104">The password policy for a user depends on whether the user is cloud only or on-premises.</span></span>
- <span data-ttu-id="11393-105">Само в облака потребителите трябва да изберат парола, която отговаря на изискванията в тази статия: [правила за пароли, приложими само за потребителските акаунти в облака](https://docs.microsoft.com/azure/active-directory/authentication/concept-sspr-policy?WT.mc_id=Portal-Microsoft_Azure_Support#password-policies-that-only-apply-to-cloud-user-accounts)</span><span class="sxs-lookup"><span data-stu-id="11393-105">Cloud only users must choose a password that meets the requirements in this article: [Password policies that only apply to cloud user accounts](https://docs.microsoft.com/azure/active-directory/authentication/concept-sspr-policy?WT.mc_id=Portal-Microsoft_Azure_Support#password-policies-that-only-apply-to-cloud-user-accounts)</span></span>
- <span data-ttu-id="11393-106">Локалните потребители трябва да изберат парола, която отговаря на локалните изисквания.</span><span class="sxs-lookup"><span data-stu-id="11393-106">On-premises users must choose a password that meets the on-premises requirements.</span></span> <span data-ttu-id="11393-107">Ако локален потребител не е в състояние да зададе паролата си, проверете локалните изисквания.</span><span class="sxs-lookup"><span data-stu-id="11393-107">If an on-premises user is unable to set their password, check your on-premises requirements.</span></span>

<span data-ttu-id="11393-108">**Не знам как да задам или да проверя правилата за изтичане на парола**</span><span class="sxs-lookup"><span data-stu-id="11393-108">**I don't know how to set or check password expiration policies**</span></span>

- <span data-ttu-id="11393-109">Можете да зададете и да проверите правилата за изтичане на срока за потребители в облака в своя клиент с помощта на PowerShell.</span><span class="sxs-lookup"><span data-stu-id="11393-109">You can set and check the expiration policy for cloud users in your tenant by using PowerShell.</span></span> <span data-ttu-id="11393-110">Следвайте инструкциите в тази статия: [Задаване или проверка на правилата за пароли с помощта на PowerShell](https://docs.microsoft.com/azure/active-directory/authentication/concept-sspr-policy?WT.mc_id=Portal-Microsoft_Azure_Support#set-or-check-the-password-policies-by-using-powershell)</span><span class="sxs-lookup"><span data-stu-id="11393-110">Follow the instructions in this article: [Set or check the password policies by using PowerShell](https://docs.microsoft.com/azure/active-directory/authentication/concept-sspr-policy?WT.mc_id=Portal-Microsoft_Azure_Support#set-or-check-the-password-policies-by-using-powershell)</span></span>
- <span data-ttu-id="11393-111">Правилата за изтичане на парола за локални потребители се задават във вашата локална реклама.</span><span class="sxs-lookup"><span data-stu-id="11393-111">The password expiration policy for on-premises users is set in your on-premises AD.</span></span>

<span data-ttu-id="11393-112">**Други полезни връзки:**</span><span class="sxs-lookup"><span data-stu-id="11393-112">**Other Helpful links:**</span></span>
- [<span data-ttu-id="11393-113">Първи стъпки в нулирането на паролата</span><span class="sxs-lookup"><span data-stu-id="11393-113">Getting Started with Password Reset</span></span>](https://docs.microsoft.com/azure/active-directory/authentication/concept-sspr-policy?WT.mc_id=Portal-Microsoft_Azure_Support#set-or-check-the-password-policies-by-using-powershell)
- [<span data-ttu-id="11393-114">Отстраняване на неизправности при нулиране на паролата на администратор</span><span class="sxs-lookup"><span data-stu-id="11393-114">Troubleshoot Administrator-initiated Password Reset</span></span>](https://docs.microsoft.com/azure/active-directory/active-directory-passwords-troubleshoot?WT.mc_id=Portal-Microsoft_Azure_Support#troubleshoot-the-password-reset-portal)
