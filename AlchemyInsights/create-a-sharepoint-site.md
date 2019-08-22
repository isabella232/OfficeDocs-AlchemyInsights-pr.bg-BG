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
ms.openlocfilehash: 96780bd2f4182c1385406ec2a31cd62745137985
ms.sourcegitcommit: 1d98db8acb9959aba3b5e308a567ade6b62da56c
ms.translationtype: MT
ms.contentlocale: bg-BG
ms.lasthandoff: 08/22/2019
ms.locfileid: "36515796"
---
# <a name="create-a-sharepoint-site"></a><span data-ttu-id="28b93-102">Създаване на сайт на SharePoint</span><span class="sxs-lookup"><span data-stu-id="28b93-102">Create a SharePoint site</span></span>

<span data-ttu-id="28b93-103">Можете да видите следната информация за създаване на сайт на SharePoint:</span><span class="sxs-lookup"><span data-stu-id="28b93-103">You can see the following for information about SharePoint site creation:</span></span>
- <span data-ttu-id="28b93-104">[Управление на сайтове в центъра за администрация на нови SharePoint](https://docs.microsoft.com/sharepoint/manage-site-creation): Научете повече за сайт създаване опции, включително как да се създаде един класически сайт или екипи сайт, който не включва група на Office 365.</span><span class="sxs-lookup"><span data-stu-id="28b93-104">[Manage sites in the new SharePoint admin center](https://docs.microsoft.com/sharepoint/manage-site-creation): Learn about site creation options, including how to create a classic site or a teams site that doesn't include an Office 365 group.</span></span>
- <span data-ttu-id="28b93-105">[Създаване на екип сайт в SharePoint](https://support.office.com/article/create-a-team-site-in-sharepoint-ef10c1e7-15f3-42a3-98aa-b5972711777d?ui=en-US&amp;rs=en-US&amp;ad=US): Научете как да създадете сайт на екип.</span><span class="sxs-lookup"><span data-stu-id="28b93-105">[Create a team site in SharePoint](https://support.office.com/article/create-a-team-site-in-sharepoint-ef10c1e7-15f3-42a3-98aa-b5972711777d?ui=en-US&amp;rs=en-US&amp;ad=US): Learn how to create a team site.</span></span>
- <span data-ttu-id="28b93-106">[Създаване на съобщение сайт в SharePoint Online](https://support.office.com/article/7fb44b20-a72f-4d2c-9173-fc8f59ba50eb): Научете как да създадете сайт, комуникации.</span><span class="sxs-lookup"><span data-stu-id="28b93-106">[Create a communication site in SharePoint Online](https://support.office.com/article/7fb44b20-a72f-4d2c-9173-fc8f59ba50eb): Learn how to create a communications site.</span></span>
- <span data-ttu-id="28b93-107">[Управление на сайтове в центъра за администрация на нови SharePoint](https://docs.microsoft.com/sharepoint/manage-sites-in-new-admin-center#create-a-site): Научете как да създадете един класически сайт или сайт на екип, който не съдържа група на Office 365.</span><span class="sxs-lookup"><span data-stu-id="28b93-107">[Manage sites in the new SharePoint admin center](https://docs.microsoft.com/sharepoint/manage-sites-in-new-admin-center#create-a-site):  Learn how to create a classic site or a team site that doesn't include an Office 365 group.</span></span>


  
> [! Съвети]
> - <span data-ttu-id="28b93-109">Не можете да създадете сайт на същия URL адрес на съществуващ сайт.</span><span class="sxs-lookup"><span data-stu-id="28b93-109">You cannot create a site with the same URL of an existing site.</span></span> <span data-ttu-id="28b93-110">Ако изтрит даден сайт и желаещи да повторно използване на URL, е възможно изтрити сайт все още съществува под **Изтрити сайтове**.</span><span class="sxs-lookup"><span data-stu-id="28b93-110">If you deleted a site and are wishing to re-use the URL, it's possible the deleted site still exists under **Deleted sites**.</span></span> <span data-ttu-id="28b93-111">За да управлявате изтрити вж. сайтове, [Изтриване на сайт](https://docs.microsoft.com/sharepoint/manage-sites-in-new-admin-center#delete-a-site).</span><span class="sxs-lookup"><span data-stu-id="28b93-111">To manage deleted sites see, [Delete a Site](https://docs.microsoft.com/sharepoint/manage-sites-in-new-admin-center#delete-a-site).</span></span> <span data-ttu-id="28b93-112">За да премахнете напълно сайт с Powershell, вижте [Премахване-SPSite](https://docs.microsoft.com/sharepoint/manage-sites-in-new-admin-center#delete-a-site) cmdlet пример.</span><span class="sxs-lookup"><span data-stu-id="28b93-112">To completely remove a site with Powershell, see the [Remove-SPSite](https://docs.microsoft.com/sharepoint/manage-sites-in-new-admin-center#delete-a-site) cmdlet example.</span></span>
> - <span data-ttu-id="28b93-113">Някои потребители може да не успеете да създадете сайт.</span><span class="sxs-lookup"><span data-stu-id="28b93-113">Some users may not be able to create a site.</span></span> <span data-ttu-id="28b93-114">Вижте [управление на създаване на сайт в SharePoint Online](https://docs.microsoft.com/sharepoint/manage-site-creation).</span><span class="sxs-lookup"><span data-stu-id="28b93-114">See [Manage site creation in SharePoint Online](https://docs.microsoft.com/sharepoint/manage-site-creation).</span></span>
> - <span data-ttu-id="28b93-115">Това е възможно сайтът изглежда остана на **Създаване** повече от очакваното.</span><span class="sxs-lookup"><span data-stu-id="28b93-115">It's possible the site appears stuck at **Creating** longer than expected.</span></span> <span data-ttu-id="28b93-116">Ако повече от 24 часа са изминали от вас за първи път видях този проблем, моля влезте билет подкрепа.</span><span class="sxs-lookup"><span data-stu-id="28b93-116">If more than 24 hours have passed since you first saw this issue, please log a support ticket.</span></span> <span data-ttu-id="28b93-117">В много случаи ние вече работим върху решение.</span><span class="sxs-lookup"><span data-stu-id="28b93-117">In many cases, we're already working on a solution.</span></span> <span data-ttu-id="28b93-118">Моля, дайте ни най-малко 24 часа да завършите решение.</span><span class="sxs-lookup"><span data-stu-id="28b93-118">Please give us at least 24 hours to complete a solution.</span></span>
> - <span data-ttu-id="28b93-119">Ако трябва да създадете нов сайт на екип, който не съдържа Office 365 група,</span><span class="sxs-lookup"><span data-stu-id="28b93-119">If you need to create a new team site that doesn't include an Office 365 group,</span></span> 


