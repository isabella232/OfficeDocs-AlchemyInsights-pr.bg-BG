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
ms.openlocfilehash: c3bf5dd9066685af2df7ba50f0eb3ba6e891c2a9
ms.sourcegitcommit: 0eb4f9bde53395b5fd4b5cd4ffc56ca96db91298
ms.translationtype: MT
ms.contentlocale: bg-BG
ms.lasthandoff: 03/10/2021
ms.locfileid: "50708663"
---
# <a name="monitoring-conditional-access-for-exchange"></a><span data-ttu-id="8750a-102">Наблюдение на условния достъп за Exchange</span><span class="sxs-lookup"><span data-stu-id="8750a-102">Monitoring Conditional Access for Exchange</span></span>

<span data-ttu-id="8750a-103">Потребителите, които са насочени към условен достъп, ще получат имейл за известяване, ако не отговарят на изискванията за достъп на вашата организация.</span><span class="sxs-lookup"><span data-stu-id="8750a-103">Users targeted with conditional access will receive a notification email if they do not meet your organization's access requirements.</span></span> <span data-ttu-id="8750a-104">За да разрешите, ви препоръчваме едно или няколко от следните решения:</span><span class="sxs-lookup"><span data-stu-id="8750a-104">To resolve, we recommend one or more of the following solutions:</span></span>

- <span data-ttu-id="8750a-105">Ако устройството се предполага, че е записано, уведомете потребителя да отиде в приложението Company Portal и да се увери, че той се появява във фирмения портал.</span><span class="sxs-lookup"><span data-stu-id="8750a-105">If the device is presumed to be enrolled, advise the user to go to the Company Portal app and verify that it appears in the Company Portal.</span></span> <span data-ttu-id="8750a-106">Ако не е, потребителят трябва да запише устройството.</span><span class="sxs-lookup"><span data-stu-id="8750a-106">If it doesn't, the user should enroll the device.</span></span>
- <span data-ttu-id="8750a-107">В портала на Azure отидете на настройване на съответствието на > устройства.</span><span class="sxs-lookup"><span data-stu-id="8750a-107">In the Azure portal go to Intune > Device compliance.</span></span> <span data-ttu-id="8750a-108">Под наблюдение щракнете върху съответствие на устройството.</span><span class="sxs-lookup"><span data-stu-id="8750a-108">Under Monitor click Device compliance.</span></span> <span data-ttu-id="8750a-109">Вижте отчета за съответствие на устройството, за да се уверите, че устройството на потребителя е маркирано като съвместимо.</span><span class="sxs-lookup"><span data-stu-id="8750a-109">View your device compliance report to verify that the user's device is marked as compliant.</span></span>
- <span data-ttu-id="8750a-110">В портала на Azure отидете на настройване на съответствието на > устройства.</span><span class="sxs-lookup"><span data-stu-id="8750a-110">In the Azure portal go to Intune > Device compliance.</span></span> <span data-ttu-id="8750a-111">Под управление щракнете върху правила.</span><span class="sxs-lookup"><span data-stu-id="8750a-111">Under Manage, click Policies.</span></span> <span data-ttu-id="8750a-112">В списъка с правила за съответствие Проверете дали даден профил е присвоен на устройството на потребителя.</span><span class="sxs-lookup"><span data-stu-id="8750a-112">In the list of compliance policies, verify that a profile is assigned to your user's device.</span></span> <span data-ttu-id="8750a-113">Ако не е присвоен профил, в противен случай няма да може да се потвърди състоянието на съответствие на устройството.</span><span class="sxs-lookup"><span data-stu-id="8750a-113">If no profile is assigned, then Intune will not be able to confirm the device's compliance status.</span></span>
- <span data-ttu-id="8750a-114">Редактирайте възложената задача за условен достъп на потребителя.</span><span class="sxs-lookup"><span data-stu-id="8750a-114">Edit the user's conditional access assignment.</span></span>

1. <span data-ttu-id="8750a-115">В портала на Azure отидете на **Настройване** на правилата за  >  **условен достъп**  >  .</span><span class="sxs-lookup"><span data-stu-id="8750a-115">In the Azure portal go to **Intune** > **Conditional access** > **Policies**.</span></span>
2. <span data-ttu-id="8750a-116">Изберете правило от списъка.</span><span class="sxs-lookup"><span data-stu-id="8750a-116">Select a policy from the list.</span></span>
3. <span data-ttu-id="8750a-117">Щракнете върху потребители и групи.</span><span class="sxs-lookup"><span data-stu-id="8750a-117">Click Users and groups.</span></span>
4. <span data-ttu-id="8750a-118">За да насочвате определени правила към някого, добавете ги към списъка включване.</span><span class="sxs-lookup"><span data-stu-id="8750a-118">To target a certain policy at someone, add them to the Include list.</span></span> <span data-ttu-id="8750a-119">За да се гарантира, че даден човек е пропуснат от правилата, добавете ги към списъка за изключване.</span><span class="sxs-lookup"><span data-stu-id="8750a-119">To ensure that a person is omitted from the policy, add them to the Exclude list.</span></span>

<span data-ttu-id="8750a-120">Полезни връзки:</span><span class="sxs-lookup"><span data-stu-id="8750a-120">Helpful links:</span></span>

[<span data-ttu-id="8750a-121">Общ преглед на съответствието на устройството</span><span class="sxs-lookup"><span data-stu-id="8750a-121">Device compliance overview</span></span>](https://docs.microsoft.com/intune/device-compliance-get-started)

[<span data-ttu-id="8750a-122">Отстраняване на неизправности при CA</span><span class="sxs-lookup"><span data-stu-id="8750a-122">Troubleshooting CA</span></span>](https://docs.microsoft.com/intune/troubleshoot-conditional-access)

[<span data-ttu-id="8750a-123">Правила за отстраняване на неизправности</span><span class="sxs-lookup"><span data-stu-id="8750a-123">Troubleshooting policy</span></span>](https://docs.microsoft.com/troubleshoot/mem/intune/troubleshoot-policies-in-microsoft-intune)

[<span data-ttu-id="8750a-124">Следене на съответствието на устройството</span><span class="sxs-lookup"><span data-stu-id="8750a-124">Monitoring Intune device compliance</span></span>](https://docs.microsoft.com/intune/compliance-policy-monitor)

<span data-ttu-id="8750a-125">Забележка: тези стъпки са полезни само при отстраняване на неизправности с функцията за условен достъп на Azure Active Directory.</span><span class="sxs-lookup"><span data-stu-id="8750a-125">Note: these steps are only helpful in troubleshooting the Azure Active Directory feature Conditional Access.</span></span> <span data-ttu-id="8750a-126">Възможно е също така да поставите под карантина устройството блокирането на имейл достъпа чрез правилата за Exchange.</span><span class="sxs-lookup"><span data-stu-id="8750a-126">It is also possible to quarantine a device blocking it's email access with Exchange policy.</span></span> <span data-ttu-id="8750a-127">Повече информация за управлението на устройства на Exchange може да бъде намерена [тук] ( https://docs.microsoft.com/previous-versions/office/exchange-server-2010/ff959225(v=exchg.141) .</span><span class="sxs-lookup"><span data-stu-id="8750a-127">More information on Exchange device management can be found [here](https://docs.microsoft.com/previous-versions/office/exchange-server-2010/ff959225(v=exchg.141).</span></span>
