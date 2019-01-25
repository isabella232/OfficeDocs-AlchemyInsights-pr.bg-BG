---
title: Мониторинг на условен достъп
ms.author: pebaum
author: pebaum
ms.date: 8/1/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.assetid: dcb86c54-769e-4832-9f88-bc45f1e5f36c
ms.openlocfilehash: 06307b57475e8828e6d4e5e01625d5100576f12b
ms.sourcegitcommit: e2864efcfb493b6e46b662b746661a61232bdba7
ms.translationtype: MT
ms.contentlocale: bg-BG
ms.lasthandoff: 01/24/2019
ms.locfileid: "29457789"
---
# <a name="monitoring-conditional-access"></a><span data-ttu-id="4be3e-102">Мониторинг на условен достъп</span><span class="sxs-lookup"><span data-stu-id="4be3e-102">Monitoring Conditional Access</span></span>

<span data-ttu-id="4be3e-p101">Потребителите, насочени с условен достъп ще получите известие по имейл, ако те не отговарят на изискванията за достъп на вашата организация. За да разрешите, ние препоръчваме един или повече от следните решения:</span><span class="sxs-lookup"><span data-stu-id="4be3e-p101">Users targeted with conditional access will receive a notification email if they do not meet your organization's access requirements. To resolve, we recommend one or more of the following solutions:</span></span>
  
- <span data-ttu-id="4be3e-p102">Ако устройството се предполага да бъдат записани, съветва потребителят да отидете на компанията портал ап и проверете дали тя се появява в портала на компанията. Ако това не стане, потребителят трябва да се запишат устройството.</span><span class="sxs-lookup"><span data-stu-id="4be3e-p102">If the device is presumed to be enrolled, advise the user to go to the Company Portal app and verify that it appears in the Company Portal. If it doesn't, the user should enroll the device.</span></span>
    
- <span data-ttu-id="4be3e-p103">В портала на лазурното отидете на **Intune \> устройство съответствие**. Под **монитор** щракнете върху **устройство за съответствие**. Преглед на доклад за съответствие вашето устройство да се провери, че устройството на потребителя е маркиран като съответстваща.</span><span class="sxs-lookup"><span data-stu-id="4be3e-p103">In the Azure portal go to **Intune \> Device compliance**. Under **Monitor** click **Device compliance**. View your device compliance report to verify that the user's device is marked as compliant.</span></span> 
    
- <span data-ttu-id="4be3e-p104">В портала на лазурното отидете на **Intune \> устройство съответствие**. Под **управление**щракнете върху **правила**. В списъка на правилата за съответствие Проверете, че профил е зададен на устройството ви потребителя. Ако няма профил е присвоен, тогава Intune не ще бъде в състояние да потвърди съответствието състоянието на устройството.</span><span class="sxs-lookup"><span data-stu-id="4be3e-p104">In the Azure portal go to **Intune \> Device compliance**. Under **Manage**, click **Policies**. In the list of compliance policies, verify that a profile is assigned to your user's device. If no profile is assigned, then Intune will not be able to confirm the device's compliance status.</span></span> 
    
- <span data-ttu-id="4be3e-114">Редактиране на потребителя условен достъп задача.</span><span class="sxs-lookup"><span data-stu-id="4be3e-114">Edit the user's conditional access assignment.</span></span>
    
1. <span data-ttu-id="4be3e-115">В портала на лазурното отидете на **Intune \> условен достъп \> политика**</span><span class="sxs-lookup"><span data-stu-id="4be3e-115">In the Azure portal go to **Intune \> Conditional access \> Policies**</span></span>
    
2. <span data-ttu-id="4be3e-116">Изберете правило от списъка</span><span class="sxs-lookup"><span data-stu-id="4be3e-116">Select a policy from the list</span></span>
    
3. <span data-ttu-id="4be3e-117">Щракнете върху **потребители и групи**</span><span class="sxs-lookup"><span data-stu-id="4be3e-117">Click **Users and groups**</span></span>
    
4. <span data-ttu-id="4be3e-p105">Да се насочите някои политика на някого, трябва да ги добавите към списъка за **включване** . Да гарантира, че дадено лице е пропуснато от политиката, ги добавите към списъка за **изключване** .</span><span class="sxs-lookup"><span data-stu-id="4be3e-p105">To target a certain policy at someone, add them to the **Include** list. To ensure that a person is omitted from the policy, add them to the **Exclude** list.</span></span> 
    
<span data-ttu-id="4be3e-120">Прочетете още: [как да монитор условен достъп устройства](https://docs.microsoft.com/en-us/intune/conditional-access-exchange-monitor)</span><span class="sxs-lookup"><span data-stu-id="4be3e-120">Read more: [How to Monitor Conditional Access devices](https://docs.microsoft.com/en-us/intune/conditional-access-exchange-monitor)</span></span>
  

