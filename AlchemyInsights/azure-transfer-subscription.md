---
title: Прехвърляне на собствеността на Azure за фактуриране
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9003560"
- "6849"
ms.openlocfilehash: e9a1e74b321e2c2dda5f7a4f69681a0acf0635d5
ms.sourcegitcommit: a5ba4dc8c349ed79147f67b62bde544281f7c106
ms.translationtype: MT
ms.contentlocale: bg-BG
ms.lasthandoff: 11/03/2020
ms.locfileid: "48922004"
---
# <a name="transfer-azure-billing-ownership"></a><span data-ttu-id="b7f21-102">Прехвърляне на собствеността на Azure за фактуриране</span><span class="sxs-lookup"><span data-stu-id="b7f21-102">Transfer Azure billing ownership</span></span>

<span data-ttu-id="b7f21-103">Влезте в портала на [Azure](https://portal.azure.com/) като администратор на акаунт за фактуриране, който има абонамента, който искате да прехвърлите.</span><span class="sxs-lookup"><span data-stu-id="b7f21-103">Sign in to the [Azure portal](https://portal.azure.com/) as an administrator of the billing account that has the subscription that you want to transfer.</span></span> <span data-ttu-id="b7f21-104">Ако не сте сигурни дали сте администратор, или ако трябва да определите кой е, вижте определяне на администратор на [фактуриране на акаунт](https://docs.microsoft.com/azure/cost-management-billing/understand/subscription-transfer#whoisaa).</span><span class="sxs-lookup"><span data-stu-id="b7f21-104">If you're not sure if you're and administrator, or if you need to determine who is, see [Determine account billing administrator](https://docs.microsoft.com/azure/cost-management-billing/understand/subscription-transfer#whoisaa).</span></span>

- <span data-ttu-id="b7f21-105">Извършете търсене по **управление на разходите + плащане**.</span><span class="sxs-lookup"><span data-stu-id="b7f21-105">Search on **Cost Management + Billing**.</span></span>
- <span data-ttu-id="b7f21-106">Изберете " **абонаменти** " от левия екран.</span><span class="sxs-lookup"><span data-stu-id="b7f21-106">Select **Subscriptions** from left pane.</span></span> <span data-ttu-id="b7f21-107">В зависимост от достъпа може да се наложи да изберете обхват на фактуриране **и след това абонаменти** или **Azure абонаменти**.</span><span class="sxs-lookup"><span data-stu-id="b7f21-107">Depending on the access, you may need to select a billing scope and then **Subscriptions** or **Azure subscriptions**.</span></span>
- <span data-ttu-id="b7f21-108">Изберете " **прехвърляне на собствеността върху плащането** за абонамента, който искате да прехвърлите"</span><span class="sxs-lookup"><span data-stu-id="b7f21-108">Select **Transfer billing ownership** for the subscription you want to transfer</span></span>
- <span data-ttu-id="b7f21-109">Въведете имейл адреса на потребител, който е администратор на фактуриране на акаунта, който ще бъде новият собственик за абонамента, и след това изберете **Изпращане на искане за прехвърляне**</span><span class="sxs-lookup"><span data-stu-id="b7f21-109">Enter the email address of a user who's a billing administrator of the account that will be the new owner for the subscription and then select **send transfer request**</span></span>
- <span data-ttu-id="b7f21-110">Потребителят получава имейл с инструкции, за да прегледа вашата заявка за прехвърляне.</span><span class="sxs-lookup"><span data-stu-id="b7f21-110">The user gets an email with instructions to review your transfer request.</span></span> <span data-ttu-id="b7f21-111">За да одобри заявката за прехвърляне, потребителят избира връзката в имейла и следва инструкциите.</span><span class="sxs-lookup"><span data-stu-id="b7f21-111">To approve the transfer request, the user selects the link in the email and follows the instructions.</span></span>

<span data-ttu-id="b7f21-112">**Забележка** : Ако прехвърлите собствеността за плащане на абонамента си за акаунт на потребител в друг клиент на Azure ad, всички присвоени задачи за управление на [достъп (RBAC) за ролите](https://docs.microsoft.com/azure/role-based-access-control/overview?WT.mc_id=Portal-Microsoft_Azure_Support), за да управлявате ресурсите в абонамента, се премахват трайно.</span><span class="sxs-lookup"><span data-stu-id="b7f21-112">**Note** : If you transfer billing ownership of your subscription to a user's account in another Azure AD tenant, all [role-based access control (RBAC)](https://docs.microsoft.com/azure/role-based-access-control/overview?WT.mc_id=Portal-Microsoft_Azure_Support)assignments to manage resources in the subscription are permanently removed.</span></span> <span data-ttu-id="b7f21-113">Само новият собственик ще има достъп до управление на ресурсите в абонамента.</span><span class="sxs-lookup"><span data-stu-id="b7f21-113">Only the new owner will have access to manage resources in the subscription.</span></span> <span data-ttu-id="b7f21-114">За повече информация вижте [прехвърляне на абонамент за потребител в друг клиент на AZURE ad](https://docs.microsoft.com/azure/active-directory/managed-identities-azure-resources/known-issues?WT.mc_id=Portal-Microsoft_Azure_Support).</span><span class="sxs-lookup"><span data-stu-id="b7f21-114">For more information, see [Transferring subscription to a user in another Azure AD tenant](https://docs.microsoft.com/azure/active-directory/managed-identities-azure-resources/known-issues?WT.mc_id=Portal-Microsoft_Azure_Support).</span></span>

<span data-ttu-id="b7f21-115">**Препоръчвани документи**</span><span class="sxs-lookup"><span data-stu-id="b7f21-115">**Recommended Documents**</span></span>

- [<span data-ttu-id="b7f21-116">Прехвърляне на собствеността на абонамента за Azure към друг акаунт</span><span class="sxs-lookup"><span data-stu-id="b7f21-116">Transfer billing ownership of an Azure subscription to another account</span></span>](https://docs.microsoft.com/azure/cost-management-billing/manage/billing-subscription-transfer)
- [<span data-ttu-id="b7f21-117">За прехвърляне на собствеността върху плащане за Azure абонамент</span><span class="sxs-lookup"><span data-stu-id="b7f21-117">About transferring billing ownership for an Azure subscription</span></span>](https://docs.microsoft.com//azure/cost-management-billing/understand/subscription-transfer)
- [<span data-ttu-id="b7f21-118">Прехвърляне на Visual Studio, партньорска мрежа на Microsoft (MPN) и плащане като отидете на Dev/Test абонаменти</span><span class="sxs-lookup"><span data-stu-id="b7f21-118">Transferring Visual Studio, Microsoft Partner Network (MPN) and Pay as you go Dev/Test subscriptions</span></span>](https://docs.microsoft.com/azure/billing/billing-subscription-transfer?WT.mc_id=Portal-Microsoft_Azure_Support#transferring-visual-studio-microsoft-partner-network-mpn-and-pay-as-you-go-devtest-subscriptions)
- [<span data-ttu-id="b7f21-119">Често задавани въпроси за собствеността върху прехвърляне</span><span class="sxs-lookup"><span data-stu-id="b7f21-119">Transfer Ownership FAQ</span></span>](https://docs.microsoft.com/azure/billing/billing-subscription-transfer?WT.mc_id=Portal-Microsoft_Azure_Support#frequently-asked-questions-faq-for-senders)
- [<span data-ttu-id="b7f21-120">Отстраняване на проблеми с собствеността при прехвърляне</span><span class="sxs-lookup"><span data-stu-id="b7f21-120">Troubleshoot Transfer ownership issues</span></span>](https://docs.microsoft.com/azure/billing/billing-subscription-transfer?WT.mc_id=Portal-Microsoft_Azure_Support#troubleshooting)
