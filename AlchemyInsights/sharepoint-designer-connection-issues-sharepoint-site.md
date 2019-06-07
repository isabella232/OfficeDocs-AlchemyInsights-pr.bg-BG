---
title: Нива на разрешение на SharePoint Online
ms.author: kirks
author: Techwriter40
manager: pamgreen
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: f2b1b6b4-10c9-4e83-b9cb-529a0b8a3c55
ms.openlocfilehash: 356fef8e02f2c1fd9d209c68194685bb0acaa367
ms.sourcegitcommit: 4b7e478ce700c0b781efec3857ac4dce5bdf00c6
ms.translationtype: MT
ms.contentlocale: bg-BG
ms.lasthandoff: 06/07/2019
ms.locfileid: "34760682"
---
# <a name="sharepoint-designer-connection-issues"></a>SharePoint Designer проблеми с връзката 

Ако SharePoint Designer изпитва проблеми с връзката до сайтове на SharePoint, харесвам опитвам следните общи решения.

Стъпка 1: Проверете SharePoint Designer е актуализиран.

- [SharePoint Designer 2013](https://www.microsoft.com/download/details.aspx?id=35491)

- [SharePoint Designer Service Pack 1 (SP1)](https://support.microsoft.com/help/2817441/description-of-microsoft-sharepoint-designer-2013-service-pack-1-sp1)

- [Актуализация за SharePoint Designer 2013 (KB3114721)](https://support.microsoft.com/help/3114721/august-2-2016-update-for-sharepoint-designer-2013-kb3114721)

Стъпка 2: Изчистване на местните кеш файлове

- Затворете SharePoint Designer 2013.

- На локалния компютър преминете към следните папки да премахнете кеширани файлове.

- Щракнете върху Старт, Run и изтриване на всички файлове, намерени под всеки от по-долу места.

%APPDATA%\Microsoft\Web сървър Extensions\Cache %APPDATA%\Microsoft\SharePoint Designer\ProxyAssemblyCache %USERPROFILE%\AppData\Local\Microsoft\WebsiteCache

Отворете SharePoint Designer 2013 и въведете акаунта отново, за да видим дали тя работи.

Стъпка 3: [Разрешаване на модерни удостоверяване за офис 2013 на устройства, Windows](https://docs.microsoft.com/office365/admin/security-and-compliance/enable-modern-authentication?redirectSourcePath=/article/Enable-Modern-Authentication-for-Office-2013-on-Windows-devices-7dc1c01a-090f-4971-9677-f1b192d6c910&view=o365-worldwide)

Стъпка 4: Администратори ще трябва да разрешите потребителски скрипт да позволите на SharePoint Designer връзка.

За подробни стъпки, примери и съображения вижте [Разрешаване или предотвратяване на потребителски скрипт](https://docs.microsoft.com/sharepoint/allow-or-prevent-custom-script).


