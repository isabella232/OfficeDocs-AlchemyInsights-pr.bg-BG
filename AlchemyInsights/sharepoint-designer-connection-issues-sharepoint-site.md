---
title: SharePoint Проблеми с конструкторската връзка
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
ms.openlocfilehash: d55f7c1902bb623900fa74bdae70695b6e04ad84ce7b6ea314db614283ec436d
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: bg-BG
ms.lasthandoff: 08/05/2021
ms.locfileid: "53942014"
---
# <a name="sharepoint-designer-connection-issues"></a>SharePoint Проблеми с конструкторската връзка 

Ако SharePoint Designer има проблеми с връзката към SharePoint сайтове, опитайте следните често срещани решения.

Стъпка 1: Уверете се, че SharePoint Designer 2013 се [актуализира с SharePoint Designer Service Pack 1](https://support.microsoft.com/help/2817441/description-of-microsoft-sharepoint-designer-2013-service-pack-1-sp1) и актуализацията от 2 август [2016 г. за SharePoint Designer 2013](https://support.microsoft.com/help/3114721/august-2-2016-update-for-sharepoint-designer-2013-kb3114721).



Стъпка 2: Изчистете локалните кеш файлове:

1. Затворете SharePoint Designer 2013.

2. На локалния компютър премахнете всички файлове, намерени във всяка от следните папки.

    - %APPDATA%\Microsoft\Web Server Extensions\Cache
    - %APPDATA%\Microsoft\SharePoint Designer\ProxyAssemblyCache
    - %USERPROFILE%\AppData\Local\Microsoft\WebsiteCache

3. Отворете SharePoint Designer 2013 и въведете акаунта отново, за да видите дали работи.

Стъпка 3: [Разрешаване на модерното удостоверяване за Office 2013 на Windows устройства.](https://docs.microsoft.com/microsoft-365/admin/security-and-compliance/enable-modern-authentication)

Стъпка 4: Администраторите ще трябва да **разрешат** скрипт по избор в настройките на центъра SharePoint за администриране, за да позволят SharePoint Designer. Вижте [Разрешаване или предотвратяване на скрипт по избор](https://docs.microsoft.com/sharepoint/allow-or-prevent-custom-script) за повече информация.


