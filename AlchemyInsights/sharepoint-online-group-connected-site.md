---
title: Добавяне на група към сайт на SharePoint
ms.author: pebaum
author: pebaum
manager: pamgreen
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: f7d730bf-0d6e-424c-970c-6137c71cb50b
ms.openlocfilehash: 9bec2f71465e43e1c3cba038e0e68949672ceb8a
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: bg-BG
ms.lasthandoff: 09/15/2020
ms.locfileid: "47771188"
---
# <a name="issues-when-creating-a-group-connected-site-in-sharepoint"></a><span data-ttu-id="21bc9-102">Проблеми при създаването на сайт, свързан с група в SharePoint</span><span class="sxs-lookup"><span data-stu-id="21bc9-102">Issues when creating a group connected site in SharePoint</span></span>

1. <span data-ttu-id="21bc9-103">Някои често срещани проблеми възникват при създаването или повторното създаване на сайт, свързан с група.</span><span class="sxs-lookup"><span data-stu-id="21bc9-103">Some common issues encountered when creating or re-creating a group connected site.</span></span>
<span data-ttu-id="21bc9-104">Ако сте изтрили група и свързания с нея сайт и искате да създадете друг сайт със същия URL адрес, ще трябва да премахнете завинаги предишния сайт.</span><span class="sxs-lookup"><span data-stu-id="21bc9-104">If you have deleted a group and its connected site and wish to create another site with the same URL, you'll need to permanently remove the previous site.</span></span>

   - <span data-ttu-id="21bc9-105">Изтегляне [на обвивката за управление на Спондж](https://support.office.com/article/introduction-to-the-sharepoint-online-management-shell-c16941c3-19b4-4710-8056-34c034493429)</span><span class="sxs-lookup"><span data-stu-id="21bc9-105">Download [SPO Management Shell](https://support.office.com/article/introduction-to-the-sharepoint-online-management-shell-c16941c3-19b4-4710-8056-34c034493429)</span></span>
   - <span data-ttu-id="21bc9-106">За повече информация относно първите стъпки с PowerShell вижте [Първи стъпки в обвивката за управление на SharePoint online](https://docs.microsoft.com/powershell/module/sharepoint-online/remove-sposite).</span><span class="sxs-lookup"><span data-stu-id="21bc9-106">For more info on getting started with Powershell, see [Getting started with SharePoint Online Management Shell](https://docs.microsoft.com/powershell/module/sharepoint-online/remove-sposite).</span></span>
   - <span data-ttu-id="21bc9-107">Премахнете сайта от изтрити сайтове с помощта на кратката команда [Remove-SPODeletedSite](https://docs.microsoft.com/powershell/module/sharepoint-online/remove-sposite?view=sharepoint-ps) PowerShell.</span><span class="sxs-lookup"><span data-stu-id="21bc9-107">Remove the Site from Deleted Sites using the [Remove-SPODeletedSite](https://docs.microsoft.com/powershell/module/sharepoint-online/remove-sposite?view=sharepoint-ps) Powershell cmdlet.</span></span> <span data-ttu-id="21bc9-108">За да изтриете окончателно сайтовете на групи, се изисква PowerShell.</span><span class="sxs-lookup"><span data-stu-id="21bc9-108">Powershell is required to permanently delete group sites.</span></span>

1. <span data-ttu-id="21bc9-109">Ако създавате сайт, свързан с група, и получавате предупреждение: **друга група със същия псевдоним вече съществува**, проверете съществуващите групи от центъра за администриране на [Microsoft 365](https://admin.microsoft.com/AdminPortal/Home#/groups).</span><span class="sxs-lookup"><span data-stu-id="21bc9-109">If you're creating a group connected site and receive a warning: **Another group with the same alias already exists**, check the existing groups from the [Microsoft 365 admin center](https://admin.microsoft.com/AdminPortal/Home#/groups).</span></span> <span data-ttu-id="21bc9-110">За да отстраните проблема, изтрийте съществуващата група, ако вече не е необходима или създайте сайта с различен присвоен псевдоним.</span><span class="sxs-lookup"><span data-stu-id="21bc9-110">To resolve the issue, delete the existing group if it's no longer needed or create the site with a different alias assigned.</span></span>

1. <span data-ttu-id="21bc9-111">Има различни начини за създаване и използване на модерни групи с SharePoint.</span><span class="sxs-lookup"><span data-stu-id="21bc9-111">There are different ways to create and use modern groups with SharePoint.</span></span>

   - <span data-ttu-id="21bc9-112">Можете да свържете съществуващи сайтове към група на Microsoft 365.</span><span class="sxs-lookup"><span data-stu-id="21bc9-112">You can connect existing sites to a Microsoft 365 group.</span></span> <span data-ttu-id="21bc9-113">За повече информация вижте [Свързване на група на Microsoft 365 чрез потребителския интерфейс на SharePoint](https://docs.microsoft.com/sharepoint/dev/transform/modernize-connect-to-office365-group#connect-an-office-365-group-using-the-sharepoint-user-interface).</span><span class="sxs-lookup"><span data-stu-id="21bc9-113">For more info, see [Connect a Microsoft 365 group using the SharePoint user interface](https://docs.microsoft.com/sharepoint/dev/transform/modernize-connect-to-office365-group#connect-an-office-365-group-using-the-sharepoint-user-interface).</span></span>
   - <span data-ttu-id="21bc9-114">За да създадете сайт на Microsoft 365, свързан с група, ще трябва да създадете [екипен сайт](https://admin.microsoft.com/sharepoint).</span><span class="sxs-lookup"><span data-stu-id="21bc9-114">To create a Microsoft 365 group connected site, you'll need to create a [Team Site](https://admin.microsoft.com/sharepoint).</span></span>
