---
title: Споделяне с външните потребители не работи
ms.author: mikeplum
author: MikePlumleyMSFT
manager: scotv
ms.date: 5/18/2018
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom: Adm_O365
ms.assetid: d3d0b69b-214e-4859-8957-621fd6306b30
ms.openlocfilehash: 305b3891e6c83e27b5c55c13757640e6e9d51a81
ms.sourcegitcommit: e2864efcfb493b6e46b662b746661a61232bdba7
ms.translationtype: MT
ms.contentlocale: bg-BG
ms.lasthandoff: 01/24/2019
ms.locfileid: "29458150"
---
# <a name="fix-problems-sharing-sharepoint-content-with-external-users"></a><span data-ttu-id="bcf5f-102">Отстраняване на проблеми, споделяне на съдържание в SharePoint с външни потребители</span><span class="sxs-lookup"><span data-stu-id="bcf5f-102">Fix problems sharing SharePoint content with external users</span></span>

<span data-ttu-id="bcf5f-103">Уверете се, че външни е включено споделяне за вашата организация:</span><span class="sxs-lookup"><span data-stu-id="bcf5f-103">Make sure external sharing is turned on for your organization:</span></span>
  
1. <span data-ttu-id="bcf5f-104">Отидете на [услуги &amp; добавки страница в центъра за администрация на Office 365](https://portal.office.com/adminportal/home#/Settings/ServicesAndAddIns), щракнете върху **сайтове**.</span><span class="sxs-lookup"><span data-stu-id="bcf5f-104">Go to the [Services &amp; add-ins page in the Office 365 admin center](https://portal.office.com/adminportal/home#/Settings/ServicesAndAddIns), and click **Sites**.</span></span>
    
2. <span data-ttu-id="bcf5f-p101">Уверете се, че настройката е се обърна към "За." Ако е отметнато "Само съществуващи външни потребители", се уверете, че външните потребител е включен в центъра за администрация на Office 365.</span><span class="sxs-lookup"><span data-stu-id="bcf5f-p101">Make sure the setting is turned to "On." If "Only existing external users" is selected, make sure the external user is listed in the Office 365 admin center.</span></span>
    
<span data-ttu-id="bcf5f-p102">Уверете се, външно споделяне, включено за сайта. За класически колекция:</span><span class="sxs-lookup"><span data-stu-id="bcf5f-p102">Make sure external sharing it turned on for the site. For a classic site collection:</span></span>
  
1. <span data-ttu-id="bcf5f-109">В класически SharePoint администратор център, в левия екран щракнете върху **колекции от сайтове**.</span><span class="sxs-lookup"><span data-stu-id="bcf5f-109">In the classic SharePoint admin center, in the left pane, click **site collections**.</span></span>
    
2. <span data-ttu-id="bcf5f-110">Изберете сайт или сайтове, както и на лентата, щракнете върху **споделяне**.</span><span class="sxs-lookup"><span data-stu-id="bcf5f-110">Select the site or sites, and on the ribbon, click **Sharing**.</span></span>
    
<span data-ttu-id="bcf5f-111">За сайт на екип, който принадлежи към група на Office 365 или сайт на комуникация:</span><span class="sxs-lookup"><span data-stu-id="bcf5f-111">For a team site that belongs to an Office 365 group, or a communication site:</span></span>
  
- <span data-ttu-id="bcf5f-p103">Тези нови видове на сайта имат същата споделяне настройка като вашата организационно настройка, освен ако организационно настройка позволява споделяне на файлове с помощта на връзки, които не изискват вход. В този случай сайтове позволяват споделяне с нови и съществуващи външни потребители, които се регистрират в. За да промените настройката за конкретни сайтове, използвайте нов център за администриране на SharePoint (визуализация) или PowerShell. [Научете повече](https://go.microsoft.com/fwlink/?linkid=871863).</span><span class="sxs-lookup"><span data-stu-id="bcf5f-p103">These new site types have the same sharing setting as your organization-wide setting, unless the organization-wide setting allows sharing files using links that don't require sign-in. In this case, the sites allow sharing with new and existing external users who sign in. To change the setting for specific sites, use the new SharePoint admin center (preview) or PowerShell. [Learn more](https://go.microsoft.com/fwlink/?linkid=871863).</span></span>
    
> [!NOTE]
> <span data-ttu-id="bcf5f-116">Външно споделяне Настройка за всеки сайт може да бъде по-ограничителни от вашата организационно настройка, но не по-хлабави от общоорганизационни настройката.</span><span class="sxs-lookup"><span data-stu-id="bcf5f-116">The external sharing setting for any site can be more restrictive than your organization-wide setting, but not more permissive than the organization-wide setting.</span></span> 
  

