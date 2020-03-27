---
title: Трайно изтриване на сайт в SharePoint
ms.author: pebaum
author: pebaum
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.custom: ''
ms.assetid:
- "5200006"
- "4391"
ms.openlocfilehash: 263317339d965d173a5a038fa006e0ce6f8476cc
ms.sourcegitcommit: da04e79b6072321caa16a6ceea6eb5f15de22394
ms.translationtype: HT
ms.contentlocale: bg-BG
ms.lasthandoff: 03/25/2020
ms.locfileid: "42955099"
---
# <a name="permanently-delete-a-site-in-sharepoint"></a><span data-ttu-id="86c05-102">Трайно изтриване на сайт в SharePoint</span><span class="sxs-lookup"><span data-stu-id="86c05-102">Permanently delete a site in SharePoint</span></span>

<span data-ttu-id="86c05-103">За да използвате отново URL адрес от изтрит сайт (за да създадете отново сайт), или за да изтриете трайно сайт, тъй като той вече не се използва, можете да използвате **Трайно изтриване** от новия център за администриране на SharePoint.</span><span class="sxs-lookup"><span data-stu-id="86c05-103">To reuse a URL from a deleted site (to recreate a site), or to permanently delete a site because it's no longer in use, you can use **Permanently Delete** from the New SharePoint Admin Center.</span></span> 

1. <span data-ttu-id="86c05-104">Отидете на страницата [Изтрити сайтове на новия център за администриране на SharePoint](https://admin.microsoft.com/sharepoint?page=recycleBin&modern=true) и влезте с акаунт, който има разрешения на администратор за вашата организация.</span><span class="sxs-lookup"><span data-stu-id="86c05-104">Go to the [Deleted sites page of the new SharePoint admin center](https://admin.microsoft.com/sharepoint?page=recycleBin&modern=true) and sign in with an account that has admin permissions for your organization.</span></span> 

2. <span data-ttu-id="86c05-105">От лявата колона изберете сайт. </span><span class="sxs-lookup"><span data-stu-id="86c05-105">In the left column, select a site.</span></span> 

3. <span data-ttu-id="86c05-106">Щракнете върху **Трайно изтриване**.</span><span class="sxs-lookup"><span data-stu-id="86c05-106">Click **Permanently Delete**.</span></span> 

<span data-ttu-id="86c05-107">**Забележка**: сайтовете, свързани с групи, не могат да се изтрият трайно от новия център за администриране на SharePoint.</span><span class="sxs-lookup"><span data-stu-id="86c05-107">**Note**: Group-connected sites cannot be permanently deleted from the New SharePoint Admin Center.</span></span> <span data-ttu-id="86c05-108">Вместо това ще трябва да се използва [Премахване на SPODeletedSite](https://docs.microsoft.com/powershell/module/sharepoint-online/remove-spodeletedsite).</span><span class="sxs-lookup"><span data-stu-id="86c05-108">[Remove-SPODeletedSite](https://docs.microsoft.com/powershell/module/sharepoint-online/remove-spodeletedsite) will need to be used instead.</span></span>  

<span data-ttu-id="86c05-109">За повече информация вижте [Трайно изтриване на сайт](https://docs.microsoft.com/sharepoint/delete-site-collection#permanently-delete-a-site).</span><span class="sxs-lookup"><span data-stu-id="86c05-109">For more info, see [Permanently delete a site](https://docs.microsoft.com/sharepoint/delete-site-collection#permanently-delete-a-site).</span></span> 
