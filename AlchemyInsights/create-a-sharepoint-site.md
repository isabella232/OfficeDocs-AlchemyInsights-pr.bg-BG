---
title: Създаване на сайт на SharePoint
ms.author: pebaum
author: todmccoy
ms.audience: Admin
ms.topic: article
ms.collection: Adm_O365
ms.prod: office-online-server
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "5200004"
- "3911416"
- "1386"
- "2303"
ms.assetid: e62b9f80-b017-42dc-9464-f4e32c19d6c9
ms.openlocfilehash: e1e71ae9401448ed18058f6307302dcbaf773649
ms.sourcegitcommit: 317eeed39c7777a922442992d67733726c41d9e1
ms.translationtype: MT
ms.contentlocale: bg-BG
ms.lasthandoff: 02/04/2020
ms.locfileid: "41770844"
---
# <a name="create-a-sharepoint-site"></a><span data-ttu-id="25b16-102">Създаване на сайт на SharePoint</span><span class="sxs-lookup"><span data-stu-id="25b16-102">Create a SharePoint site</span></span>

<span data-ttu-id="25b16-103">Създаване или управление на сайтове от [активни сайтове](https://admin.microsoft.com/sharepoint?page=sitemanagement&modern=true) в центъра за администриране на SharePoint.</span><span class="sxs-lookup"><span data-stu-id="25b16-103">Create or manage sites from [Active Sites](https://admin.microsoft.com/sharepoint?page=sitemanagement&modern=true) in the SharePoint Admin Center.</span></span> <span data-ttu-id="25b16-104">За повече информация вижте [Управление на сайтове в новия център за администриране на SharePoint](https://docs.microsoft.com/sharepoint/manage-site-creation).</span><span class="sxs-lookup"><span data-stu-id="25b16-104">For more info, see [Manage sites in the new SharePoint admin center](https://docs.microsoft.com/sharepoint/manage-site-creation).</span></span> 

## <a name="tips"></a><span data-ttu-id="25b16-105">Съвети:</span><span class="sxs-lookup"><span data-stu-id="25b16-105">Tips:</span></span>

- <span data-ttu-id="25b16-106">Не **можете да** създадете сайт със същия URL адрес на съществуващ сайт.</span><span class="sxs-lookup"><span data-stu-id="25b16-106">You **cannot** create a site with the same URL of an existing site.</span></span> <span data-ttu-id="25b16-107">Ако сте изтрили сайт и искате да използвате отново URL адреса, е възможно изтрит сайт все още съществува под [Изтрити сайтове](https://admin.microsoft.com/sharepoint?page=recyclebin&modern=true).</span><span class="sxs-lookup"><span data-stu-id="25b16-107">If you deleted a site and are wishing to re-use the URL, it's possible the deleted site still exists under [Deleted sites](https://admin.microsoft.com/sharepoint?page=recyclebin&modern=true).</span></span> <span data-ttu-id="25b16-108">Сайтът ще трябва да бъде изтрит за постоянно, за да използвате отново URL адреса.</span><span class="sxs-lookup"><span data-stu-id="25b16-108">The site will need to be permanently deleted to re-use the URL.</span></span> <span data-ttu-id="25b16-109">За да премахнете напълно сайт с Powershell, вижте [Премахване-SPSite](https://docs.microsoft.com/sharepoint/manage-sites-in-new-admin-center#delete-a-site) cmdlet пример.</span><span class="sxs-lookup"><span data-stu-id="25b16-109">To completely remove a site with Powershell, see the [Remove-SPSite](https://docs.microsoft.com/sharepoint/manage-sites-in-new-admin-center#delete-a-site) cmdlet example.</span></span>
- <span data-ttu-id="25b16-110">Някои потребители може да не могат да създадат сайт.</span><span class="sxs-lookup"><span data-stu-id="25b16-110">Some users may not be able to create a site.</span></span> <span data-ttu-id="25b16-111">[Вижте Управление на създаването на сайт в SharePoint Online](https://docs.microsoft.com/sharepoint/manage-site-creation).</span><span class="sxs-lookup"><span data-stu-id="25b16-111">[See Manage site creation in SharePoint Online](https://docs.microsoft.com/sharepoint/manage-site-creation).</span></span>
- <span data-ttu-id="25b16-112">Възможно е сайтът да изглежда залепен в **Създаване** на по-дълъг от очакваното.</span><span class="sxs-lookup"><span data-stu-id="25b16-112">It's possible the site appears stuck at **Creating** longer than expected.</span></span> <span data-ttu-id="25b16-113">Ако са изминали повече от 24 часа, откакто сте го видели за първи път, моля, влезте в билет за поддръжка.</span><span class="sxs-lookup"><span data-stu-id="25b16-113">If more than 24 hours have passed since you first saw this issue, please log a support ticket.</span></span> <span data-ttu-id="25b16-114">В много случаи ние вече работим по решение.</span><span class="sxs-lookup"><span data-stu-id="25b16-114">In many cases, we're already working on a solution.</span></span> <span data-ttu-id="25b16-115">Моля, дайте ни поне 24 часа, за да завършите решение.</span><span class="sxs-lookup"><span data-stu-id="25b16-115">Please give us at least 24 hours to complete a solution.</span></span>
