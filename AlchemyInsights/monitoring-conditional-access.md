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
ms.assetid: dcb86c54-769e-4832-9f88-bc45f1e5f36c
ms.openlocfilehash: 6083fc427e3791fdb0907198b525337a0c987c4e
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: bg-BG
ms.lasthandoff: 09/14/2020
ms.locfileid: "47702892"
---
# <a name="monitoring-conditional-access-for-exchange"></a><span data-ttu-id="3d3e6-102">Наблюдение на условния достъп за Exchange</span><span class="sxs-lookup"><span data-stu-id="3d3e6-102">Monitoring Conditional Access for Exchange</span></span>

<span data-ttu-id="3d3e6-103">Потребителите, които са насочени към условен достъп, ще получат имейл за известяване, ако не отговарят на изискванията за достъп на вашата организация.</span><span class="sxs-lookup"><span data-stu-id="3d3e6-103">Users targeted with conditional access will receive a notification email if they do not meet your organization's access requirements.</span></span> <span data-ttu-id="3d3e6-104">За да разрешите, ви препоръчваме едно или няколко от следните решения:</span><span class="sxs-lookup"><span data-stu-id="3d3e6-104">To resolve, we recommend one or more of the following solutions:</span></span>
  
- <span data-ttu-id="3d3e6-105">Ако устройството се предполага, че е записано, уведомете потребителя да отиде в приложението Company Portal и да се увери, че той се появява във фирмения портал.</span><span class="sxs-lookup"><span data-stu-id="3d3e6-105">If the device is presumed to be enrolled, advise the user to go to the Company Portal app and verify that it appears in the Company Portal.</span></span> <span data-ttu-id="3d3e6-106">Ако не е, потребителят трябва да запише устройството.</span><span class="sxs-lookup"><span data-stu-id="3d3e6-106">If it doesn't, the user should enroll the device.</span></span>
    
- <span data-ttu-id="3d3e6-107">В портала на Azure отидете на **Настройки за \> съответствие на устройството**.</span><span class="sxs-lookup"><span data-stu-id="3d3e6-107">In the Azure portal go to **Intune \> Device compliance**.</span></span> <span data-ttu-id="3d3e6-108">Под **наблюдение** щракнете върху **съответствие на устройството**.</span><span class="sxs-lookup"><span data-stu-id="3d3e6-108">Under **Monitor** click **Device compliance**.</span></span> <span data-ttu-id="3d3e6-109">Вижте отчета за съответствие на устройството, за да се уверите, че устройството на потребителя е маркирано като съвместимо.</span><span class="sxs-lookup"><span data-stu-id="3d3e6-109">View your device compliance report to verify that the user's device is marked as compliant.</span></span> 
    
- <span data-ttu-id="3d3e6-110">В портала на Azure отидете на **Настройки за \> съответствие на устройството**.</span><span class="sxs-lookup"><span data-stu-id="3d3e6-110">In the Azure portal go to **Intune \> Device compliance**.</span></span> <span data-ttu-id="3d3e6-111">Под **управление**щракнете върху **правила**.</span><span class="sxs-lookup"><span data-stu-id="3d3e6-111">Under **Manage**, click **Policies**.</span></span> <span data-ttu-id="3d3e6-112">В списъка с правила за съответствие Проверете дали даден профил е присвоен на устройството на потребителя.</span><span class="sxs-lookup"><span data-stu-id="3d3e6-112">In the list of compliance policies, verify that a profile is assigned to your user's device.</span></span> <span data-ttu-id="3d3e6-113">Ако не е присвоен профил, в противен случай няма да може да се потвърди състоянието на съответствие на устройството.</span><span class="sxs-lookup"><span data-stu-id="3d3e6-113">If no profile is assigned, then Intune will not be able to confirm the device's compliance status.</span></span> 
    
- <span data-ttu-id="3d3e6-114">Редактирайте възложената задача за условен достъп на потребителя.</span><span class="sxs-lookup"><span data-stu-id="3d3e6-114">Edit the user's conditional access assignment.</span></span>
    
1. <span data-ttu-id="3d3e6-115">В портала на Azure отидете на **Настройване на \> \> правилата за условен достъп**</span><span class="sxs-lookup"><span data-stu-id="3d3e6-115">In the Azure portal go to **Intune \> Conditional access \> Policies**</span></span>
    
2. <span data-ttu-id="3d3e6-116">Изберете правило от списъка</span><span class="sxs-lookup"><span data-stu-id="3d3e6-116">Select a policy from the list</span></span>
    
3. <span data-ttu-id="3d3e6-117">Щракнете върху **потребители и групи**</span><span class="sxs-lookup"><span data-stu-id="3d3e6-117">Click **Users and groups**</span></span>
    
4. <span data-ttu-id="3d3e6-118">За да насочвате определени правила към някого, добавете ги към списъка **включване** .</span><span class="sxs-lookup"><span data-stu-id="3d3e6-118">To target a certain policy at someone, add them to the **Include** list.</span></span> <span data-ttu-id="3d3e6-119">За да се гарантира, че даден човек е пропуснат от правилата, добавете ги към списъка за **изключване** .</span><span class="sxs-lookup"><span data-stu-id="3d3e6-119">To ensure that a person is omitted from the policy, add them to the **Exclude** list.</span></span> 
    
<span data-ttu-id="3d3e6-120">Прочетете още: [как да следите устройства за условен достъп](https://docs.microsoft.com/intune/conditional-access-exchange-monitor)</span><span class="sxs-lookup"><span data-stu-id="3d3e6-120">Read more: [How to Monitor Conditional Access devices](https://docs.microsoft.com/intune/conditional-access-exchange-monitor)</span></span>
  

