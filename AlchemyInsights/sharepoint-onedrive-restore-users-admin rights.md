---
title: Отстраняване на отказан достъп съобщения до OneDrive за бизнес сайтове
ms.author: pebaum
author: pebaum
manager: pamgreen
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.assetid: cebb7a4a-33e1-474e-a5d0-dbd02a80b1e9
ms.openlocfilehash: a83936acf969926c113b28ceb22b006cdb96e2b4
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: bg-BG
ms.lasthandoff: 04/22/2020
ms.locfileid: "43692790"
---
# <a name="troubleshooting-access-denied-messages-to-onedrive-for-business-sites"></a>Отстраняване на отказан достъп съобщения до OneDrive за бизнес сайтове

Този проблем най-често възниква, когато потребител се изтрива и създава отново с едно и също основно потребителско име (UPN). Новият акаунт се създава чрез различна стойност на PUID (уникален ид на паспорт). Когато потребителят се опита да получите достъп до колекция от сайтове или oneDrive, потребителят има неправилен PUID. Втори сценарий включва синхронизиране на директории с Active Directory организационна единица (ОЕ). Ако потребителите вече са влезли в SharePoint и след това се преместват в друг OU и resynced с SharePoint, те могат да възникнат този проблем.

1. За да разрешите този проблем, трябва да възстановите оригиналния UPN със стъпките в статията, [възстановяване на потребител в Microsoft 365](https://docs.microsoft.com/office365/admin/add-users/restore-user?view=o365-worldwide).
2. Ако не можете да възстановите първоначалния потребител, трябва да премахнете стария потребител от oneDrive сайт, като използвате тези стъпки, [Премахнете потребител от списъка с информация за потребителя](). 
3. След това е направено, можете да проверите потребителят има администраторски права на сайта oneDrive, като следвате стъпките [за Добавяне на администратор за OneDrive на потребителя](https://docs.microsoft.com/sharepoint/manage-user-profiles)

За повече информация относно нивата на разрешение вижте [статията, разбиране на нивата на разрешение в SharePoint](https://docs.microsoft.com/sharepoint/understanding-permission-levels).
