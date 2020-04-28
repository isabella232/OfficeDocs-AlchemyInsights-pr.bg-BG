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
ms.openlocfilehash: 8ef33cbd44b01deaf0e45813d019f7696ef5def0
ms.sourcegitcommit: 286000b588adef1bbbb28337a9d9e087ec783fa2
ms.translationtype: MT
ms.contentlocale: bg-BG
ms.lasthandoff: 04/27/2020
ms.locfileid: "43912955"
---
# <a name="issues-when-creating-a-group-connected-site-in-sharepoint"></a>Проблеми при създаване на група свързан сайт в SharePoint

1. Някои често срещани проблеми при създаване или повторно създаване на група свързан сайт.
Ако сте изтрили група и свързания сайт и искате да създадете друг сайт със същия URL адрес, ще трябва да премахнете за постоянно предишния сайт.

   - Изтегляне [на обвивката за управление на SPO](https://support.office.com/article/introduction-to-the-sharepoint-online-management-shell-c16941c3-19b4-4710-8056-34c034493429)
   - За повече информация за първи стъпки с Powershell вижте [Първи стъпки с онлайн обвивката за управление на SharePoint](https://docs.microsoft.com/powershell/module/sharepoint-online/remove-sposite).
   - Премахване на сайта от изтрити сайтове с помощта на [Remove SPOИзтритиdСайт](https://docs.microsoft.com/powershell/module/sharepoint-online/remove-sposite?view=sharepoint-ps) PowerShell команда. Powershell е необходимо за постоянно изтриване на групови сайтове.

1. Ако създавате група свързан сайт и получавате предупреждение: **Вече съществува друга група със същия псевдоним**, проверете съществуващите групи от Център за администриране на Microsoft [365](https://admin.microsoft.com/AdminPortal/Home#/groups). За да разрешите проблема, изтрийте съществуваща група, ако вече не е необходимо или създайте сайта с друг псевдоним.

1. Има различни начини за създаване и използване на съвременни групи с SharePoint.

   - Можете да свържете съществуващи сайтове към група на Microsoft 365. За повече информация вижте [Свързване на група на Microsoft 365 с помощта на потребителския интерфейс на SharePoint](https://docs.microsoft.com/sharepoint/dev/transform/modernize-connect-to-office365-group#connect-an-office-365-group-using-the-sharepoint-user-interface).
   - За да създадете свързан сайт на Група на Microsoft 365, трябва да създадете [екипен сайт](https://admin.microsoft.com/sharepoint).
