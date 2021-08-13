---
title: Отстраняване на неизправности с отказан достъп до OneDrive за бизнеса сайтове
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
ms.openlocfilehash: fc4a2bd7dcc74f5f05e8b709e4bc3eac6ed445d6e2ea9ede698abbc8667723ce
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: bg-BG
ms.lasthandoff: 08/05/2021
ms.locfileid: "53957782"
---
# <a name="troubleshooting-access-denied-messages-to-onedrive-for-business-sites"></a>Отстраняване на неизправности с отказан достъп до OneDrive за бизнеса сайтове

Този проблем най-често възниква, когато потребител бъде изтрит и създаден отново със същото основно потребителско име (UPN). Новият акаунт се създава с помощта на различна стойност на PUID (уникален ИД за паспорт). Когато потребителят се опита да получи достъп до колекция от сайтове или OneDrive, потребителят има неправилен PUID. Вторият сценарий включва синхронизиране на справочника с организационна единица на Active Directory (OU). Ако потребителите вече са влезли в SharePoint и след това са преместени в друг OU и са пренасочени с SharePoint, те може да възникнат този проблем.

1. За да разрешите този проблем, трябва да възстановите първоначалния UPN със стъпките в статията, [Възстановяване на потребител в Microsoft 365](https://docs.microsoft.com/microsoft-365/admin/add-users/restore-user).
2. Ако не можете да възстановите първоначалния потребител, трябва да премахнете стария потребител от сайта OneDrive, като използвате тези стъпки, Премахнете потребител [от списъка с информация за потребителя](). 
3. След като това приключи, можете да проверите дали потребителят има администраторски права върху сайта на OneDrive, като следвате стъпките към Добавяне на администратор за потребителски [OneDrive](https://docs.microsoft.com/sharepoint/manage-user-profiles)

За повече информация относно нивата на разрешение вижте статията Разбиране [на нивата на разрешение в SharePoint](https://docs.microsoft.com/sharepoint/understanding-permission-levels).
