---
title: Създаване на сайт на SharePoint
ms.author: pebaum
author: pebaum
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
ms.openlocfilehash: ba682f3c2b2600031f6856621691b1e0fba64113
ms.sourcegitcommit: 90f37eebec9aaa9e49c2cf4d201152c5e20e384b
ms.translationtype: MT
ms.contentlocale: bg-BG
ms.lasthandoff: 08/17/2020
ms.locfileid: "46786554"
---
# <a name="create-a-sharepoint-site"></a><span data-ttu-id="ff210-102">Създаване на сайт на SharePoint</span><span class="sxs-lookup"><span data-stu-id="ff210-102">Create a SharePoint site</span></span>

<span data-ttu-id="ff210-103">Създаване и управление на сайтове от [активни сайтове](https://admin.microsoft.com/sharepoint?page=sitemanagement&modern=true) в центъра за администриране на SharePoint.</span><span class="sxs-lookup"><span data-stu-id="ff210-103">Create or manage sites from [Active Sites](https://admin.microsoft.com/sharepoint?page=sitemanagement&modern=true) in the SharePoint Admin Center.</span></span> <span data-ttu-id="ff210-104">За повече информация вижте [управление на сайтове в новия център за администриране на SharePoint](https://docs.microsoft.com/sharepoint/manage-site-creation).</span><span class="sxs-lookup"><span data-stu-id="ff210-104">For more info, see [Manage sites in the new SharePoint admin center](https://docs.microsoft.com/sharepoint/manage-site-creation).</span></span> 

## <a name="tips"></a><span data-ttu-id="ff210-105">Съвети</span><span class="sxs-lookup"><span data-stu-id="ff210-105">Tips:</span></span>

- <span data-ttu-id="ff210-106">**Не можете да** създадете сайт със същия URL адрес на съществуващ сайт.</span><span class="sxs-lookup"><span data-stu-id="ff210-106">You **cannot** create a site with the same URL of an existing site.</span></span> <span data-ttu-id="ff210-107">Ако сте изтрили сайт и искате да го използвате повторно, е възможно изтрит сайт все още да съществува под " [Изтрити сайтове](https://admin.microsoft.com/sharepoint?page=recyclebin&modern=true)".</span><span class="sxs-lookup"><span data-stu-id="ff210-107">If you deleted a site and are wishing to re-use the URL, it's possible the deleted site still exists under [Deleted sites](https://admin.microsoft.com/sharepoint?page=recyclebin&modern=true).</span></span> <span data-ttu-id="ff210-108">Сайтът ще трябва да бъде окончателно изтрит за повторно използване на URL адреса.</span><span class="sxs-lookup"><span data-stu-id="ff210-108">The site will need to be permanently deleted to re-use the URL.</span></span> <span data-ttu-id="ff210-109">За да премахнете напълно сайт с PowerShell, вижте пример за кратка команда [Remove-SPSite](https://docs.microsoft.com/sharepoint/manage-sites-in-new-admin-center#delete-a-site) .</span><span class="sxs-lookup"><span data-stu-id="ff210-109">To completely remove a site with Powershell, see the [Remove-SPSite](https://docs.microsoft.com/sharepoint/manage-sites-in-new-admin-center#delete-a-site) cmdlet example.</span></span>
- <span data-ttu-id="ff210-110">Някои потребители може да не успеят да създадат сайт.</span><span class="sxs-lookup"><span data-stu-id="ff210-110">Some users may not be able to create a site.</span></span> <span data-ttu-id="ff210-111">[Вижте управление на създаването на сайтове в SharePoint online](https://docs.microsoft.com/sharepoint/manage-site-creation).</span><span class="sxs-lookup"><span data-stu-id="ff210-111">[See Manage site creation in SharePoint Online](https://docs.microsoft.com/sharepoint/manage-site-creation).</span></span>
- <span data-ttu-id="ff210-112">Възможно е сайтът да се показва заседнал при **създаването** на по-дълго от очакваното.</span><span class="sxs-lookup"><span data-stu-id="ff210-112">It's possible the site appears stuck at **Creating** longer than expected.</span></span> <span data-ttu-id="ff210-113">Ако са изминали повече от 24 часа, откакто за пръв път видяхте този проблем, можете да регистрирате билет за поддръжка.</span><span class="sxs-lookup"><span data-stu-id="ff210-113">If more than 24 hours have passed since you first saw this issue, please log a support ticket.</span></span> <span data-ttu-id="ff210-114">В много случаи вече работим върху решение.</span><span class="sxs-lookup"><span data-stu-id="ff210-114">In many cases, we're already working on a solution.</span></span> <span data-ttu-id="ff210-115">Моля, дайте ни най-малко 24 часа, за да завършите решение.</span><span class="sxs-lookup"><span data-stu-id="ff210-115">Please give us at least 24 hours to complete a solution.</span></span>
