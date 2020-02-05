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
ms.openlocfilehash: e7bfabe1555bb94e915f8544d460deecce6171be
ms.sourcegitcommit: 317eeed39c7777a922442992d67733726c41d9e1
ms.translationtype: MT
ms.contentlocale: bg-BG
ms.lasthandoff: 02/04/2020
ms.locfileid: "41770340"
---
# <a name="issues-when-creating-a-group-connected-site-in-sharepoint"></a><span data-ttu-id="32d1b-102">Проблеми при създаване на група свързан сайт в SharePoint</span><span class="sxs-lookup"><span data-stu-id="32d1b-102">Issues when creating a group connected site in SharePoint</span></span>

1. <span data-ttu-id="32d1b-103">Някои често срещани проблеми, възникнали при създаване или повторно създаване на свързан към групата сайт.</span><span class="sxs-lookup"><span data-stu-id="32d1b-103">Some common issues encountered when creating or re-creating a group connected site.</span></span>
<span data-ttu-id="32d1b-104">Ако сте изтрили група и свързания й сайт и искате да създадете друг сайт със същия URL адрес, ще трябва да премахнете за постоянно предишния сайт.</span><span class="sxs-lookup"><span data-stu-id="32d1b-104">If you have deleted a group and its connected site and wish to create another site with the same URL, you'll need to permanently remove the previous site.</span></span>

   - <span data-ttu-id="32d1b-105">Изтегляне [на обвивката за управление на SPO](https://support.office.com/article/introduction-to-the-sharepoint-online-management-shell-c16941c3-19b4-4710-8056-34c034493429)</span><span class="sxs-lookup"><span data-stu-id="32d1b-105">Download [SPO Management Shell](https://support.office.com/article/introduction-to-the-sharepoint-online-management-shell-c16941c3-19b4-4710-8056-34c034493429)</span></span>
   - <span data-ttu-id="32d1b-106">За повече информация за първи стъпки с PowerShell вижте Първи стъпки с обвивката за [онлайн управление на SharePoint](https://docs.microsoft.com/powershell/module/sharepoint-online/remove-sposite).</span><span class="sxs-lookup"><span data-stu-id="32d1b-106">For more info on getting started with Powershell, see [Getting started with SharePoint Online Management Shell](https://docs.microsoft.com/powershell/module/sharepoint-online/remove-sposite).</span></span>
   - <span data-ttu-id="32d1b-107">Премахване на сайта от изтрити сайтове с помощта на [Командата Remove-SPODeletedСайт](https://docs.microsoft.com/powershell/module/sharepoint-online/remove-sposite?view=sharepoint-ps) Powershell.</span><span class="sxs-lookup"><span data-stu-id="32d1b-107">Remove the Site from Deleted Sites using the [Remove-SPODeletedSite](https://docs.microsoft.com/powershell/module/sharepoint-online/remove-sposite?view=sharepoint-ps) Powershell cmdlet.</span></span> <span data-ttu-id="32d1b-108">PowerShell е необходимо за окончателно изтриване на групови театри.</span><span class="sxs-lookup"><span data-stu-id="32d1b-108">Powershell is required to permanently delete group sites.</span></span>

1. <span data-ttu-id="32d1b-109">Ако създавате група свързан сайт и получавате предупреждение: **друга група със същия псевдоним вече съществува**, проверете съществуващите групи от Office [365 от центъра за администриране](https://admin.microsoft.com/AdminPortal/Home#/groups).</span><span class="sxs-lookup"><span data-stu-id="32d1b-109">If you're creating a group connected site and receive a warning: **Another group with the same alias already exists**, check the existing groups from the [Office 365 from the Admin Center](https://admin.microsoft.com/AdminPortal/Home#/groups).</span></span> <span data-ttu-id="32d1b-110">За да разрешите проблема, изтрийте съществуващата група, ако вече не е необходимо или създайте сайта с различен псевдоним присвоен.</span><span class="sxs-lookup"><span data-stu-id="32d1b-110">To resolve the issue, delete the existing group if it's no longer needed or create the site with a different alias assigned.</span></span>

1. <span data-ttu-id="32d1b-111">Има различни начини за създаване и използване на съвременни групи с SharePoint.</span><span class="sxs-lookup"><span data-stu-id="32d1b-111">There are different ways to create and use modern groups with SharePoint.</span></span>

   - <span data-ttu-id="32d1b-112">Можете да свържете съществуващи театри към група на Office 365.</span><span class="sxs-lookup"><span data-stu-id="32d1b-112">You can connect existing sites to an Office 365 group.</span></span> <span data-ttu-id="32d1b-113">За повече информация вижте [Свързване на група на Office 365 с помощта на потребителския интерфейс на SharePoint](https://docs.microsoft.com/sharepoint/dev/transform/modernize-connect-to-office365-group#connect-an-office-365-group-using-the-sharepoint-user-interface).</span><span class="sxs-lookup"><span data-stu-id="32d1b-113">For more info, see [Connect an Office 365 group using the SharePoint user interface](https://docs.microsoft.com/sharepoint/dev/transform/modernize-connect-to-office365-group#connect-an-office-365-group-using-the-sharepoint-user-interface).</span></span>
   - <span data-ttu-id="32d1b-114">За да създадете сайт, свързан с група на Office 365, трябва да създадете [екипен сайт](https://admin.microsoft.com/sharepoint).</span><span class="sxs-lookup"><span data-stu-id="32d1b-114">To create an Office 365 group connected site, you'll need to create a [Team Site](https://admin.microsoft.com/sharepoint).</span></span>
