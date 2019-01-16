---
title: Условен достъп с Intune
ms.author: pebaum
author: pebaum
ms.date: 10/11/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.assetid: aecba7c5-e86d-4ec8-9d44-679f5a3d659d
ms.openlocfilehash: 59f1aefaeec3d655b2388b00e7d58a8c2338504b
ms.sourcegitcommit: d6ea5e9458a2b8ceaab3ac4bd483e1130b9a398a
ms.translationtype: MT
ms.contentlocale: bg-BG
ms.lasthandoff: 01/15/2019
ms.locfileid: "28275628"
---
# <a name="conditional-access-with-intune"></a><span data-ttu-id="fdffa-102">Условен достъп с Intune</span><span class="sxs-lookup"><span data-stu-id="fdffa-102">Conditional Access with Intune</span></span>

<span data-ttu-id="fdffa-103">Използване на **Условен достъп** с Intune изисква три стъпки:</span><span class="sxs-lookup"><span data-stu-id="fdffa-103">Using **Conditional Access** with Intune requires 3 steps:</span></span> 
  
- <span data-ttu-id="fdffa-p101">Създаване на **Условен достъп политика** , която дефинира какви ресурси са защитени, както и какви условия трябва да бъдат изпълнени за достъп до тези ресурси. Например устройството трябва да бъде съвместим преди достъп до корпоративни имейл.</span><span class="sxs-lookup"><span data-stu-id="fdffa-p101">Create a **Conditional Access Policy** that defines what resources are being protected, and what conditions need to be met to access those resources. For example, a device must be compliant before accessing corporate email.</span></span> 
    
- <span data-ttu-id="fdffa-p102">Създаване на **Спазване на политиката** да дефинирате настройки, които трябва да бъдат изпълнени, преди устройството се счита съвместим. Например устройство трябва да има ПИН на най-малко 6 цифри преди се счита съвместим.</span><span class="sxs-lookup"><span data-stu-id="fdffa-p102">Create a **Compliance Policy** to define settings that must be met before the device is considered compliant. For example, a device must have a pin of at least 6 digits before it is considered compliant.</span></span> 
    
- <span data-ttu-id="fdffa-p103">Гарантира **Съответствие политики** и **Условен достъп политики** са насочени към желаните групи от потребители. Това може да наложи създаването на специфични групи от потребители в Azure Active Directory.</span><span class="sxs-lookup"><span data-stu-id="fdffa-p103">Ensuring both **Compliance Policies** and **Conditional Access Policies** are targeted to the desired groups of users. This may require creating specific groups of users in Azure Active Directory.</span></span> 
    
<span data-ttu-id="fdffa-110">Прочетете още:</span><span class="sxs-lookup"><span data-stu-id="fdffa-110">Read more:</span></span>
  
- [<span data-ttu-id="fdffa-111">Условен достъп най-добрите практики</span><span class="sxs-lookup"><span data-stu-id="fdffa-111">Conditional Access best practices</span></span>](https://docs.microsoft.com/en-us/azure/active-directory/conditional-access/best-practices)
    
- [<span data-ttu-id="fdffa-112">Запознаване с условен достъп</span><span class="sxs-lookup"><span data-stu-id="fdffa-112">Getting started with Conditional Access </span></span>](https://docs.microsoft.com/en-us/azure/active-directory/active-directory-conditional-access-azure-portal-get-started)
    

