---
title: Мониторинг на условен достъп
ms.author: pebaum
author: pebaum
ms.date: 8/1/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: dcb86c54-769e-4832-9f88-bc45f1e5f36c
ms.openlocfilehash: 374814f4eabd61433a15876ebf7f351819933c21
ms.sourcegitcommit: 1d98db8acb9959aba3b5e308a567ade6b62da56c
ms.translationtype: MT
ms.contentlocale: bg-BG
ms.lasthandoff: 08/22/2019
ms.locfileid: "36538730"
---
# <a name="monitoring-conditional-access-for-exchange"></a><span data-ttu-id="ab640-102">Мониторинг на условен достъп за обмен</span><span class="sxs-lookup"><span data-stu-id="ab640-102">Monitoring Conditional Access for Exchange</span></span>

<span data-ttu-id="ab640-103">Потребителите, насочени с условен достъп ще получите известие по имейл, ако те не отговарят на изискванията за достъп на вашата организация.</span><span class="sxs-lookup"><span data-stu-id="ab640-103">Users targeted with conditional access will receive a notification email if they do not meet your organization's access requirements.</span></span> <span data-ttu-id="ab640-104">За да разрешите, ние препоръчваме един или повече от следните решения:</span><span class="sxs-lookup"><span data-stu-id="ab640-104">To resolve, we recommend one or more of the following solutions:</span></span>
  
- <span data-ttu-id="ab640-105">Ако устройството се предполага да бъдат записани, съветва потребителят да отидете на компанията портал ап и проверете дали тя се появява в портала на компанията.</span><span class="sxs-lookup"><span data-stu-id="ab640-105">If the device is presumed to be enrolled, advise the user to go to the Company Portal app and verify that it appears in the Company Portal.</span></span> <span data-ttu-id="ab640-106">Ако това не стане, потребителят трябва да се запишат устройството.</span><span class="sxs-lookup"><span data-stu-id="ab640-106">If it doesn't, the user should enroll the device.</span></span>
    
- <span data-ttu-id="ab640-107">В портала на лазурното отидете на **Intune \> устройство съответствие**.</span><span class="sxs-lookup"><span data-stu-id="ab640-107">In the Azure portal go to **Intune \> Device compliance**.</span></span> <span data-ttu-id="ab640-108">Под **монитор** щракнете върху **устройство за съответствие**.</span><span class="sxs-lookup"><span data-stu-id="ab640-108">Under **Monitor** click **Device compliance**.</span></span> <span data-ttu-id="ab640-109">Преглед на доклад за съответствие вашето устройство да се провери, че устройството на потребителя е маркиран като съответстваща.</span><span class="sxs-lookup"><span data-stu-id="ab640-109">View your device compliance report to verify that the user's device is marked as compliant.</span></span> 
    
- <span data-ttu-id="ab640-110">В портала на лазурното отидете на **Intune \> устройство съответствие**.</span><span class="sxs-lookup"><span data-stu-id="ab640-110">In the Azure portal go to **Intune \> Device compliance**.</span></span> <span data-ttu-id="ab640-111">Под **управление**щракнете върху **правила**.</span><span class="sxs-lookup"><span data-stu-id="ab640-111">Under **Manage**, click **Policies**.</span></span> <span data-ttu-id="ab640-112">В списъка на правилата за съответствие Проверете, че профил е зададен на устройството ви потребителя.</span><span class="sxs-lookup"><span data-stu-id="ab640-112">In the list of compliance policies, verify that a profile is assigned to your user's device.</span></span> <span data-ttu-id="ab640-113">Ако няма профил е присвоен, тогава Intune не ще бъде в състояние да потвърди съответствието състоянието на устройството.</span><span class="sxs-lookup"><span data-stu-id="ab640-113">If no profile is assigned, then Intune will not be able to confirm the device's compliance status.</span></span> 
    
- <span data-ttu-id="ab640-114">Редактиране на потребителя условен достъп задача.</span><span class="sxs-lookup"><span data-stu-id="ab640-114">Edit the user's conditional access assignment.</span></span>
    
1. <span data-ttu-id="ab640-115">В портала на лазурното отидете на **Intune \> условен достъп \> политика**</span><span class="sxs-lookup"><span data-stu-id="ab640-115">In the Azure portal go to **Intune \> Conditional access \> Policies**</span></span>
    
2. <span data-ttu-id="ab640-116">Изберете правило от списъка</span><span class="sxs-lookup"><span data-stu-id="ab640-116">Select a policy from the list</span></span>
    
3. <span data-ttu-id="ab640-117">Щракнете върху **потребители и групи**</span><span class="sxs-lookup"><span data-stu-id="ab640-117">Click **Users and groups**</span></span>
    
4. <span data-ttu-id="ab640-118">Да се насочите някои политика на някого, трябва да ги добавите към списъка за **включване** .</span><span class="sxs-lookup"><span data-stu-id="ab640-118">To target a certain policy at someone, add them to the **Include** list.</span></span> <span data-ttu-id="ab640-119">Да гарантира, че дадено лице е пропуснато от политиката, ги добавите към списъка за **изключване** .</span><span class="sxs-lookup"><span data-stu-id="ab640-119">To ensure that a person is omitted from the policy, add them to the **Exclude** list.</span></span> 
    
<span data-ttu-id="ab640-120">Прочетете още: [как да монитор условен достъп устройства](https://docs.microsoft.com/intune/conditional-access-exchange-monitor)</span><span class="sxs-lookup"><span data-stu-id="ab640-120">Read more: [How to Monitor Conditional Access devices](https://docs.microsoft.com/intune/conditional-access-exchange-monitor)</span></span>
  

