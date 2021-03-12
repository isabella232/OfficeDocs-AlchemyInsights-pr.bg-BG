---
title: Проблеми с инсталирането на Microsoft Defender на Mac или Linux
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/16/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "6028"
- "9001222"
ms.openlocfilehash: a8d5ad2246b9b83e1e0a4d5be4dd8bb41c16e734
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: bg-BG
ms.lasthandoff: 09/14/2020
ms.locfileid: "50713284"
---
# <a name="issues-installing-microsoft-defender-on-mac-or-linux"></a>Проблеми с инсталирането на Microsoft Defender на Mac или Linux

**Mac**

- Уверете се, че системните изисквания са изпълнени, преди да инсталирате Microsoft Defender ATP for Mac. За повече информация вижте [как да инсталирате Microsoft Defender ATP for Mac](https://docs.microsoft.com/windows/security/threat-protection/microsoft-defender-atp/microsoft-defender-atp-mac#how-to-install-microsoft-defender-atp-for-mac).  
- Прегледайте информацията във файла: "/Library/Logs/Microsoft/mdatp/install.log".

**Linux**

- Уверете се, че системните изисквания са изпълнени, преди да инсталирате Microsoft Defender ATP за Линукс. За повече информация вижте [как да инсталирате Microsoft Defender ATP за Линукс](https://docs.microsoft.com/windows/security/threat-protection/microsoft-defender-atp/microsoft-defender-atp-linux#system-requirements). 
- За да се уверите, че услугата MDATP се изпълнява, вижте [Неуспешно инсталиране](https://docs.microsoft.com/windows/security/threat-protection/microsoft-defender-atp/linux-support-install#installation-failed).  
    За отстраняване на неизправности и отстраняване на проблеми Ако услугата не се изпълнява, вижте [стъпки за отстраняване на неизправности, ако услугата mdatp не се изпълнява](https://docs.microsoft.com/windows/security/threat-protection/microsoft-defender-atp/linux-support-install#steps-to-troubleshoot-if-mdatp-service-isnt-running).
- За стъпки за проверка на конфигурацията на клиента, което проверява изправността на продукта, и за да изпълните тест за откриване в текстов файл на EICAR, вижте [Конфигуриране на клиент](https://docs.microsoft.com/windows/security/threat-protection/microsoft-defender-atp/linux-install-manually#client-configuration).  

    **Забележка** За списък на поддържаните файлови системи за дейности в Access вижте [Microsoft Defender ATP за Линукс](https://docs.microsoft.com/windows/security/threat-protection/microsoft-defender-atp/microsoft-defender-atp-linux#system-requirements).