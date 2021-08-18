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
ms.openlocfilehash: defc11265caf371ce0a62a10a5de1d8ff88a8e11
ms.sourcegitcommit: ab75f66355116e995b3cb5505465b31989339e28
ms.translationtype: MT
ms.contentlocale: bg-BG
ms.lasthandoff: 08/13/2021
ms.locfileid: "58325238"
---
# <a name="issues-installing-microsoft-defender-on-mac-or-linux"></a>Проблеми с инсталирането на Microsoft Defender на Mac или Linux

**Mac**

- Уверете се, че изискванията към системата са изпълнени, преди да инсталирате Microsoft Defender ATP for Mac. За повече информация вижте Как [да инсталирате Microsoft Defender ATP for Mac](https://docs.microsoft.com/windows/security/threat-protection/microsoft-defender-atp/microsoft-defender-atp-mac#how-to-install-microsoft-defender-atp-for-mac).  
- Прегледайте информацията във файла: "/Library/Logs/Microsoft/mdatp/install.log".

**Linux**

- Уверете се, че изискванията към системата са изпълнени, преди да инсталирате Microsoft Defender ATP за Linux. За повече информация вижте Как [да инсталирате MDATP за Linux](https://docs.microsoft.com/windows/security/threat-protection/microsoft-defender-atp/microsoft-defender-atp-linux#system-requirements). 
- За да проверите дали се изпълнява услугата MDATP, вижте Неуспешно [инсталиране](https://docs.microsoft.com/windows/security/threat-protection/microsoft-defender-atp/linux-support-install#installation-failed).  
    За отстраняване и отстраняване на проблеми, ако услугата не се изпълнява, вижте Стъпки за отстраняване на неизправности, ако [услугата mdatp не се изпълнява](https://docs.microsoft.com/windows/security/threat-protection/microsoft-defender-atp/linux-support-install#steps-to-troubleshoot-if-mdatp-service-isnt-running).
- За стъпки за проверка на конфигурацията на клиента, която проверява изздраве на продукта, и за да изпълните тест за откриване на текстовия файл на EICAR, вижте Конфигуриране [на клиента](https://docs.microsoft.com/windows/security/threat-protection/microsoft-defender-atp/linux-install-manually#client-configuration).  

    **Забележка** За списък на поддържаните файлови системи за дейности при достъп вижте [Microsoft Defender ATP за Linux](https://docs.microsoft.com/windows/security/threat-protection/microsoft-defender-atp/microsoft-defender-atp-linux#system-requirements).