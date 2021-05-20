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
ms.openlocfilehash: 39f180852fd0438597fa1ce665b2703fbc7b1aa4
ms.sourcegitcommit: f4866e94918c7b591ad0cd3b58169d340bcc7f00
ms.translationtype: MT
ms.contentlocale: bg-BG
ms.lasthandoff: 05/19/2021
ms.locfileid: "52539669"
---
# <a name="issues-installing-microsoft-defender-on-mac-or-linux"></a>Проблеми с инсталирането на Microsoft Defender на Mac или Linux

**Mac**

- Уверете се, че изискванията към системата са изпълнени, преди да Microsoft Defender ATP за Mac. За повече информация вижте [Как да инсталирате Microsoft Defender ATP за Mac.](/windows/security/threat-protection/microsoft-defender-atp/microsoft-defender-atp-mac#how-to-install-microsoft-defender-atp-for-mac)  
- Прегледайте информацията във файла: "/Library/Logs/Microsoft/mdatp/install.log".

**Linux**

- Уверете се, че изискванията към системата са изпълнени, преди да Microsoft Defender ATP за Linux. За повече информация вижте Как [да инсталирате MDATP за Linux](/windows/security/threat-protection/microsoft-defender-atp/microsoft-defender-atp-linux#system-requirements). 
- За да проверите дали се изпълнява услугата MDATP, вижте Неуспешно [инсталиране](/windows/security/threat-protection/microsoft-defender-atp/linux-support-install#installation-failed).  
    За отстраняване и отстраняване на проблеми, ако услугата не се изпълнява, вижте Стъпки за отстраняване на неизправности, ако [услугата mdatp не се изпълнява](/windows/security/threat-protection/microsoft-defender-atp/linux-support-install#steps-to-troubleshoot-if-mdatp-service-isnt-running).
- За стъпки за проверка на конфигурацията на клиента, която проверява изздраве на продукта, и за да изпълните тест за откриване на текстовия файл на EICAR, вижте [Конфигуриране на клиента](/windows/security/threat-protection/microsoft-defender-atp/linux-install-manually#client-configuration).  

    **Забележка** За списък на поддържаните файлови системи за дейност при достъп вижте [Microsoft Defender ATP за Linux](/windows/security/threat-protection/microsoft-defender-atp/microsoft-defender-atp-linux#system-requirements).