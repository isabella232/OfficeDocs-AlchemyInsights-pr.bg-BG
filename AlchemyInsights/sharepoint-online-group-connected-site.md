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
# <a name="issues-when-creating-a-group-connected-site-in-sharepoint"></a>Проблеми при създаването на сайт, свързан с група в SharePoint

1. Някои често срещани проблеми възникват при създаването или повторното създаване на сайт, свързан с група.
Ако сте изтрили група и свързания с нея сайт и искате да създадете друг сайт със същия URL адрес, ще трябва да премахнете завинаги предишния сайт.

   - Изтегляне [на обвивката за управление на Спондж](https://support.office.com/article/introduction-to-the-sharepoint-online-management-shell-c16941c3-19b4-4710-8056-34c034493429)
   - За повече информация относно първите стъпки с PowerShell вижте [Първи стъпки в обвивката за управление на SharePoint online](https://docs.microsoft.com/powershell/module/sharepoint-online/remove-sposite).
   - Премахнете сайта от изтрити сайтове с помощта на кратката команда [Remove-SPODeletedSite](https://docs.microsoft.com/powershell/module/sharepoint-online/remove-sposite?view=sharepoint-ps) PowerShell. За да изтриете окончателно сайтовете на групи, се изисква PowerShell.

1. Ако създавате сайт, свързан с група, и получавате предупреждение: **друга група със същия псевдоним вече съществува**, проверете съществуващите групи от центъра за администриране на [Microsoft 365](https://admin.microsoft.com/AdminPortal/Home#/groups). За да отстраните проблема, изтрийте съществуващата група, ако вече не е необходима или създайте сайта с различен присвоен псевдоним.

1. Има различни начини за създаване и използване на модерни групи с SharePoint.

   - Можете да свържете съществуващи сайтове към група на Microsoft 365. За повече информация вижте [Свързване на група на Microsoft 365 чрез потребителския интерфейс на SharePoint](https://docs.microsoft.com/sharepoint/dev/transform/modernize-connect-to-office365-group#connect-an-office-365-group-using-the-sharepoint-user-interface).
   - За да създадете сайт на Microsoft 365, свързан с група, ще трябва да създадете [екипен сайт](https://admin.microsoft.com/sharepoint).
