---
title: Добавяне на група към SharePoint сайт
ms.author: kirks
author: Techwriter40
manager: pamgreen
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: f7d730bf-0d6e-424c-970c-6137c71cb50b
ms.openlocfilehash: f0126f7f753275e9bbf8c3a09a6af5faf9a27862
ms.sourcegitcommit: 4b7e478ce700c0b781efec3857ac4dce5bdf00c6
ms.translationtype: MT
ms.contentlocale: bg-BG
ms.lasthandoff: 06/07/2019
ms.locfileid: "34758720"
---
# <a name="create-group-connected-site-in-sharepoint-online"></a><span data-ttu-id="7a74f-102">Създаване на група свързани сайт в SharePoint Online</span><span class="sxs-lookup"><span data-stu-id="7a74f-102">Create group connected site in SharePoint Online</span></span>

<span data-ttu-id="7a74f-103">Има няколко общи проблеми, срещани при създаване или повторно създаване група свързан сайт.</span><span class="sxs-lookup"><span data-stu-id="7a74f-103">There are a couple of common issues encountered when creating or re-creating a group connected site.</span></span>

 <span data-ttu-id="7a74f-104">Ако сте изтрили група и нейните свързани сайт и искате да създадете друг сайт със същия URL адрес, трябва да премахнете завинаги предишният сайт.</span><span class="sxs-lookup"><span data-stu-id="7a74f-104">If you have deleted a group and its connected site and wish to create another site with the same URL, you'll need to permanently remove the previous site.</span></span>

<span data-ttu-id="7a74f-105">Изтегляне [SPO управление Шел](https://support.office.com/article/introduction-to-the-sharepoint-online-management-shell-c16941c3-19b4-4710-8056-34c034493429)</span><span class="sxs-lookup"><span data-stu-id="7a74f-105">Download [SPO Management Shell](https://support.office.com/article/introduction-to-the-sharepoint-online-management-shell-c16941c3-19b4-4710-8056-34c034493429)</span></span>

 <span data-ttu-id="7a74f-106">За повече информация за първи стъпки с powershell вижте [Първи стъпки с SharePoint онлайн управление Шел](https://docs.microsoft.com/powershell/module/sharepoint-online/remove-sposite?view=sharepoint-ps)</span><span class="sxs-lookup"><span data-stu-id="7a74f-106">For more info on getting started with powershell, see [Getting started with SharePoint Online Management Shell](https://docs.microsoft.com/powershell/module/sharepoint-online/remove-sposite?view=sharepoint-ps)</span></span>

<span data-ttu-id="7a74f-107">Премахване на сайт от изтрити сайтове с помощта на [Премахване-SPODeletedSite](https://docs.microsoft.com/powershell/module/sharepoint-online/remove-sposite?view=sharepoint-ps) powershell cmdlet.</span><span class="sxs-lookup"><span data-stu-id="7a74f-107">Remove the Site from Deleted Sites using the [Remove-SPODeletedSite](https://docs.microsoft.com/powershell/module/sharepoint-online/remove-sposite?view=sharepoint-ps) powershell cmdlet.</span></span>

<span data-ttu-id="7a74f-108">Ако сте създаване на група свързани сайт и да получите предупреждение вече съществува друга група със същия псевдоним, проверете съществуващите групи от [Office 365 от центъра за администрация на](https://admin.microsoft.com/Adminportal/Home?source=applauncher#/groups).</span><span class="sxs-lookup"><span data-stu-id="7a74f-108">If you're creating a group connected site and receive a warning Another group with the same alias already exists, check the existing groups from the [Office 365 from the Admin Center](https://admin.microsoft.com/Adminportal/Home?source=applauncher#/groups).</span></span> <span data-ttu-id="7a74f-109">За разрешаване на проблема, изтрийте съществуващата група, ако вече не е необходимо или създадете сайт с друг псевдоним присвоени.</span><span class="sxs-lookup"><span data-stu-id="7a74f-109">To resolve the issue, delete the existing group if it's no longer needed or create the site with a different alias assigned.</span></span>

<span data-ttu-id="7a74f-110">Има различни начини за създаване и използване на съвременни групи с SharePoint.</span><span class="sxs-lookup"><span data-stu-id="7a74f-110">There are different ways to create and use modern groups with SharePoint.</span></span>

<span data-ttu-id="7a74f-111">Можете да се свържете съществуващи сайтове на Office 365 група.</span><span class="sxs-lookup"><span data-stu-id="7a74f-111">You can connect existing sites to an Office 365 group.</span></span> <span data-ttu-id="7a74f-112">За повече информация вижте [Свързване на Office 365 група, като използвате SharePoint потребител ineterface](https://docs.microsoft.com/sharepoint/dev/transform/modernize-connect-to-office365-group#connect-an-office-365-group-using-the-sharepoint-user-interface).</span><span class="sxs-lookup"><span data-stu-id="7a74f-112">For more info, see [Connect an Office 365 group using the SharePoint user ineterface](https://docs.microsoft.com/sharepoint/dev/transform/modernize-connect-to-office365-group#connect-an-office-365-group-using-the-sharepoint-user-interface).</span></span>

<span data-ttu-id="7a74f-113">За да създадете свързан сайт за група на Office 365, трябва да създадете сайт на екип.</span><span class="sxs-lookup"><span data-stu-id="7a74f-113">To create an Office 365 group connected site, you'll need to create a Team Site.</span></span> <span data-ttu-id="7a74f-114">За повече информация вижте [Създаване на екип сайт в SharePoint](https://support.office.com/article/create-a-team-site-in-sharepoint-ef10c1e7-15f3-42a3-98aa-b5972711777d).</span><span class="sxs-lookup"><span data-stu-id="7a74f-114">For more info, see [Create a team site in SharePoint](https://support.office.com/article/create-a-team-site-in-sharepoint-ef10c1e7-15f3-42a3-98aa-b5972711777d).</span></span>

