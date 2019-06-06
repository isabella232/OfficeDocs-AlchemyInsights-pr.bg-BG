---
title: Дават на потребителите достъп до SharePoint и OneDrive
ms.author: kirks
author: Techwriter40
manager: pamgreen
ms.date: 11/14/2018
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: cebb7a4a-33e1-474e-a5d0-dbd02a80b1e9
ms.openlocfilehash: 9326932e93970edc96396a141c9b36b14e7b4d4d
ms.sourcegitcommit: 241e21b6da226563bf70bdb1f5bad3d91c38cd2c
ms.translationtype: MT
ms.contentlocale: bg-BG
ms.lasthandoff: 06/05/2019
ms.locfileid: "34736637"
---
# <a name="give-users-access-to-sharepoint-and-onedrive"></a>Дават на потребителите достъп до SharePoint и OneDrive

Този проблем най-често се случва, когато даден потребител е изтрита и създадена отново със същото основно име на потребителя (UPN). Новият акаунт е създаден с помощта на различни PUID (паспорт уникален ИД) стойност. Когато потребителят се опитва да получи достъп до колекция от сайтове или техните OneDrive, потребителят има неправилен PUID. Вторият сценарий включва директория синхронизация с Active Directory организационни единици (OU). Ако потребителите са вече влезли в SharePoint, след това се премества в различни OU и resynced с SharePoint, те могат да срещнат този проблем.

За да разрешите този проблем трябва да възстановите оригиналния UPN със стъпките в статията,[възстановяване на потребител в Office 365](https://docs.microsoft.com/en-us/office365/admin/add-users/restore-user?view=o365-worldwide).

След това е направено, можете да проверите потребителят има права на администратор на сайта на OneDrive като следвате стъпките за [Добавяне администратор на за потребителски OneDrive](https://docs.microsoft.com/en-us/sharepoint/manage-user-profiles?redirectSourcePath=%252fen-us%252farticle%252fmanage-user-profiles-in-the-sharepoint-admin-center-494bec9c-6654-41f0-920f-f7f937ea9723#add-and-remove-admins-for-a-users-onedrive)

За повече информация за нивата на разрешения вижте статията, [разбиране на нивата на разрешение в SharePoint](https://docs.microsoft.com/en-us/sharepoint/understanding-permission-levels).
