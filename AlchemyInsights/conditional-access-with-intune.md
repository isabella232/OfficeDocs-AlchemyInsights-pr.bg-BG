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
ms.sourcegitcommit: 9d78905c512192ffc4675468abd2efc5f2e4baf4
ms.translationtype: MT
ms.contentlocale: bg-BG
ms.lasthandoff: 04/23/2019
ms.locfileid: "32393530"
---
# <a name="conditional-access-with-intune"></a><span data-ttu-id="0a438-102">Условен достъп с Intune</span><span class="sxs-lookup"><span data-stu-id="0a438-102">Conditional Access with Intune</span></span>

<span data-ttu-id="0a438-103">Използване на **Условен достъп** с Intune изисква три стъпки:</span><span class="sxs-lookup"><span data-stu-id="0a438-103">Using **Conditional Access** with Intune requires 3 steps:</span></span> 
  
- <span data-ttu-id="0a438-104">Създаване на **Условен достъп политика** , която дефинира какви ресурси са защитени, както и какви условия трябва да бъдат изпълнени за достъп до тези ресурси.</span><span class="sxs-lookup"><span data-stu-id="0a438-104">Create a **Conditional Access Policy** that defines what resources are being protected, and what conditions need to be met to access those resources.</span></span> <span data-ttu-id="0a438-105">Например устройството трябва да бъде съвместим преди достъп до корпоративни имейл.</span><span class="sxs-lookup"><span data-stu-id="0a438-105">For example, a device must be compliant before accessing corporate email.</span></span> 
    
- <span data-ttu-id="0a438-106">Създаване на **Спазване на политиката** да дефинирате настройки, които трябва да бъдат изпълнени, преди устройството се счита съвместим.</span><span class="sxs-lookup"><span data-stu-id="0a438-106">Create a **Compliance Policy** to define settings that must be met before the device is considered compliant.</span></span> <span data-ttu-id="0a438-107">Например устройство трябва да има ПИН на най-малко 6 цифри преди се счита съвместим.</span><span class="sxs-lookup"><span data-stu-id="0a438-107">For example, a device must have a pin of at least 6 digits before it is considered compliant.</span></span> 
    
- <span data-ttu-id="0a438-108">Гарантира **Съответствие политики** и **Условен достъп политики** са насочени към желаните групи от потребители.</span><span class="sxs-lookup"><span data-stu-id="0a438-108">Ensuring both **Compliance Policies** and **Conditional Access Policies** are targeted to the desired groups of users.</span></span> <span data-ttu-id="0a438-109">Това може да наложи създаването на специфични групи от потребители в Azure Active Directory.</span><span class="sxs-lookup"><span data-stu-id="0a438-109">This may require creating specific groups of users in Azure Active Directory.</span></span> 
    
<span data-ttu-id="0a438-110">Прочетете още:</span><span class="sxs-lookup"><span data-stu-id="0a438-110">Read more:</span></span>
  
- [<span data-ttu-id="0a438-111">Условен достъп най-добрите практики</span><span class="sxs-lookup"><span data-stu-id="0a438-111">Conditional Access best practices</span></span>](https://docs.microsoft.com/azure/active-directory/conditional-access/best-practices)
    
- [<span data-ttu-id="0a438-112">Запознаване с условен достъп</span><span class="sxs-lookup"><span data-stu-id="0a438-112">Getting started with Conditional Access </span></span>](https://docs.microsoft.com/azure/active-directory/active-directory-conditional-access-azure-portal-get-started)
    

