---
title: Мониторинг на условен достъп
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: dcb86c54-769e-4832-9f88-bc45f1e5f36c
ms.openlocfilehash: 8b76d58791408037b5704b421d7afa166e3ea0be
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: bg-BG
ms.lasthandoff: 04/22/2020
ms.locfileid: "43713707"
---
# <a name="monitoring-conditional-access-for-exchange"></a><span data-ttu-id="4128d-102">Мониторинг на условен достъп за обмен</span><span class="sxs-lookup"><span data-stu-id="4128d-102">Monitoring Conditional Access for Exchange</span></span>

<span data-ttu-id="4128d-103">Потребителите, към които е насочен условен достъп, ще получат имейл с известие, ако не отговарят на изискванията за достъп на вашата организация.</span><span class="sxs-lookup"><span data-stu-id="4128d-103">Users targeted with conditional access will receive a notification email if they do not meet your organization's access requirements.</span></span> <span data-ttu-id="4128d-104">За да разрешите проблема, препоръчваме едно или повече от следните решения:</span><span class="sxs-lookup"><span data-stu-id="4128d-104">To resolve, we recommend one or more of the following solutions:</span></span>
  
- <span data-ttu-id="4128d-105">Ако устройството се предполага, че се записва, посъветвапотребителя да отидете на приложението "Портал на компанията" и се уверете, че той се появява в портала на компанията.</span><span class="sxs-lookup"><span data-stu-id="4128d-105">If the device is presumed to be enrolled, advise the user to go to the Company Portal app and verify that it appears in the Company Portal.</span></span> <span data-ttu-id="4128d-106">Ако не, потребителят трябва да запишете устройството.</span><span class="sxs-lookup"><span data-stu-id="4128d-106">If it doesn't, the user should enroll the device.</span></span>
    
- <span data-ttu-id="4128d-107">В портала на Azure отидете на **Intune \> устройство съответствие .**</span><span class="sxs-lookup"><span data-stu-id="4128d-107">In the Azure portal go to **Intune \> Device compliance**.</span></span> <span data-ttu-id="4128d-108">Под **Монитор** щракнете върху **съответствие то на устройството**.</span><span class="sxs-lookup"><span data-stu-id="4128d-108">Under **Monitor** click **Device compliance**.</span></span> <span data-ttu-id="4128d-109">Прегледайте отчета за съответствие то на устройството, за да се уверите, че устройството на потребителя е означено като съвместимо.</span><span class="sxs-lookup"><span data-stu-id="4128d-109">View your device compliance report to verify that the user's device is marked as compliant.</span></span> 
    
- <span data-ttu-id="4128d-110">В портала на Azure отидете на **Intune \> устройство съответствие .**</span><span class="sxs-lookup"><span data-stu-id="4128d-110">In the Azure portal go to **Intune \> Device compliance**.</span></span> <span data-ttu-id="4128d-111">Под **Управление**щракнете върху **Правила**.</span><span class="sxs-lookup"><span data-stu-id="4128d-111">Under **Manage**, click **Policies**.</span></span> <span data-ttu-id="4128d-112">В списъка с правила за съответствие проверете дали даден профил е присвоен на устройството на потребителя.</span><span class="sxs-lookup"><span data-stu-id="4128d-112">In the list of compliance policies, verify that a profile is assigned to your user's device.</span></span> <span data-ttu-id="4128d-113">Ако не е присвоен профил, Intune няма да може да потвърди състоянието на съответствие на устройството.</span><span class="sxs-lookup"><span data-stu-id="4128d-113">If no profile is assigned, then Intune will not be able to confirm the device's compliance status.</span></span> 
    
- <span data-ttu-id="4128d-114">Редактиране на задаване на условен достъп на потребителя.</span><span class="sxs-lookup"><span data-stu-id="4128d-114">Edit the user's conditional access assignment.</span></span>
    
1. <span data-ttu-id="4128d-115">В портала на Azure отидете **на Intune \> условен достъп \> правила**</span><span class="sxs-lookup"><span data-stu-id="4128d-115">In the Azure portal go to **Intune \> Conditional access \> Policies**</span></span>
    
2. <span data-ttu-id="4128d-116">Изберете правила от списъка</span><span class="sxs-lookup"><span data-stu-id="4128d-116">Select a policy from the list</span></span>
    
3. <span data-ttu-id="4128d-117">Кликнете върху **Потребители и групи**</span><span class="sxs-lookup"><span data-stu-id="4128d-117">Click **Users and groups**</span></span>
    
4. <span data-ttu-id="4128d-118">За да насочвате към определени правила към някого, добавете ги към списъка **"Включване".**</span><span class="sxs-lookup"><span data-stu-id="4128d-118">To target a certain policy at someone, add them to the **Include** list.</span></span> <span data-ttu-id="4128d-119">За да сте сигурни, че дадено лице е пропуснато от правилата, добавете го към списъка **"Изключване".**</span><span class="sxs-lookup"><span data-stu-id="4128d-119">To ensure that a person is omitted from the policy, add them to the **Exclude** list.</span></span> 
    
<span data-ttu-id="4128d-120">Прочетете повече: [Как да наблюдавате устройствата с условен достъп](https://docs.microsoft.com/intune/conditional-access-exchange-monitor)</span><span class="sxs-lookup"><span data-stu-id="4128d-120">Read more: [How to Monitor Conditional Access devices](https://docs.microsoft.com/intune/conditional-access-exchange-monitor)</span></span>
  

