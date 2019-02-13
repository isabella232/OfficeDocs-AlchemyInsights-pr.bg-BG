---
title: Условен достъп с Intune
ms.author: pebaum
author: pebaum
ms.date: 10/11/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: aecba7c5-e86d-4ec8-9d44-679f5a3d659d
ms.openlocfilehash: 2e778bf4fbdb766700fb24b3405b4ddce89253f7
ms.sourcegitcommit: dd43cc0a9470f98b8ef2a3787c823801d674c666
ms.translationtype: MT
ms.contentlocale: bg-BG
ms.lasthandoff: 02/12/2019
ms.locfileid: "29935917"
---
# <a name="conditional-access-with-intune"></a><span data-ttu-id="6135a-102">Условен достъп с Intune</span><span class="sxs-lookup"><span data-stu-id="6135a-102">Conditional Access with Intune</span></span>

<span data-ttu-id="6135a-103">Използване на **Условен достъп** с Intune изисква три стъпки:</span><span class="sxs-lookup"><span data-stu-id="6135a-103">Using **Conditional Access** with Intune requires 3 steps:</span></span> 
  
- <span data-ttu-id="6135a-p101">Създаване на **Условен достъп политика** , която дефинира какви ресурси са защитени, както и какви условия трябва да бъдат изпълнени за достъп до тези ресурси. Например устройството трябва да бъде съвместим преди достъп до корпоративни имейл.</span><span class="sxs-lookup"><span data-stu-id="6135a-p101">Create a **Conditional Access Policy** that defines what resources are being protected, and what conditions need to be met to access those resources. For example, a device must be compliant before accessing corporate email.</span></span> 
    
- <span data-ttu-id="6135a-p102">Създаване на **Спазване на политиката** да дефинирате настройки, които трябва да бъдат изпълнени, преди устройството се счита съвместим. Например устройство трябва да има ПИН на най-малко 6 цифри преди се счита съвместим.</span><span class="sxs-lookup"><span data-stu-id="6135a-p102">Create a **Compliance Policy** to define settings that must be met before the device is considered compliant. For example, a device must have a pin of at least 6 digits before it is considered compliant.</span></span> 
    
- <span data-ttu-id="6135a-p103">Гарантира **Съответствие политики** и **Условен достъп политики** са насочени към желаните групи от потребители. Това може да наложи създаването на специфични групи от потребители в Azure Active Directory.</span><span class="sxs-lookup"><span data-stu-id="6135a-p103">Ensuring both **Compliance Policies** and **Conditional Access Policies** are targeted to the desired groups of users. This may require creating specific groups of users in Azure Active Directory.</span></span> 
    
<span data-ttu-id="6135a-110">Прочетете още:</span><span class="sxs-lookup"><span data-stu-id="6135a-110">Read more:</span></span>
  
- [<span data-ttu-id="6135a-111">Условен достъп най-добрите практики</span><span class="sxs-lookup"><span data-stu-id="6135a-111">Conditional Access best practices</span></span>](https://docs.microsoft.com/azure/active-directory/conditional-access/best-practices)
    
- [<span data-ttu-id="6135a-112">Запознаване с условен достъп</span><span class="sxs-lookup"><span data-stu-id="6135a-112">Getting started with Conditional Access </span></span>](https://docs.microsoft.com/azure/active-directory/active-directory-conditional-access-azure-portal-get-started)
    

