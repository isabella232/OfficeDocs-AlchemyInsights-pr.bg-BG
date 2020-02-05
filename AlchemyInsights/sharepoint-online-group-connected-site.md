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
# <a name="issues-when-creating-a-group-connected-site-in-sharepoint"></a>Проблеми при създаване на група свързан сайт в SharePoint

1. Някои често срещани проблеми, възникнали при създаване или повторно създаване на свързан към групата сайт.
Ако сте изтрили група и свързания й сайт и искате да създадете друг сайт със същия URL адрес, ще трябва да премахнете за постоянно предишния сайт.

   - Изтегляне [на обвивката за управление на SPO](https://support.office.com/article/introduction-to-the-sharepoint-online-management-shell-c16941c3-19b4-4710-8056-34c034493429)
   - За повече информация за първи стъпки с PowerShell вижте Първи стъпки с обвивката за [онлайн управление на SharePoint](https://docs.microsoft.com/powershell/module/sharepoint-online/remove-sposite).
   - Премахване на сайта от изтрити сайтове с помощта на [Командата Remove-SPODeletedСайт](https://docs.microsoft.com/powershell/module/sharepoint-online/remove-sposite?view=sharepoint-ps) Powershell. PowerShell е необходимо за окончателно изтриване на групови театри.

1. Ако създавате група свързан сайт и получавате предупреждение: **друга група със същия псевдоним вече съществува**, проверете съществуващите групи от Office [365 от центъра за администриране](https://admin.microsoft.com/AdminPortal/Home#/groups). За да разрешите проблема, изтрийте съществуващата група, ако вече не е необходимо или създайте сайта с различен псевдоним присвоен.

1. Има различни начини за създаване и използване на съвременни групи с SharePoint.

   - Можете да свържете съществуващи театри към група на Office 365. За повече информация вижте [Свързване на група на Office 365 с помощта на потребителския интерфейс на SharePoint](https://docs.microsoft.com/sharepoint/dev/transform/modernize-connect-to-office365-group#connect-an-office-365-group-using-the-sharepoint-user-interface).
   - За да създадете сайт, свързан с група на Office 365, трябва да създадете [екипен сайт](https://admin.microsoft.com/sharepoint).
