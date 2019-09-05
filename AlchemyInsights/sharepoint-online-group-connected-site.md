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
# <a name="issues-when-creating-or-group-connected-sites-in-sharepoint-online"></a>Проблеми при създаване или групиране на свързани сайтове в SharePoint online

Има няколко често срещани проблеми при създаване или повторно създаване на група свързан сайт.

 Ако сте изтрили група и свързания с него сайт и искате да създадете друг сайт със същия URL адрес, ще трябва да премахнете окончателно предишния сайт.

Изтегляй [обвивката за управление на](https://support.office.com/article/introduction-to-the-sharepoint-online-management-shell-c16941c3-19b4-4710-8056-34c034493429)

 За повече информация за първи стъпки с PowerShell вижте [Първи стъпки с онлайн обвивката за управление на SharePoint](https://docs.microsoft.com/powershell/module/sharepoint-online/remove-sposite?view=sharepoint-ps)

Премахнете сайта от изтрити сайтове с помощта на кратката команда [Премахване-SPO](https://docs.microsoft.com/powershell/module/sharepoint-online/remove-sposite?view=sharepoint-ps)

Ако създавате група свързан сайт и получите предупреждение друга група със същия псевдоним вече съществува, проверете съществуващите групи от [Office 365 от центъра за администриране](https://admin.microsoft.com/Adminportal/Home?source=applauncher#/groups). За да отстраните проблема, изтрийте съществуващата група, ако вече не е необходима или създайте сайта с различен псевдоним.

Има различни начини за създаване и използване на модерни групи с SharePoint.

Можете да свържете съществуващи сайтове към група на Office 365. За повече информация вижте [Свързване на Office 365 група с помощта на потребител на SharePoint интерлицето](https://docs.microsoft.com/sharepoint/dev/transform/modernize-connect-to-office365-group#connect-an-office-365-group-using-the-sharepoint-user-interface).

За да създадете свързан сайт на Office 365 група, ще трябва да създадете екипен сайт. За повече информация вижте [Създаване на екипен сайт в SharePoint](https://support.office.com/article/create-a-team-site-in-sharepoint-ef10c1e7-15f3-42a3-98aa-b5972711777d).

