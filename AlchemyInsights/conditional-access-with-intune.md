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
ms.openlocfilehash: e147e7460ee6a786e577a43c0b8355fc27ee367b
ms.sourcegitcommit: 1d98db8acb9959aba3b5e308a567ade6b62da56c
ms.translationtype: MT
ms.contentlocale: bg-BG
ms.lasthandoff: 08/22/2019
ms.locfileid: "36504983"
---
# <a name="conditional-access-with-intune"></a><span data-ttu-id="fb529-102">Условен достъп с Intune</span><span class="sxs-lookup"><span data-stu-id="fb529-102">Conditional Access with Intune</span></span>

<span data-ttu-id="fb529-103">Използване на **Условен достъп** с Intune изисква три стъпки:</span><span class="sxs-lookup"><span data-stu-id="fb529-103">Using **Conditional Access** with Intune requires 3 steps:</span></span> 
  
- <span data-ttu-id="fb529-104">Създаване на **Условен достъп политика** , която дефинира какви ресурси са защитени, както и какви условия трябва да бъдат изпълнени за достъп до тези ресурси.</span><span class="sxs-lookup"><span data-stu-id="fb529-104">Create a **Conditional Access Policy** that defines what resources are being protected, and what conditions need to be met to access those resources.</span></span> <span data-ttu-id="fb529-105">Например устройството трябва да бъде съвместим преди достъп до корпоративни имейл.</span><span class="sxs-lookup"><span data-stu-id="fb529-105">For example, a device must be compliant before accessing corporate email.</span></span> 
    
- <span data-ttu-id="fb529-106">Създаване на **Спазване на политиката** да дефинирате настройки, които трябва да бъдат изпълнени, преди устройството се счита съвместим.</span><span class="sxs-lookup"><span data-stu-id="fb529-106">Create a **Compliance Policy** to define settings that must be met before the device is considered compliant.</span></span> <span data-ttu-id="fb529-107">Например устройство трябва да има ПИН на най-малко 6 цифри преди се счита съвместим.</span><span class="sxs-lookup"><span data-stu-id="fb529-107">For example, a device must have a pin of at least 6 digits before it is considered compliant.</span></span> 
    
- <span data-ttu-id="fb529-108">Гарантира **Съответствие политики** и **Условен достъп политики** са насочени към желаните групи от потребители.</span><span class="sxs-lookup"><span data-stu-id="fb529-108">Ensuring both **Compliance Policies** and **Conditional Access Policies** are targeted to the desired groups of users.</span></span> <span data-ttu-id="fb529-109">Това може да наложи създаването на специфични групи от потребители в Azure Active Directory.</span><span class="sxs-lookup"><span data-stu-id="fb529-109">This may require creating specific groups of users in Azure Active Directory.</span></span> 
    
<span data-ttu-id="fb529-110">Прочетете още:</span><span class="sxs-lookup"><span data-stu-id="fb529-110">Read more:</span></span>
  
- [<span data-ttu-id="fb529-111">Условен достъп най-добрите практики</span><span class="sxs-lookup"><span data-stu-id="fb529-111">Conditional Access best practices</span></span>](https://docs.microsoft.com/azure/active-directory/conditional-access/best-practices)
    
- [<span data-ttu-id="fb529-112">Запознаване с условен достъп</span><span class="sxs-lookup"><span data-stu-id="fb529-112">Getting started with Conditional Access </span></span>](https://docs.microsoft.com/azure/active-directory/active-directory-conditional-access-azure-portal-get-started)
    

