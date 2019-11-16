---
title: Отстраняване на неизправности достъп отказан съобщения OneDrive за бизнес сайтове
ms.author: efrene
author: efrene
manager: pamgreen
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.assetid: cebb7a4a-33e1-474e-a5d0-dbd02a80b1e9
ms.openlocfilehash: 3c40ad76a8961a3d0b4963483291c2a1364c51d3
ms.sourcegitcommit: b43f77221f47b50c41197a448a9c26c423ce1ad5
ms.translationtype: MT
ms.contentlocale: bg-BG
ms.lasthandoff: 11/15/2019
ms.locfileid: "37766700"
---
# <a name="troubleshooting-access-denied-messages-to-onedrive-for-business-sites"></a>Отстраняване на неизправности достъп отказан съобщения OneDrive за бизнес сайтове

Този проблем най-често се случва, когато потребител се изтрива и създава отново със същото основно потребителско име (UPN). Нов акаунт се създава с помощта на различен PUID (паспорт Еднозначен ID) стойност. Когато потребителят се опита да получите достъп до колекция от сайтове или техните OneDrive, потребителят е неправилен PUID. Втори сценарий включва указатели с Active Directory организационна единица (ОЕ). Ако потребителите вече са влезли в SharePoint и след това се преместват в друга ОЕ и повторно синхронизиране с SharePoint, те могат да възникнат този проблем.

1. За да разрешите този проблем, трябва да възстановите оригиналния UPN стъпки в статията, [възстановяване на потребител в Office 365](https://docs.microsoft.com/office365/admin/add-users/restore-user?view=o365-worldwide).
2. Ако не можете да възстановите първоначалния потребител трябва да премахнете стария потребител от сайта на OneDrive с помощта на тези стъпки, [премахнете потребител от списъка с информация за потребителя](). 
3. След това се прави, можете да проверите потребителят има администраторски права на сайта на OneDrive като следвате стъпките за добавяне на [администратор за onedrive на потребителя](https://docs.microsoft.com/sharepoint/manage-user-profiles?redirectSourcePath=%252fen-us%252farticle%252fmanage-user-profiles-in-the-sharepoint-admin-center-494bec9c-6654-41f0-920f-f7f937ea9723#add-and-remove-admins-for-a-users-onedrive)

За повече информация относно нивата на разрешение вижте статията, [разбиране на нивата на разрешение в SharePoint](https://docs.microsoft.com/sharepoint/understanding-permission-levels).
