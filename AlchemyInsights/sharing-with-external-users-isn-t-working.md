---
title: Споделянето с външни потребители не работи
ms.author: mikeplum
author: MikePlumleyMSFT
manager: scotv
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: d3d0b69b-214e-4859-8957-621fd6306b30
ms.openlocfilehash: 9a40f52637bc8aa7894754118f0f862aa6c71fe2
ms.sourcegitcommit: f28dafa0f727870038f72bc904da926daf4ec07b
ms.translationtype: MT
ms.contentlocale: bg-BG
ms.lasthandoff: 06/05/2020
ms.locfileid: "44582764"
---
# <a name="fix-problems-sharing-sharepoint-content-with-external-users"></a><span data-ttu-id="e8699-102">Отстраняване на проблеми при споделяне на съдържание на SharePoint с външни потребители</span><span class="sxs-lookup"><span data-stu-id="e8699-102">Fix problems sharing SharePoint content with external users</span></span>

<span data-ttu-id="e8699-103">Уверете се, че външното споделяне е включено за вашата организация:</span><span class="sxs-lookup"><span data-stu-id="e8699-103">Make sure external sharing is turned on for your organization:</span></span>
  
1. <span data-ttu-id="e8699-104">Отидете на [страницата с добавки за услуги &amp; в центъра за администриране на Microsoft 365](https://portal.office.com/adminportal/home#/Settings/ServicesAndAddIns)и щракнете върху **Сайтове**.</span><span class="sxs-lookup"><span data-stu-id="e8699-104">Go to the [Services &amp; add-ins page in the Microsoft 365 admin center](https://portal.office.com/adminportal/home#/Settings/ServicesAndAddIns), and click **Sites**.</span></span>
    
2. <span data-ttu-id="e8699-105">Уверете се, че настройката е включена на "Включено".</span><span class="sxs-lookup"><span data-stu-id="e8699-105">Make sure the setting is turned to "On."</span></span> <span data-ttu-id="e8699-106">Ако е избрана опцията "Само съществуващите външни потребители", уверете се, че външният потребител е посочен в центъра за администриране на Microsoft 365.</span><span class="sxs-lookup"><span data-stu-id="e8699-106">If "Only existing external users" is selected, make sure the external user is listed in the Microsoft 365 admin center.</span></span>
    
<span data-ttu-id="e8699-107">Уверете се, че външното споделяне е включено за сайта.</span><span class="sxs-lookup"><span data-stu-id="e8699-107">Make sure external sharing it turned on for the site.</span></span> <span data-ttu-id="e8699-108">За класическа колекция от сайтове:</span><span class="sxs-lookup"><span data-stu-id="e8699-108">For a classic site collection:</span></span>
  
1. <span data-ttu-id="e8699-109">В новия център за администриране на SharePoint в левия прозорец щракнете върху **сайтове**.</span><span class="sxs-lookup"><span data-stu-id="e8699-109">In the new SharePoint admin center, in the left pane, click **sites**.</span></span>
    
2. <span data-ttu-id="e8699-110">Изберете сайта или сайтовете и върху лентата щракнете върху **Споделяне**.</span><span class="sxs-lookup"><span data-stu-id="e8699-110">Select the site or sites, and on the ribbon, click **Sharing**.</span></span>
    
<span data-ttu-id="e8699-111">За екипен сайт, който принадлежи към група на Microsoft 365 или комуникационен сайт:</span><span class="sxs-lookup"><span data-stu-id="e8699-111">For a team site that belongs to a Microsoft 365 group, or a communication site:</span></span>
  
- <span data-ttu-id="e8699-112">Тези нови типове сайтове имат същата настройка за споделяне като настройката за организацията, освен ако настройката за организация позволява споделяне на файлове, използващи връзки, които не изискват влизане.</span><span class="sxs-lookup"><span data-stu-id="e8699-112">These new site types have the same sharing setting as your organization-wide setting, unless the organization-wide setting allows sharing files using links that don't require sign-in.</span></span> <span data-ttu-id="e8699-113">В този случай сайтове позволяват споделяне с нови и съществуващи външни потребители, които влизат.</span><span class="sxs-lookup"><span data-stu-id="e8699-113">In this case, the sites allow sharing with new and existing external users who sign in.</span></span> <span data-ttu-id="e8699-114">За да промените настройката за определени сайтове, използвайте новия център за администриране на SharePoint или PowerShell.</span><span class="sxs-lookup"><span data-stu-id="e8699-114">To change the setting for specific sites, use the new SharePoint admin center or PowerShell.</span></span> <span data-ttu-id="e8699-115">[Научете повече](https://go.microsoft.com/fwlink/?linkid=871863).</span><span class="sxs-lookup"><span data-stu-id="e8699-115">[Learn more](https://go.microsoft.com/fwlink/?linkid=871863).</span></span>
    
> [!NOTE]
> <span data-ttu-id="e8699-116">Външната настройка за споделяне за всеки сайт може да бъде по-ограничителна от настройката на организацията, но не по-пускаща от настройката за организация.</span><span class="sxs-lookup"><span data-stu-id="e8699-116">The external sharing setting for any site can be more restrictive than your organization-wide setting, but not more permissive than the organization-wide setting.</span></span> 
  

