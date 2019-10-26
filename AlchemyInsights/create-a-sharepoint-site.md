---
title: Създаване на сайт на SharePoint
ms.author: efrene
author: efrene
ms.date: 1/16/2019
ms.audience: ITPro
ms.topic: article
ms.collection: Adm_O365
ms.prod: office-online-server
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "5200004"
- "1386"
- "2303"
ms.assetid: e62b9f80-b017-42dc-9464-f4e32c19d6c9
ms.openlocfilehash: 30c51d84005534cc1de9e8b8136da1a07be57b73
ms.sourcegitcommit: 0b06093dabd685f76cc39b1d7c0f8b03883b6e79
ms.translationtype: MT
ms.contentlocale: bg-BG
ms.lasthandoff: 10/25/2019
ms.locfileid: "36738186"
---
# <a name="create-a-sharepoint-site"></a><span data-ttu-id="663df-102">Създаване на сайт на SharePoint</span><span class="sxs-lookup"><span data-stu-id="663df-102">Create a SharePoint site</span></span>

<span data-ttu-id="663df-103">Можете да видите следното за информация за създаване на сайт на SharePoint:</span><span class="sxs-lookup"><span data-stu-id="663df-103">You can see the following for information about SharePoint site creation:</span></span>
- <span data-ttu-id="663df-104">[Управление на сайтове в новия център за администриране на SharePoint](https://docs.microsoft.com/sharepoint/manage-site-creation): Научете за опциите за създаване на сайт, включително как да създадете класически сайт или екип сайт, който не включва Office 365 група.</span><span class="sxs-lookup"><span data-stu-id="663df-104">[Manage sites in the new SharePoint admin center](https://docs.microsoft.com/sharepoint/manage-site-creation): Learn about site creation options, including how to create a classic site or a teams site that doesn't include an Office 365 group.</span></span>
- <span data-ttu-id="663df-105">[Създаване на екипен сайт в SharePoint](https://support.office.com/article/create-a-team-site-in-sharepoint-ef10c1e7-15f3-42a3-98aa-b5972711777d): Научете как да създадете екипен сайт.</span><span class="sxs-lookup"><span data-stu-id="663df-105">[Create a team site in SharePoint](https://support.office.com/article/create-a-team-site-in-sharepoint-ef10c1e7-15f3-42a3-98aa-b5972711777d): Learn how to create a team site.</span></span>
- <span data-ttu-id="663df-106">[Създаване на сайт за комуникация в SharePoint online](https://support.office.com/article/7fb44b20-a72f-4d2c-9173-fc8f59ba50eb): Научете как да създадете комуникационен сайт.</span><span class="sxs-lookup"><span data-stu-id="663df-106">[Create a communication site in SharePoint Online](https://support.office.com/article/7fb44b20-a72f-4d2c-9173-fc8f59ba50eb): Learn how to create a communications site.</span></span>
- <span data-ttu-id="663df-107">[Управление на сайтове в новия център за администриране на SharePoint](https://docs.microsoft.com/sharepoint/manage-sites-in-new-admin-center#create-a-site): Научете как да създадете класически сайт или екипен сайт, който не включва група на Office 365.</span><span class="sxs-lookup"><span data-stu-id="663df-107">[Manage sites in the new SharePoint admin center](https://docs.microsoft.com/sharepoint/manage-sites-in-new-admin-center#create-a-site):  Learn how to create a classic site or a team site that doesn't include an Office 365 group.</span></span>


  
> <span data-ttu-id="663df-108">[! Съвети</span><span class="sxs-lookup"><span data-stu-id="663df-108">[!Tips]</span></span>
> - <span data-ttu-id="663df-109">Не можете да създадете сайт със същия URL адрес на съществуващ сайт.</span><span class="sxs-lookup"><span data-stu-id="663df-109">You cannot create a site with the same URL of an existing site.</span></span> <span data-ttu-id="663df-110">Ако сте изтрили сайт и искате да използвате отново URL адреса, това е възможно изтрит сайт все още съществува в **Изтрити сайтове**.</span><span class="sxs-lookup"><span data-stu-id="663df-110">If you deleted a site and are wishing to re-use the URL, it's possible the deleted site still exists under **Deleted sites**.</span></span> <span data-ttu-id="663df-111">За да управлявате изтритите сайтове, [Изтрийте сайт](https://docs.microsoft.com/sharepoint/manage-sites-in-new-admin-center#delete-a-site).</span><span class="sxs-lookup"><span data-stu-id="663df-111">To manage deleted sites see, [Delete a Site](https://docs.microsoft.com/sharepoint/manage-sites-in-new-admin-center#delete-a-site).</span></span> <span data-ttu-id="663df-112">За да премахнете напълно сайт с PowerShell, вижте например команда за [Премахване на SPSite](https://docs.microsoft.com/sharepoint/manage-sites-in-new-admin-center#delete-a-site) .</span><span class="sxs-lookup"><span data-stu-id="663df-112">To completely remove a site with Powershell, see the [Remove-SPSite](https://docs.microsoft.com/sharepoint/manage-sites-in-new-admin-center#delete-a-site) cmdlet example.</span></span>
> - <span data-ttu-id="663df-113">Някои потребители може да не успеят да създадат сайт.</span><span class="sxs-lookup"><span data-stu-id="663df-113">Some users may not be able to create a site.</span></span> <span data-ttu-id="663df-114">Вижте [управление на създаването на сайт в SharePoint online](https://docs.microsoft.com/sharepoint/manage-site-creation).</span><span class="sxs-lookup"><span data-stu-id="663df-114">See [Manage site creation in SharePoint Online](https://docs.microsoft.com/sharepoint/manage-site-creation).</span></span>
> - <span data-ttu-id="663df-115">Това е възможно сайтът се появява остана в **Създаване** на повече от очакваното.</span><span class="sxs-lookup"><span data-stu-id="663df-115">It's possible the site appears stuck at **Creating** longer than expected.</span></span> <span data-ttu-id="663df-116">Ако са изминали повече от 24 часа от първия път, когато сте видели този проблем, моля, впишете билет за поддръжка.</span><span class="sxs-lookup"><span data-stu-id="663df-116">If more than 24 hours have passed since you first saw this issue, please log a support ticket.</span></span> <span data-ttu-id="663df-117">В много случаи вече работим по решение.</span><span class="sxs-lookup"><span data-stu-id="663df-117">In many cases, we're already working on a solution.</span></span> <span data-ttu-id="663df-118">Моля, дайте ни поне 24 часа, за да завършим решение.</span><span class="sxs-lookup"><span data-stu-id="663df-118">Please give us at least 24 hours to complete a solution.</span></span>
> - <span data-ttu-id="663df-119">Ако трябва да създадете нов екипен сайт, който не включва група на Office 365,</span><span class="sxs-lookup"><span data-stu-id="663df-119">If you need to create a new team site that doesn't include an Office 365 group,</span></span> 


