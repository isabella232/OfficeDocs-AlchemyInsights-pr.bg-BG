---
title: Наблюдение на условния достъп
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "9003769"
- "6702"
ms.openlocfilehash: 0687875a3714067e774872d02630564858d71d1b
ms.sourcegitcommit: 9fd002ce49ad9a7e58c3eb997a8063e2e1feab55
ms.translationtype: MT
ms.contentlocale: bg-BG
ms.lasthandoff: 10/06/2020
ms.locfileid: "48366417"
---
# <a name="monitoring-conditional-access-for-exchange"></a><span data-ttu-id="0117b-102">Наблюдение на условния достъп за Exchange</span><span class="sxs-lookup"><span data-stu-id="0117b-102">Monitoring Conditional Access for Exchange</span></span>

<span data-ttu-id="0117b-103">Потребителите, които са насочени към условен достъп, ще получат имейл за известяване, ако не отговарят на изискванията за достъп на вашата организация.</span><span class="sxs-lookup"><span data-stu-id="0117b-103">Users targeted with conditional access will receive a notification email if they do not meet your organization's access requirements.</span></span> <span data-ttu-id="0117b-104">За да разрешите, ви препоръчваме едно или няколко от следните решения:</span><span class="sxs-lookup"><span data-stu-id="0117b-104">To resolve, we recommend one or more of the following solutions:</span></span>

- <span data-ttu-id="0117b-105">Ако устройството се предполага, че е записано, уведомете потребителя да отиде в приложението Company Portal и да се увери, че той се появява във фирмения портал.</span><span class="sxs-lookup"><span data-stu-id="0117b-105">If the device is presumed to be enrolled, advise the user to go to the Company Portal app and verify that it appears in the Company Portal.</span></span> <span data-ttu-id="0117b-106">Ако не е, потребителят трябва да запише устройството.</span><span class="sxs-lookup"><span data-stu-id="0117b-106">If it doesn't, the user should enroll the device.</span></span>
- <span data-ttu-id="0117b-107">В портала на Azure отидете на настройване на съответствието на > устройства.</span><span class="sxs-lookup"><span data-stu-id="0117b-107">In the Azure portal go to Intune > Device compliance.</span></span> <span data-ttu-id="0117b-108">Под наблюдение щракнете върху съответствие на устройството.</span><span class="sxs-lookup"><span data-stu-id="0117b-108">Under Monitor click Device compliance.</span></span> <span data-ttu-id="0117b-109">Вижте отчета за съответствие на устройството, за да се уверите, че устройството на потребителя е маркирано като съвместимо.</span><span class="sxs-lookup"><span data-stu-id="0117b-109">View your device compliance report to verify that the user's device is marked as compliant.</span></span>
- <span data-ttu-id="0117b-110">В портала на Azure отидете на настройване на съответствието на > устройства.</span><span class="sxs-lookup"><span data-stu-id="0117b-110">In the Azure portal go to Intune > Device compliance.</span></span> <span data-ttu-id="0117b-111">Под управление щракнете върху правила.</span><span class="sxs-lookup"><span data-stu-id="0117b-111">Under Manage, click Policies.</span></span> <span data-ttu-id="0117b-112">В списъка с правила за съответствие Проверете дали даден профил е присвоен на устройството на потребителя.</span><span class="sxs-lookup"><span data-stu-id="0117b-112">In the list of compliance policies, verify that a profile is assigned to your user's device.</span></span> <span data-ttu-id="0117b-113">Ако не е присвоен профил, в противен случай няма да може да се потвърди състоянието на съответствие на устройството.</span><span class="sxs-lookup"><span data-stu-id="0117b-113">If no profile is assigned, then Intune will not be able to confirm the device's compliance status.</span></span>
- <span data-ttu-id="0117b-114">Редактирайте възложената задача за условен достъп на потребителя.</span><span class="sxs-lookup"><span data-stu-id="0117b-114">Edit the user's conditional access assignment.</span></span>

1. <span data-ttu-id="0117b-115">В портала на Azure отидете на **Настройване**на правилата за  >  **условен достъп**  >  **Policies**.</span><span class="sxs-lookup"><span data-stu-id="0117b-115">In the Azure portal go to **Intune** > **Conditional access** > **Policies**.</span></span>
2. <span data-ttu-id="0117b-116">Изберете правило от списъка.</span><span class="sxs-lookup"><span data-stu-id="0117b-116">Select a policy from the list.</span></span>
3. <span data-ttu-id="0117b-117">Щракнете върху потребители и групи.</span><span class="sxs-lookup"><span data-stu-id="0117b-117">Click Users and groups.</span></span>
4. <span data-ttu-id="0117b-118">За да насочвате определени правила към някого, добавете ги към списъка включване.</span><span class="sxs-lookup"><span data-stu-id="0117b-118">To target a certain policy at someone, add them to the Include list.</span></span> <span data-ttu-id="0117b-119">За да се гарантира, че даден човек е пропуснат от правилата, добавете ги към списъка за изключване.</span><span class="sxs-lookup"><span data-stu-id="0117b-119">To ensure that a person is omitted from the policy, add them to the Exclude list.</span></span>

<span data-ttu-id="0117b-120">Полезни връзки:</span><span class="sxs-lookup"><span data-stu-id="0117b-120">Helpful links:</span></span>

[<span data-ttu-id="0117b-121">Общ преглед на съответствието на устройството</span><span class="sxs-lookup"><span data-stu-id="0117b-121">Device compliance overview</span></span>](https://docs.microsoft.com/intune/device-compliance-get-started)

[<span data-ttu-id="0117b-122">Отстраняване на неизправности при CA</span><span class="sxs-lookup"><span data-stu-id="0117b-122">Troubleshooting CA</span></span>](https://docs.microsoft.com/intune/troubleshoot-conditional-access)

[<span data-ttu-id="0117b-123">Правила за отстраняване на неизправности</span><span class="sxs-lookup"><span data-stu-id="0117b-123">Troubleshooting policy</span></span>](https://docs.microsoft.com/intune/troubleshoot-policies-in-microsoft-intune)

[<span data-ttu-id="0117b-124">Следене на съответствието на устройството</span><span class="sxs-lookup"><span data-stu-id="0117b-124">Monitoring Intune device compliance</span></span>](https://docs.microsoft.com/intune/compliance-policy-monitor)

<span data-ttu-id="0117b-125">Забележка: тези стъпки са полезни само при отстраняване на неизправности с функцията за условен достъп на Azure Active Directory.</span><span class="sxs-lookup"><span data-stu-id="0117b-125">Note: these steps are only helpful in troubleshooting the Azure Active Directory feature Conditional Access.</span></span> <span data-ttu-id="0117b-126">Възможно е също така да поставите под карантина устройството блокирането на имейл достъпа чрез правилата за Exchange.</span><span class="sxs-lookup"><span data-stu-id="0117b-126">It is also possible to quarantine a device blocking it's email access with Exchange policy.</span></span> <span data-ttu-id="0117b-127">Повече информация за управлението на устройства на Exchange можете да намерите [тук](<https://docs.microsoft.com/previous-versions/office/exchange-server-2010/ff959225(v=exchg.141>).</span><span class="sxs-lookup"><span data-stu-id="0117b-127">More information on Exchange device management can be found [here](<https://docs.microsoft.com/previous-versions/office/exchange-server-2010/ff959225(v=exchg.141>).</span></span>
