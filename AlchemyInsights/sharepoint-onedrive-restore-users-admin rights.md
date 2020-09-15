---
title: Отстраняване на неизправности при отказан достъп на съобщения до сайтовете на OneDrive за бизнеса
ms.author: pebaum
author: pebaum
manager: pamgreen
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.assetid: cebb7a4a-33e1-474e-a5d0-dbd02a80b1e9
ms.openlocfilehash: 9001cf0b7d9f1f05a2ecedca2c3137dd1b8a1c38
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: bg-BG
ms.lasthandoff: 09/14/2020
ms.locfileid: "47670605"
---
# <a name="troubleshooting-access-denied-messages-to-onedrive-for-business-sites"></a>Отстраняване на неизправности при отказан достъп на съобщения до сайтовете на OneDrive за бизнеса

Този проблем най-често се случва, когато потребителят бъде изтрит и пресъздаден със същото основно потребителско име (UPN). Новият акаунт се създава с помощта на различна стойност на PUID (уникален ИД за Passport). Когато потребителят се опитва да получи достъп до колекция от сайтове или техния OneDrive, потребителят има неправилни PUID. Вторият сценарий включва синхронизирането на справочен указател с организационната единица за Active Directory (OU). Ако потребителите вече са влезли в SharePoint, а след това бъдат преместени в друга ОЕ и да се синхронизират с SharePoint, може да изпитате този проблем.

1. За да отстраните този проблем, трябва да възстановите първоначалния UPN със стъпките в статията [възстановяване на потребител в Microsoft 365](https://docs.microsoft.com/microsoft-365/admin/add-users/restore-user).
2. Ако не можете да възстановите първоначалния потребител, трябва да премахнете старият потребител от сайта на OneDrive, като използвате тези стъпки, за да [премахнете потребителя от списъка с информация за потребителите](). 
3. След като това приключи, можете да проверите дали потребителят има администраторски права за сайта на OneDrive, като следвате стъпките за [Добавяне на администратор за onedrive на потребителя](https://docs.microsoft.com/sharepoint/manage-user-profiles) .

За повече информация относно нивата на разрешение вижте статията, [запознаване с нивата на разрешение в SharePoint](https://docs.microsoft.com/sharepoint/understanding-permission-levels).
