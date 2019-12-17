---
title: Проблеми с връзката на SharePoint Designer
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
ms.openlocfilehash: 9730bd66afd494385db3de605f5fe68d0f274ed3
ms.sourcegitcommit: 0f0186044a3597e42ad14c32ca58e7224344dcfa
ms.translationtype: MT
ms.contentlocale: bg-BG
ms.lasthandoff: 12/15/2019
ms.locfileid: "40051702"
---
# <a name="sharepoint-designer-connection-issues"></a>Проблеми с връзката на SharePoint Designer 

Ако SharePoint Designer изпитва проблеми с връзката към сайтове на SharePoint, моля, опитайте следните общи решения.

Стъпка 1: Проверете дали SharePoint Designer 2013 се актуализира с [SharePoint Designer Service Pack 1](https://support.microsoft.com/help/2817441/description-of-microsoft-sharepoint-designer-2013-service-pack-1-sp1) и [актуализация на 2 август 2016 за SharePoint Designer 2013](https://support.microsoft.com/help/3114721/august-2-2016-update-for-sharepoint-designer-2013-kb3114721).



Стъпка 2: изчистете локалните кеш файлове:

1. Затворете SharePoint Designer 2013.

2. На локалния компютър премахнете всички файлове, намерени във всяка от следните папки.

    - %Pipn%\mimsuser\lucerude
    - %Popon%\mimrosice\larter\sucor
    - %\Usit\up\pulersfir\mupsitep

3. Отворете SharePoint Designer 2013 и въведете отново акаунта, за да видите дали работи.

Стъпка 3: [Разрешаване на съвременни удостоверяване за Office 2013 на устройства с Windows](https://docs.microsoft.com/office365/admin/security-and-compliance/enable-modern-authentication?redirectSourcePath=/article/Enable-Modern-Authentication-for-Office-2013-on-Windows-devices-7dc1c01a-090f-4971-9677-f1b192d6c910&view=o365-worldwide).

Стъпка 4: администраторите ще трябва да **позволи персонализиран скрипт** в настройките на центъра за администриране на SharePoint, за да позволите на SharePoint Designer връзка. За повече информация вижте [Разрешаване или предотвратяване на персонализиран скрипт](https://docs.microsoft.com/sharepoint/allow-or-prevent-custom-script) .


