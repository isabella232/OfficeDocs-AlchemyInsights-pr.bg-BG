---
title: Условен достъп с InTune
ms.author: pebaum
author: pebaum
ms.date: 10/11/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: aecba7c5-e86d-4ec8-9d44-679f5a3d659d
ms.openlocfilehash: e147e7460ee6a786e577a43c0b8355fc27ee367b
ms.sourcegitcommit: 0b06093dabd685f76cc39b1d7c0f8b03883b6e79
ms.translationtype: MT
ms.contentlocale: bg-BG
ms.lasthandoff: 10/25/2019
ms.locfileid: "36504983"
---
# <a name="conditional-access-with-intune"></a><span data-ttu-id="b113c-102">Условен достъп с InTune</span><span class="sxs-lookup"><span data-stu-id="b113c-102">Conditional Access with Intune</span></span>

<span data-ttu-id="b113c-103">Използването на **условен достъп** с InTune изисква 3 стъпки:</span><span class="sxs-lookup"><span data-stu-id="b113c-103">Using **Conditional Access** with Intune requires 3 steps:</span></span> 
  
- <span data-ttu-id="b113c-104">Създаване на **правила за условен достъп** , която определя какви ресурси са защитени и какви условия трябва да бъдат изпълнени за достъп до тези ресурси.</span><span class="sxs-lookup"><span data-stu-id="b113c-104">Create a **Conditional Access Policy** that defines what resources are being protected, and what conditions need to be met to access those resources.</span></span> <span data-ttu-id="b113c-105">Например дадено устройство трябва да отговаря на изискванията, преди да получи достъп до корпоративен имейл.</span><span class="sxs-lookup"><span data-stu-id="b113c-105">For example, a device must be compliant before accessing corporate email.</span></span> 
    
- <span data-ttu-id="b113c-106">Създаване на **правила за съответствие** , за да дефинирате настройки, които трябва да бъдат изпълнени, преди устройството да се счита за съвместимо.</span><span class="sxs-lookup"><span data-stu-id="b113c-106">Create a **Compliance Policy** to define settings that must be met before the device is considered compliant.</span></span> <span data-ttu-id="b113c-107">Например устройството трябва да има щифт от поне 6 цифри, преди да се счита за съвместим.</span><span class="sxs-lookup"><span data-stu-id="b113c-107">For example, a device must have a pin of at least 6 digits before it is considered compliant.</span></span> 
    
- <span data-ttu-id="b113c-108">Осигуряването на **политики за съответствие** и **правила за условен достъп** са насочени към желаните групи потребители.</span><span class="sxs-lookup"><span data-stu-id="b113c-108">Ensuring both **Compliance Policies** and **Conditional Access Policies** are targeted to the desired groups of users.</span></span> <span data-ttu-id="b113c-109">Това може да изисква създаване на конкретни групи от потребители в Azure Active Directory.</span><span class="sxs-lookup"><span data-stu-id="b113c-109">This may require creating specific groups of users in Azure Active Directory.</span></span> 
    
<span data-ttu-id="b113c-110">Прочети още:</span><span class="sxs-lookup"><span data-stu-id="b113c-110">Read more:</span></span>
  
- [<span data-ttu-id="b113c-111">Най-добри практики за условен достъп</span><span class="sxs-lookup"><span data-stu-id="b113c-111">Conditional Access best practices</span></span>](https://docs.microsoft.com/azure/active-directory/conditional-access/best-practices)
    
- [<span data-ttu-id="b113c-112">Първи стъпки с условен достъп</span><span class="sxs-lookup"><span data-stu-id="b113c-112">Getting started with Conditional Access </span></span>](https://docs.microsoft.com/azure/active-directory/active-directory-conditional-access-azure-portal-get-started)
    

