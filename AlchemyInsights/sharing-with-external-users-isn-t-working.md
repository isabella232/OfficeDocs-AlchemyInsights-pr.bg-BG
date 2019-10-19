---
title: Споделянето с външни потребители не работи
ms.author: mikeplum
author: MikePlumleyMSFT
manager: scotv
ms.date: 5/18/2018
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: d3d0b69b-214e-4859-8957-621fd6306b30
ms.openlocfilehash: d4c8fc75ff8db2319b88a20bea9b3ee661f2e36e
ms.sourcegitcommit: 037331d71f06750d972c0b6278b23bb15c4806ca
ms.translationtype: MT
ms.contentlocale: bg-BG
ms.lasthandoff: 10/18/2019
ms.locfileid: "36502220"
---
# <a name="fix-problems-sharing-sharepoint-content-with-external-users"></a><span data-ttu-id="125ac-102">Отстраняване на проблеми при споделянето на съдържание на SharePoint с външни потребители</span><span class="sxs-lookup"><span data-stu-id="125ac-102">Fix problems sharing SharePoint content with external users</span></span>

<span data-ttu-id="125ac-103">Уверете се, че външното споделяне е включено за вашата организация:</span><span class="sxs-lookup"><span data-stu-id="125ac-103">Make sure external sharing is turned on for your organization:</span></span>
  
1. <span data-ttu-id="125ac-104">Отидете на [страницата с &amp; добавки за услуги в центъра за администриране на Microsoft 365](https://portal.office.com/adminportal/home#/Settings/ServicesAndAddIns)и щракнете върху **сайтове**.</span><span class="sxs-lookup"><span data-stu-id="125ac-104">Go to the [Services &amp; add-ins page in the Microsoft 365 admin center](https://portal.office.com/adminportal/home#/Settings/ServicesAndAddIns), and click **Sites**.</span></span>
    
2. <span data-ttu-id="125ac-105">Уверете се, че настройката е обърната към "включено".</span><span class="sxs-lookup"><span data-stu-id="125ac-105">Make sure the setting is turned to "On."</span></span> <span data-ttu-id="125ac-106">Ако е избрана "само съществуващи външни потребители", уверете се, че външният потребител е включен в центъра за администриране на Microsoft 365.</span><span class="sxs-lookup"><span data-stu-id="125ac-106">If "Only existing external users" is selected, make sure the external user is listed in the Microsoft 365 admin center.</span></span>
    
<span data-ttu-id="125ac-107">Уверете се, че външното споделяне е включено за сайта.</span><span class="sxs-lookup"><span data-stu-id="125ac-107">Make sure external sharing it turned on for the site.</span></span> <span data-ttu-id="125ac-108">За класическа колекция от сайтове:</span><span class="sxs-lookup"><span data-stu-id="125ac-108">For a classic site collection:</span></span>
  
1. <span data-ttu-id="125ac-109">В новия център за администриране на SharePoint в левия екран щракнете върху **сайтове**.</span><span class="sxs-lookup"><span data-stu-id="125ac-109">In the new SharePoint admin center, in the left pane, click **sites**.</span></span>
    
2. <span data-ttu-id="125ac-110">Изберете сайта или сайтовете и в лентата щракнете върху **споделяне**.</span><span class="sxs-lookup"><span data-stu-id="125ac-110">Select the site or sites, and on the ribbon, click **Sharing**.</span></span>
    
<span data-ttu-id="125ac-111">За екипен сайт, който принадлежи към група на Office 365 или сайт за комуникация:</span><span class="sxs-lookup"><span data-stu-id="125ac-111">For a team site that belongs to an Office 365 group, or a communication site:</span></span>
  
- <span data-ttu-id="125ac-112">Тези нови типове сайтове имат една и съща настройка за споделяне като вашата организационна настройка, освен ако настройката за цялата организация позволява споделяне на файлове с помощта на връзки, които не изискват влизане.</span><span class="sxs-lookup"><span data-stu-id="125ac-112">These new site types have the same sharing setting as your organization-wide setting, unless the organization-wide setting allows sharing files using links that don't require sign-in.</span></span> <span data-ttu-id="125ac-113">В този случай сайтовете позволяват споделяне с нови и съществуващи външни потребители, които се подписват.</span><span class="sxs-lookup"><span data-stu-id="125ac-113">In this case, the sites allow sharing with new and existing external users who sign in.</span></span> <span data-ttu-id="125ac-114">За да промените настройката за определени сайтове, използвайте новия център за администриране на SharePoint или PowerShell.</span><span class="sxs-lookup"><span data-stu-id="125ac-114">To change the setting for specific sites, use the new SharePoint admin center or PowerShell.</span></span> <span data-ttu-id="125ac-115">[Научете повече](https://go.microsoft.com/fwlink/?linkid=871863).</span><span class="sxs-lookup"><span data-stu-id="125ac-115">[Learn more](https://go.microsoft.com/fwlink/?linkid=871863).</span></span>
    
> [!NOTE]
> <span data-ttu-id="125ac-116">Настройката за външно споделяне за всеки сайт може да бъде по-ограничителна от настройката за цялата организация, но не по-разрешима от настройката за цялата организация.</span><span class="sxs-lookup"><span data-stu-id="125ac-116">The external sharing setting for any site can be more restrictive than your organization-wide setting, but not more permissive than the organization-wide setting.</span></span> 
  

