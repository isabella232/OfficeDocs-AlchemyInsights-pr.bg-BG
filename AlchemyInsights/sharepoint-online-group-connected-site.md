---
title: Добавяне на група към SharePoint сайт
ms.author: pebaum
author: pebaum
manager: pamgreen
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "5200004"
- "5766"
ms.assetid: f7d730bf-0d6e-424c-970c-6137c71cb50b
ms.openlocfilehash: 396efbf9772b5398427a4fcc76e104fa95820af6
ms.sourcegitcommit: 86c95d3f0f268e500b3732243ca85a650b2e7b8f
ms.translationtype: MT
ms.contentlocale: bg-BG
ms.lasthandoff: 07/22/2021
ms.locfileid: "53532208"
---
# <a name="common-issues-when-creating-a-group-connected-site-in-sharepoint"></a>Често срещани проблеми при създаване на свързан сайт на група в SharePoint

1. Ако сте изтрили група и нейния свързан сайт и искате да създадете друг сайт със същия URL адрес, ще трябва окончателно да премахнете предишния сайт.

   - Изтегляне на [обвивката за управление на SPO](https://support.office.com/article/introduction-to-the-sharepoint-online-management-shell-c16941c3-19b4-4710-8056-34c034493429)
   - За повече информация относно първи стъпки с Powershell вижте Първи стъпки в SharePoint [обвивката за онлайн управление.](/powershell/module/sharepoint-online/remove-sposite)
   - Премахване на сайта от изтрити сайтове с помощта [на кратката команда Remove-SPODeletedSite](/powershell/module/sharepoint-online/remove-sposite?view=sharepoint-ps) Powershell. Powershell е необходим за окончателно изтриване на сайтове на групи.

1. Ако създавате свързан сайт на група и получавате **предупреждение:** Вече съществува друга група със същия псевдоним , проверете съществуващите групи [от Център за администриране на Microsoft 365](https://admin.microsoft.com/AdminPortal/Home#/groups). За да отстраните проблема, изтрийте съществуващата група, ако вече не е необходима, или създайте сайта с различен псевдоним.

1. Има различни начини за създаване и използване на модерни групи с SharePoint.

   - Можете да свържете съществуващи сайтове към Microsoft 365 група. За повече информация [вж. Свързване група Microsoft 365 с помощта на потребителския интерфейс SharePoint приложението](/sharepoint/dev/transform/modernize-connect-to-office365-group#connect-an-office-365-group-using-the-sharepoint-user-interface).
   - За да създадете Microsoft 365 свързан сайт на група, ще трябва да създадете [екипен сайт](https://admin.microsoft.com/sharepoint).
