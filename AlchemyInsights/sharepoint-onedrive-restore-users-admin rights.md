---
title: Отстраняване на неизправности Достъпът отказан съобщения за OneDrive за бизнес сайтове
ms.author: pebaum
author: pebaum
manager: pamgreen
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.assetid: cebb7a4a-33e1-474e-a5d0-dbd02a80b1e9
ms.openlocfilehash: 95bd46e8b7a6006f3735612d9a5602fb2b2a283b
ms.sourcegitcommit: bc7d6f4f3c9f7060d073f5130e1ec856e248d020
ms.translationtype: MT
ms.contentlocale: bg-BG
ms.lasthandoff: 06/02/2020
ms.locfileid: "44511173"
---
# <a name="troubleshooting-access-denied-messages-to-onedrive-for-business-sites"></a>Отстраняване на неизправности Достъпът отказан съобщения за OneDrive за бизнес сайтове

Този проблем най-често възниква, когато потребителят се изтрива и създава отново със същото основно потребителско име (UPN). Новият акаунт се създава с различна стойност puid (паспорт уникален ИД). Когато потребителят се опита да получите достъп до колекция от сайтове или своя OneDrive, потребителят е неправилен PUID. Втори сценарий включва указатели с Active Directory организационна единица (ОЕ). Ако потребителите вече са влезли в SharePoint и след това се преместват в друг ОЕ и resynced SharePoint, те може да се появи този проблем.

1. За да разрешите този проблем, трябва да възстановите първоначалния UPN със стъпките в статията, възстановяване на [потребител в Microsoft 365](https://docs.microsoft.com/microsoft-365/admin/add-users/restore-user).
2. Ако не можете да възстановите първоначалния потребител трябва да премахнете стария потребител от oneDrive сайта с помощта на тези стъпки, [Премахване на потребител от списъка с информация за потребителя](). 
3. След това можете да проверите потребителят има администраторски права на oneDrive сайт, като следвате стъпките за [Добавяне на администратор за потребител OneDrive](https://docs.microsoft.com/sharepoint/manage-user-profiles)

За повече информация относно нивата на разрешение вижте [статията, Разбиране нивата на разрешенията в SharePoint](https://docs.microsoft.com/sharepoint/understanding-permission-levels).
