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
ms.openlocfilehash: 6646ca4792ac4d9fb8bfb7433d53ecf4aeba8da0aca797225c16c02b28499889
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: bg-BG
ms.lasthandoff: 08/05/2021
ms.locfileid: "54013233"
---
# <a name="issues-installing-microsoft-defender-on-mac-or-linux"></a>Проблеми с инсталирането на Microsoft Defender на Mac или Linux

**Mac**

- Уверете се, че изискванията към системата са изпълнени, преди да инсталирате Microsoft Defender ATP for Mac. За повече информация вижте Как [да инсталирате Microsoft Defender ATP for Mac](/windows/security/threat-protection/microsoft-defender-atp/microsoft-defender-atp-mac#how-to-install-microsoft-defender-atp-for-mac).  
- Прегледайте информацията във файла: "/Library/Logs/Microsoft/mdatp/install.log".

**Linux**

- Уверете се, че изискванията към системата са изпълнени, преди да инсталирате Microsoft Defender ATP за Linux. За повече информация вижте Как [да инсталирате MDATP за Linux](/windows/security/threat-protection/microsoft-defender-atp/microsoft-defender-atp-linux#system-requirements). 
- За да проверите дали се изпълнява услугата MDATP, вижте Неуспешно [инсталиране](/windows/security/threat-protection/microsoft-defender-atp/linux-support-install#installation-failed).  
    За отстраняване и отстраняване на проблеми, ако услугата не се изпълнява, вижте Стъпки за отстраняване на неизправности, ако [услугата mdatp не се изпълнява](/windows/security/threat-protection/microsoft-defender-atp/linux-support-install#steps-to-troubleshoot-if-mdatp-service-isnt-running).
- За стъпки за проверка на конфигурацията на клиента, която проверява изздраве на продукта, и за да изпълните тест за откриване на текстовия файл на EICAR, вижте [Конфигуриране на клиента](/windows/security/threat-protection/microsoft-defender-atp/linux-install-manually#client-configuration).  

    **Забележка** За списък на поддържаните файлови системи за дейности при достъп вижте [Microsoft Defender ATP за Linux.](/windows/security/threat-protection/microsoft-defender-atp/microsoft-defender-atp-linux#system-requirements)