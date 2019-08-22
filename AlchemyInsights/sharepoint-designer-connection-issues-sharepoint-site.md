---
title: SharePoint Designer проблеми с връзката
ms.author: efrene
author: efrene
manager: pamgreen
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: f2b1b6b4-10c9-4e83-b9cb-529a0b8a3c55
ms.openlocfilehash: a4aeaeaea5743c276b907c78317ff30f5610be81
ms.sourcegitcommit: 1d98db8acb9959aba3b5e308a567ade6b62da56c
ms.translationtype: MT
ms.contentlocale: bg-BG
ms.lasthandoff: 08/22/2019
ms.locfileid: "36508412"
---
# <a name="sharepoint-designer-connection-issues"></a>SharePoint Designer проблеми с връзката 

Ако SharePoint Designer изпитва проблеми с връзката до сайтове на SharePoint, опитайте следните общи решения.

Стъпка 1: Уверете се, че SharePoint Designer 2013 се актуализира с [SharePoint Designer Service Pack 1](https://support.microsoft.com/help/2817441/description-of-microsoft-sharepoint-designer-2013-service-pack-1-sp1) и на [2 август 2016 актуализацията за SharePoint Designer 2013](https://support.microsoft.com/help/3114721/august-2-2016-update-for-sharepoint-designer-2013-kb3114721).



Стъпка 2: Изчистване на местните кеш файлове:

1. Затворете SharePoint Designer 2013.

2. На локалния компютър премахнете всички файлове, намерени във всяка от следните папки.

    - %APPDATA%\Microsoft\Web сървър Extensions\Cache
    - %APPDATA%\Microsoft\SharePoint Designer\ProxyAssemblyCache
    - %USERPROFILE%\AppData\Local\Microsoft\WebsiteCache

3. Отворете SharePoint Designer 2013 и въведете акаунта отново, за да видим дали тя работи.

Стъпка 3: [Разрешаване на модерни удостоверяване за офис 2013 на устройства, Windows](https://docs.microsoft.com/office365/admin/security-and-compliance/enable-modern-authentication?redirectSourcePath=/article/Enable-Modern-Authentication-for-Office-2013-on-Windows-devices-7dc1c01a-090f-4971-9677-f1b192d6c910&view=o365-worldwide).

Стъпка 4: Администратори ще трябва да **Разрешите потребителски скрипт** в настройките на центъра за администриране на SharePoint да позволите на SharePoint Designer връзка. Вижте [Разрешаване или предотвратяване на потребителски скрипт](https://docs.microsoft.com/sharepoint/allow-or-prevent-custom-script) за повече информация.


