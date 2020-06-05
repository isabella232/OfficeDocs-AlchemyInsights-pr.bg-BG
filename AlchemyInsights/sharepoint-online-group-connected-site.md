---
title: Добавяне на група към сайт на SharePoint
ms.author: pebaum
author: pebaum
manager: pamgreen
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: f7d730bf-0d6e-424c-970c-6137c71cb50b
ms.openlocfilehash: 5dab9fce935936898927afd55f8f6e9260249157
ms.sourcegitcommit: f28dafa0f727870038f72bc904da926daf4ec07b
ms.translationtype: MT
ms.contentlocale: bg-BG
ms.lasthandoff: 06/05/2020
ms.locfileid: "44582800"
---
# <a name="issues-when-creating-a-group-connected-site-in-sharepoint"></a><span data-ttu-id="cdf2f-102">Проблеми при създаване на група свързан сайт в SharePoint</span><span class="sxs-lookup"><span data-stu-id="cdf2f-102">Issues when creating a group connected site in SharePoint</span></span>

1. <span data-ttu-id="cdf2f-103">Някои често срещани проблеми се срещат при създаване или повторно създаване на свързан сайт на група.</span><span class="sxs-lookup"><span data-stu-id="cdf2f-103">Some common issues encountered when creating or re-creating a group connected site.</span></span>
<span data-ttu-id="cdf2f-104">Ако сте изтрили група и свързания с нея сайт и искате да създадете друг сайт със същия URL адрес, ще трябва да премахнете за постоянно предишния сайт.</span><span class="sxs-lookup"><span data-stu-id="cdf2f-104">If you have deleted a group and its connected site and wish to create another site with the same URL, you'll need to permanently remove the previous site.</span></span>

   - <span data-ttu-id="cdf2f-105">Изтегляне на [SPO обвивка за управление](https://support.office.com/article/introduction-to-the-sharepoint-online-management-shell-c16941c3-19b4-4710-8056-34c034493429)</span><span class="sxs-lookup"><span data-stu-id="cdf2f-105">Download [SPO Management Shell](https://support.office.com/article/introduction-to-the-sharepoint-online-management-shell-c16941c3-19b4-4710-8056-34c034493429)</span></span>
   - <span data-ttu-id="cdf2f-106">За повече информация относно първи стъпки с PowerShell вижте [Първи стъпки с Обвивката за управление на SharePoint Online](https://docs.microsoft.com/powershell/module/sharepoint-online/remove-sposite).</span><span class="sxs-lookup"><span data-stu-id="cdf2f-106">For more info on getting started with Powershell, see [Getting started with SharePoint Online Management Shell](https://docs.microsoft.com/powershell/module/sharepoint-online/remove-sposite).</span></span>
   - <span data-ttu-id="cdf2f-107">Премахнете сайта от изтрити сайтове с помощта на кратката команда [Remove-SPODeletedSite](https://docs.microsoft.com/powershell/module/sharepoint-online/remove-sposite?view=sharepoint-ps) PowerShell.</span><span class="sxs-lookup"><span data-stu-id="cdf2f-107">Remove the Site from Deleted Sites using the [Remove-SPODeletedSite](https://docs.microsoft.com/powershell/module/sharepoint-online/remove-sposite?view=sharepoint-ps) Powershell cmdlet.</span></span> <span data-ttu-id="cdf2f-108">Powershell е необходимо да изтриете за постоянно групови сайтове.</span><span class="sxs-lookup"><span data-stu-id="cdf2f-108">Powershell is required to permanently delete group sites.</span></span>

1. <span data-ttu-id="cdf2f-109">Ако създавате свързан към група сайт и получите предупреждение: **Друга група със същия псевдоним вече съществува**, проверете съществуващите групи от центъра за администриране на Microsoft [365](https://admin.microsoft.com/AdminPortal/Home#/groups).</span><span class="sxs-lookup"><span data-stu-id="cdf2f-109">If you're creating a group connected site and receive a warning: **Another group with the same alias already exists**, check the existing groups from the [Microsoft 365 admin center](https://admin.microsoft.com/AdminPortal/Home#/groups).</span></span> <span data-ttu-id="cdf2f-110">За да разрешите проблема, изтрийте съществуващата група, ако вече не е необходима или създаване на сайта с друг псевдоним присвоен.</span><span class="sxs-lookup"><span data-stu-id="cdf2f-110">To resolve the issue, delete the existing group if it's no longer needed or create the site with a different alias assigned.</span></span>

1. <span data-ttu-id="cdf2f-111">Има различни начини за създаване и използване на съвременни групи с SharePoint.</span><span class="sxs-lookup"><span data-stu-id="cdf2f-111">There are different ways to create and use modern groups with SharePoint.</span></span>

   - <span data-ttu-id="cdf2f-112">Можете да свържете съществуващи сайтове към microsoft 365 група.</span><span class="sxs-lookup"><span data-stu-id="cdf2f-112">You can connect existing sites to a Microsoft 365 group.</span></span> <span data-ttu-id="cdf2f-113">За повече информация вижте [Свързване на microsoft 365 група с помощта на потребителския интерфейс на SharePoint](https://docs.microsoft.com/sharepoint/dev/transform/modernize-connect-to-office365-group#connect-an-office-365-group-using-the-sharepoint-user-interface).</span><span class="sxs-lookup"><span data-stu-id="cdf2f-113">For more info, see [Connect a Microsoft 365 group using the SharePoint user interface](https://docs.microsoft.com/sharepoint/dev/transform/modernize-connect-to-office365-group#connect-an-office-365-group-using-the-sharepoint-user-interface).</span></span>
   - <span data-ttu-id="cdf2f-114">За да създадете свързан сайт на група на Microsoft 365, трябва да създадете [екипен сайт](https://admin.microsoft.com/sharepoint).</span><span class="sxs-lookup"><span data-stu-id="cdf2f-114">To create a Microsoft 365 group connected site, you'll need to create a [Team Site](https://admin.microsoft.com/sharepoint).</span></span>
