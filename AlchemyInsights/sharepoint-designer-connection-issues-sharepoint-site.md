---
title: Проблеми с връзката с SharePoint Designer
ms.author: pebaum
author: pebaum
manager: pamgreen
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: f2b1b6b4-10c9-4e83-b9cb-529a0b8a3c55
ms.openlocfilehash: 01ccc6bc28148f397fb6cd2b7a0eaaeb5b51973f
ms.sourcegitcommit: bc7d6f4f3c9f7060d073f5130e1ec856e248d020
ms.translationtype: MT
ms.contentlocale: bg-BG
ms.lasthandoff: 06/02/2020
ms.locfileid: "44511533"
---
# <a name="sharepoint-designer-connection-issues"></a>Проблеми с връзката с SharePoint Designer 

Ако SharePoint Designer изпитва проблеми с връзката към сайтове на SharePoint, опитайте следните общи решения.

Стъпка 1: Уверете се, че SharePoint Designer 2013 се актуализира с [SharePoint Designer Service Pack 1](https://support.microsoft.com/help/2817441/description-of-microsoft-sharepoint-designer-2013-service-pack-1-sp1) и [2 август 2016 актуализацията за SharePoint Designer 2013](https://support.microsoft.com/help/3114721/august-2-2016-update-for-sharepoint-designer-2013-kb3114721).



Стъпка 2: Изчистете локалните кеш файлове:

1. Затворете SharePoint Designer 2013.

2. На локалния компютър премахнете всички файлове, намерени във всяка от следните папки.

    - %APPDATA%\Microsoft\Разширения на уеб сървър\Кеш
    - %APPDATA%\Microsoft\Дизайнер на SharePoint\Прокси събраниеКакто
    - %USERPROFILE%\AppData локално\MicrosoftCache

3. Отворете SharePoint Designer 2013 и въведете акаунта отново, за да видите дали работи.

Стъпка 3: [Разрешаване на съвременни удостоверяване за Office 2013 на устройства с Windows](https://docs.microsoft.com/microsoft-365/admin/security-and-compliance/enable-modern-authentication).

Стъпка 4: Администраторите ще трябва да **разрешите потребителски скрипт** в настройките на центъра за администриране на SharePoint да позволите на връзката SharePoint Designer. За повече информация вижте [Разрешаване или забраняване на скриптове по избор.](https://docs.microsoft.com/sharepoint/allow-or-prevent-custom-script)


