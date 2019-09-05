---
title: Добавяне на група към сайт на SharePoint
ms.author: pebaum
author: Techwriter40
manager: pamgreen
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: f7d730bf-0d6e-424c-970c-6137c71cb50b
ms.openlocfilehash: 423db4e5bbb85e75aee3548d5b6b46a64ebc6fa0
ms.sourcegitcommit: a65d196d00adb70045af5caca9828fe44b951f61
ms.translationtype: MT
ms.contentlocale: bg-BG
ms.lasthandoff: 09/04/2019
ms.locfileid: "36750509"
---
# <a name="issues-when-creating-or-group-connected-sites-in-sharepoint-online"></a><span data-ttu-id="c155c-102">Проблеми при създаване или групиране на свързани сайтове в SharePoint online</span><span class="sxs-lookup"><span data-stu-id="c155c-102">Issues when creating or group connected sites in SharePoint Online</span></span>

<span data-ttu-id="c155c-103">Има няколко често срещани проблеми при създаване или повторно създаване на група свързан сайт.</span><span class="sxs-lookup"><span data-stu-id="c155c-103">There are a couple of common issues encountered when creating or re-creating a group connected site.</span></span>

 <span data-ttu-id="c155c-104">Ако сте изтрили група и свързания с него сайт и искате да създадете друг сайт със същия URL адрес, ще трябва да премахнете окончателно предишния сайт.</span><span class="sxs-lookup"><span data-stu-id="c155c-104">If you have deleted a group and its connected site and wish to create another site with the same URL, you'll need to permanently remove the previous site.</span></span>

<span data-ttu-id="c155c-105">Изтегляй [обвивката за управление на](https://support.office.com/article/introduction-to-the-sharepoint-online-management-shell-c16941c3-19b4-4710-8056-34c034493429)</span><span class="sxs-lookup"><span data-stu-id="c155c-105">Download [SPO Management Shell](https://support.office.com/article/introduction-to-the-sharepoint-online-management-shell-c16941c3-19b4-4710-8056-34c034493429)</span></span>

 <span data-ttu-id="c155c-106">За повече информация за първи стъпки с PowerShell вижте [Първи стъпки с онлайн обвивката за управление на SharePoint](https://docs.microsoft.com/powershell/module/sharepoint-online/remove-sposite?view=sharepoint-ps)</span><span class="sxs-lookup"><span data-stu-id="c155c-106">For more info on getting started with powershell, see [Getting started with SharePoint Online Management Shell](https://docs.microsoft.com/powershell/module/sharepoint-online/remove-sposite?view=sharepoint-ps)</span></span>

<span data-ttu-id="c155c-107">Премахнете сайта от изтрити сайтове с помощта на кратката команда [Премахване-SPO](https://docs.microsoft.com/powershell/module/sharepoint-online/remove-sposite?view=sharepoint-ps)</span><span class="sxs-lookup"><span data-stu-id="c155c-107">Remove the Site from Deleted Sites using the [Remove-SPODeletedSite](https://docs.microsoft.com/powershell/module/sharepoint-online/remove-sposite?view=sharepoint-ps) powershell cmdlet.</span></span>

<span data-ttu-id="c155c-108">Ако създавате група свързан сайт и получите предупреждение друга група със същия псевдоним вече съществува, проверете съществуващите групи от [Office 365 от центъра за администриране](https://admin.microsoft.com/Adminportal/Home?source=applauncher#/groups).</span><span class="sxs-lookup"><span data-stu-id="c155c-108">If you're creating a group connected site and receive a warning Another group with the same alias already exists, check the existing groups from the [Office 365 from the Admin Center](https://admin.microsoft.com/Adminportal/Home?source=applauncher#/groups).</span></span> <span data-ttu-id="c155c-109">За да отстраните проблема, изтрийте съществуващата група, ако вече не е необходима или създайте сайта с различен псевдоним.</span><span class="sxs-lookup"><span data-stu-id="c155c-109">To resolve the issue, delete the existing group if it's no longer needed or create the site with a different alias assigned.</span></span>

<span data-ttu-id="c155c-110">Има различни начини за създаване и използване на модерни групи с SharePoint.</span><span class="sxs-lookup"><span data-stu-id="c155c-110">There are different ways to create and use modern groups with SharePoint.</span></span>

<span data-ttu-id="c155c-111">Можете да свържете съществуващи сайтове към група на Office 365.</span><span class="sxs-lookup"><span data-stu-id="c155c-111">You can connect existing sites to an Office 365 group.</span></span> <span data-ttu-id="c155c-112">За повече информация вижте [Свързване на Office 365 група с помощта на потребител на SharePoint интерлицето](https://docs.microsoft.com/sharepoint/dev/transform/modernize-connect-to-office365-group#connect-an-office-365-group-using-the-sharepoint-user-interface).</span><span class="sxs-lookup"><span data-stu-id="c155c-112">For more info, see [Connect an Office 365 group using the SharePoint user ineterface](https://docs.microsoft.com/sharepoint/dev/transform/modernize-connect-to-office365-group#connect-an-office-365-group-using-the-sharepoint-user-interface).</span></span>

<span data-ttu-id="c155c-113">За да създадете свързан сайт на Office 365 група, ще трябва да създадете екипен сайт.</span><span class="sxs-lookup"><span data-stu-id="c155c-113">To create an Office 365 group connected site, you'll need to create a Team Site.</span></span> <span data-ttu-id="c155c-114">За повече информация вижте [Създаване на екипен сайт в SharePoint](https://support.office.com/article/create-a-team-site-in-sharepoint-ef10c1e7-15f3-42a3-98aa-b5972711777d).</span><span class="sxs-lookup"><span data-stu-id="c155c-114">For more info, see [Create a team site in SharePoint](https://support.office.com/article/create-a-team-site-in-sharepoint-ef10c1e7-15f3-42a3-98aa-b5972711777d).</span></span>

