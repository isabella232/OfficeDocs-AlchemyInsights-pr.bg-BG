---
title: Проблеми с връзката на SharePoint Designer
ms.author: pebaum
author: pebaum
manager: pamgreen
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: f2b1b6b4-10c9-4e83-b9cb-529a0b8a3c55
ms.openlocfilehash: 997ba3de58485d4fe6d24b926c33348378af8cd3
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: bg-BG
ms.lasthandoff: 09/14/2020
ms.locfileid: "47727160"
---
# <a name="sharepoint-designer-connection-issues"></a>Проблеми с връзката на SharePoint Designer 

Ако SharePoint Designer има проблеми с връзката към сайтове на SharePoint, моля, опитайте следните общи решения.

Стъпка 1: Уверете се, че SharePoint Designer 2013 е актуализиран с [SharePoint Designer Service Pack 1](https://support.microsoft.com/help/2817441/description-of-microsoft-sharepoint-designer-2013-service-pack-1-sp1) и [2 август 2016 актуализация за SharePoint Designer 2013](https://support.microsoft.com/help/3114721/august-2-2016-update-for-sharepoint-designer-2013-kb3114721).



Стъпка 2: изчистете локалните кеш файлове:

1. Затворете SharePoint Designer 2013.

2. На локалния компютър премахнете всички файлове, намерени във всяка от следните папки.

    - %APPDATA%\Microsoft\Web сървър Extensions\Cache
    - %APPDATA%\Microsoft\SharePoint Designer\ProxyAssemblyCache
    - %USERPROFILE%\AppData\Local\Microsoft\WebsiteCache

3. Отворете SharePoint Designer 2013 и въведете акаунта отново, за да видите дали работи.

Стъпка 3: [Разрешаване на модерното удостоверяване за Office 2013 на устройства с Windows](https://docs.microsoft.com/microsoft-365/admin/security-and-compliance/enable-modern-authentication).

Стъпка 4: администраторите ще трябва да **разрешат скрипт по избор** в настройките на центъра за администриране на SharePoint, за да позволят връзката на SharePoint Designer. Вижте [Разрешаване или забраняване на скрипт по избор](https://docs.microsoft.com/sharepoint/allow-or-prevent-custom-script) за повече информация.


