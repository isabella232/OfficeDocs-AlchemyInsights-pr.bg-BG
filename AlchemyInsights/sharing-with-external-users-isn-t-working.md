---
title: Споделяне с външните потребители не работи
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
ms.sourcegitcommit: 1d98db8acb9959aba3b5e308a567ade6b62da56c
ms.translationtype: MT
ms.contentlocale: bg-BG
ms.lasthandoff: 08/22/2019
ms.locfileid: "36502220"
---
# <a name="fix-problems-sharing-sharepoint-content-with-external-users"></a><span data-ttu-id="72f66-102">Отстраняване на проблеми, споделяне на съдържание в SharePoint с външни потребители</span><span class="sxs-lookup"><span data-stu-id="72f66-102">Fix problems sharing SharePoint content with external users</span></span>

<span data-ttu-id="72f66-103">Уверете се, че външни е включено споделяне за вашата организация:</span><span class="sxs-lookup"><span data-stu-id="72f66-103">Make sure external sharing is turned on for your organization:</span></span>
  
1. <span data-ttu-id="72f66-104">Отидете на [услуги &amp; добавки страница в центъра за администрация на Microsoft 365](https://portal.office.com/adminportal/home#/Settings/ServicesAndAddIns), щракнете върху **сайтове**.</span><span class="sxs-lookup"><span data-stu-id="72f66-104">Go to the [Services &amp; add-ins page in the Microsoft 365 admin center](https://portal.office.com/adminportal/home#/Settings/ServicesAndAddIns), and click **Sites**.</span></span>
    
2. <span data-ttu-id="72f66-105">Уверете се, че настройката е се обърна към "За."</span><span class="sxs-lookup"><span data-stu-id="72f66-105">Make sure the setting is turned to "On."</span></span> <span data-ttu-id="72f66-106">Ако е отметнато "Само съществуващи външни потребители", се уверете, че външните потребител е включен в центъра за администрация на Microsoft 365.</span><span class="sxs-lookup"><span data-stu-id="72f66-106">If "Only existing external users" is selected, make sure the external user is listed in the Microsoft 365 admin center.</span></span>
    
<span data-ttu-id="72f66-107">Уверете се, външно споделяне, включено за сайта.</span><span class="sxs-lookup"><span data-stu-id="72f66-107">Make sure external sharing it turned on for the site.</span></span> <span data-ttu-id="72f66-108">За класически колекция:</span><span class="sxs-lookup"><span data-stu-id="72f66-108">For a classic site collection:</span></span>
  
1. <span data-ttu-id="72f66-109">В новата SharePoint администратор център, в левия екран щракнете върху **сайтове**.</span><span class="sxs-lookup"><span data-stu-id="72f66-109">In the new SharePoint admin center, in the left pane, click **sites**.</span></span>
    
2. <span data-ttu-id="72f66-110">Изберете сайт или сайтове, както и на лентата, щракнете върху **споделяне**.</span><span class="sxs-lookup"><span data-stu-id="72f66-110">Select the site or sites, and on the ribbon, click **Sharing**.</span></span>
    
<span data-ttu-id="72f66-111">За сайт на екип, който принадлежи към група на Office 365 или сайт на комуникация:</span><span class="sxs-lookup"><span data-stu-id="72f66-111">For a team site that belongs to an Office 365 group, or a communication site:</span></span>
  
- <span data-ttu-id="72f66-112">Тези нови видове на сайта имат същата споделяне настройка като вашата организационно настройка, освен ако организационно настройка позволява споделяне на файлове с помощта на връзки, които не изискват вход.</span><span class="sxs-lookup"><span data-stu-id="72f66-112">These new site types have the same sharing setting as your organization-wide setting, unless the organization-wide setting allows sharing files using links that don't require sign-in.</span></span> <span data-ttu-id="72f66-113">В този случай сайтове позволяват споделяне с нови и съществуващи външни потребители, които се регистрират в.</span><span class="sxs-lookup"><span data-stu-id="72f66-113">In this case, the sites allow sharing with new and existing external users who sign in.</span></span> <span data-ttu-id="72f66-114">За да промените настройката за конкретни сайтове, използвайте нов център за администриране на SharePoint или PowerShell.</span><span class="sxs-lookup"><span data-stu-id="72f66-114">To change the setting for specific sites, use the new SharePoint admin center or PowerShell.</span></span> <span data-ttu-id="72f66-115">[Научете повече](https://go.microsoft.com/fwlink/?linkid=871863).</span><span class="sxs-lookup"><span data-stu-id="72f66-115">[Learn more](https://go.microsoft.com/fwlink/?linkid=871863).</span></span>
    
> [!NOTE]
> <span data-ttu-id="72f66-116">Външно споделяне Настройка за всеки сайт може да бъде по-ограничителни от вашата организационно настройка, но не по-хлабави от общоорганизационни настройката.</span><span class="sxs-lookup"><span data-stu-id="72f66-116">The external sharing setting for any site can be more restrictive than your organization-wide setting, but not more permissive than the organization-wide setting.</span></span> 
  

