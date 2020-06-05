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
# <a name="issues-when-creating-a-group-connected-site-in-sharepoint"></a>Проблеми при създаване на група свързан сайт в SharePoint

1. Някои често срещани проблеми се срещат при създаване или повторно създаване на свързан сайт на група.
Ако сте изтрили група и свързания с нея сайт и искате да създадете друг сайт със същия URL адрес, ще трябва да премахнете за постоянно предишния сайт.

   - Изтегляне на [SPO обвивка за управление](https://support.office.com/article/introduction-to-the-sharepoint-online-management-shell-c16941c3-19b4-4710-8056-34c034493429)
   - За повече информация относно първи стъпки с PowerShell вижте [Първи стъпки с Обвивката за управление на SharePoint Online](https://docs.microsoft.com/powershell/module/sharepoint-online/remove-sposite).
   - Премахнете сайта от изтрити сайтове с помощта на кратката команда [Remove-SPODeletedSite](https://docs.microsoft.com/powershell/module/sharepoint-online/remove-sposite?view=sharepoint-ps) PowerShell. Powershell е необходимо да изтриете за постоянно групови сайтове.

1. Ако създавате свързан към група сайт и получите предупреждение: **Друга група със същия псевдоним вече съществува**, проверете съществуващите групи от центъра за администриране на Microsoft [365](https://admin.microsoft.com/AdminPortal/Home#/groups). За да разрешите проблема, изтрийте съществуващата група, ако вече не е необходима или създаване на сайта с друг псевдоним присвоен.

1. Има различни начини за създаване и използване на съвременни групи с SharePoint.

   - Можете да свържете съществуващи сайтове към microsoft 365 група. За повече информация вижте [Свързване на microsoft 365 група с помощта на потребителския интерфейс на SharePoint](https://docs.microsoft.com/sharepoint/dev/transform/modernize-connect-to-office365-group#connect-an-office-365-group-using-the-sharepoint-user-interface).
   - За да създадете свързан сайт на група на Microsoft 365, трябва да създадете [екипен сайт](https://admin.microsoft.com/sharepoint).
