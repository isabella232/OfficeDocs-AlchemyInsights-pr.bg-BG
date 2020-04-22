---
title: Условен достъп с Intune
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: aecba7c5-e86d-4ec8-9d44-679f5a3d659d
ms.openlocfilehash: c9c47d71b2da3840504d5b28c7c9e067b4c05fa5
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: bg-BG
ms.lasthandoff: 04/22/2020
ms.locfileid: "43706010"
---
# <a name="conditional-access-with-intune"></a><span data-ttu-id="935bc-102">Условен достъп с Intune</span><span class="sxs-lookup"><span data-stu-id="935bc-102">Conditional Access with Intune</span></span>

<span data-ttu-id="935bc-103">Използването на **условен достъп** с Intune изисква 3 стъпки:</span><span class="sxs-lookup"><span data-stu-id="935bc-103">Using **Conditional Access** with Intune requires 3 steps:</span></span> 
  
- <span data-ttu-id="935bc-104">Създаване на **правила за условен достъп,** определящ какви ресурси са защитени и какви условия трябва да бъдат изпълнени, за да получите достъп до тези ресурси.</span><span class="sxs-lookup"><span data-stu-id="935bc-104">Create a **Conditional Access Policy** that defines what resources are being protected, and what conditions need to be met to access those resources.</span></span> <span data-ttu-id="935bc-105">Например, устройството трябва да е съвместимо, преди да има достъп до корпоративните имейли.</span><span class="sxs-lookup"><span data-stu-id="935bc-105">For example, a device must be compliant before accessing corporate email.</span></span> 
    
- <span data-ttu-id="935bc-106">Създаване на **правила за съответствие,** за да определите настройки, които трябва да бъдат изпълнени, преди устройството да се счита за съвместимо.</span><span class="sxs-lookup"><span data-stu-id="935bc-106">Create a **Compliance Policy** to define settings that must be met before the device is considered compliant.</span></span> <span data-ttu-id="935bc-107">Например, устройството трябва да има щифт от поне 6 цифри, преди да се счита за съвместимо.</span><span class="sxs-lookup"><span data-stu-id="935bc-107">For example, a device must have a pin of at least 6 digits before it is considered compliant.</span></span> 
    
- <span data-ttu-id="935bc-108">Осигуряването **на правила за съответствие** и политики за **условен достъп** са насочени към желаните групи потребители.</span><span class="sxs-lookup"><span data-stu-id="935bc-108">Ensuring both **Compliance Policies** and **Conditional Access Policies** are targeted to the desired groups of users.</span></span> <span data-ttu-id="935bc-109">Това може да изисква създаване на определени групи потребители в Azure Active Directory.</span><span class="sxs-lookup"><span data-stu-id="935bc-109">This may require creating specific groups of users in Azure Active Directory.</span></span> 
    
<span data-ttu-id="935bc-110">Прочетете повече:</span><span class="sxs-lookup"><span data-stu-id="935bc-110">Read more:</span></span>
  
- [<span data-ttu-id="935bc-111">Най-добри практики за условен достъп</span><span class="sxs-lookup"><span data-stu-id="935bc-111">Conditional Access best practices</span></span>](https://docs.microsoft.com/azure/active-directory/conditional-access/best-practices)
    
- [<span data-ttu-id="935bc-112">Първи стъпки с условния достъп</span><span class="sxs-lookup"><span data-stu-id="935bc-112">Getting started with Conditional Access </span></span>](https://docs.microsoft.com/azure/active-directory/active-directory-conditional-access-azure-portal-get-started)
    

