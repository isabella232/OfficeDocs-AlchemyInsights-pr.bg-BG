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
ms.openlocfilehash: 6aea12d44a44a3e11eaf3fb1bd47ff3e9dbfd9e7
ms.sourcegitcommit: 1d98db8acb9959aba3b5e308a567ade6b62da56c
ms.translationtype: MT
ms.contentlocale: bg-BG
ms.lasthandoff: 08/22/2019
ms.locfileid: "36507836"
---
# <a name="issues-when-creating-or-group-connected-sites-in-sharepoint-online"></a>Проблеми при създаването или група свързани обекти в SharePoint Online

Има няколко общи проблеми, срещани при създаване или повторно създаване група свързан сайт.

 Ако сте изтрили група и нейните свързани сайт и искате да създадете друг сайт със същия URL адрес, трябва да премахнете завинаги предишният сайт.

Изтегляне [SPO управление Шел](https://support.office.com/article/introduction-to-the-sharepoint-online-management-shell-c16941c3-19b4-4710-8056-34c034493429)

 За повече информация за първи стъпки с powershell вижте [Първи стъпки с SharePoint онлайн управление Шел](https://docs.microsoft.com/powershell/module/sharepoint-online/remove-sposite?view=sharepoint-ps)

Премахване на сайт от изтрити сайтове с помощта на [Премахване-SPODeletedSite](https://docs.microsoft.com/powershell/module/sharepoint-online/remove-sposite?view=sharepoint-ps) powershell cmdlet.

Ако сте създаване на група свързани сайт и да получите предупреждение вече съществува друга група със същия псевдоним, проверете съществуващите групи от [Office 365 от центъра за администрация на](https://admin.microsoft.com/Adminportal/Home?source=applauncher#/groups). За разрешаване на проблема, изтрийте съществуващата група, ако вече не е необходимо или създадете сайт с друг псевдоним присвоени.

Има различни начини за създаване и използване на съвременни групи с SharePoint.

Можете да се свържете съществуващи сайтове на Office 365 група. За повече информация вижте [Свързване на Office 365 група, като използвате SharePoint потребител ineterface](https://docs.microsoft.com/sharepoint/dev/transform/modernize-connect-to-office365-group#connect-an-office-365-group-using-the-sharepoint-user-interface).

За да създадете свързан сайт за група на Office 365, трябва да създадете сайт на екип. За повече информация вижте [Създаване на екип сайт в SharePoint](https://support.office.com/article/create-a-team-site-in-sharepoint-ef10c1e7-15f3-42a3-98aa-b5972711777d).

