---
title: Отстраняване на неизправности при достъп отказан съобщения до OneDrive за бизнес сайтове
ms.author: efrene
author: efrene
manager: pamgreen
ms.date: 11/14/2018
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.assetid: cebb7a4a-33e1-474e-a5d0-dbd02a80b1e9
ms.openlocfilehash: 39f9b9b1ca22f6e5959e2b431fb373b0002c0a92
ms.sourcegitcommit: 1d98db8acb9959aba3b5e308a567ade6b62da56c
ms.translationtype: MT
ms.contentlocale: bg-BG
ms.lasthandoff: 08/22/2019
ms.locfileid: "36507800"
---
# <a name="troubleshooting-access-denied-messages-to-onedrive-for-business-sites"></a>Отстраняване на неизправности при достъп отказан съобщения до OneDrive за бизнес сайтове

Този проблем най-често се случва, когато даден потребител е изтрита и създадена отново със същото основно име на потребителя (UPN). Новият акаунт е създаден с помощта на различни PUID (паспорт уникален ИД) стойност. Когато потребителят се опитва да получи достъп до колекция от сайтове или техните OneDrive, потребителят има неправилен PUID. Вторият сценарий включва директория синхронизация с Active Directory организационни единици (OU). Ако потребителите са вече влезли в SharePoint, след това се премества в различни OU и resynced с SharePoint, те могат да срещнат този проблем.

1. За да разрешите този проблем трябва да възстановите оригиналния UPN със стъпките в статията,[възстановяване на потребител в Office 365](https://docs.microsoft.com/office365/admin/add-users/restore-user?view=o365-worldwide).
2. Ако не можете да възстановите оригиналния потребител трябва да премахнете старите потребител от сайта на OneDrive, с помощта на тези стъпки, [Премахване на потребител от списъка с информация за потребителя](). 
3. След това е направено, можете да проверите потребителят има права на администратор на сайта на OneDrive като следвате стъпките за [Добавяне администратор на за потребителски OneDrive](https://docs.microsoft.com/sharepoint/manage-user-profiles?redirectSourcePath=%252fen-us%252farticle%252fmanage-user-profiles-in-the-sharepoint-admin-center-494bec9c-6654-41f0-920f-f7f937ea9723#add-and-remove-admins-for-a-users-onedrive)

За повече информация за нивата на разрешения вижте статията, [разбиране на нивата на разрешение в SharePoint](https://docs.microsoft.com/sharepoint/understanding-permission-levels).
