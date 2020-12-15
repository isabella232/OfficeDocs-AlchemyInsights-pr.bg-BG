---
title: Няма върнати резултати по време на търсене/Експортиране на съдържание
ms.author: v-jmathew
author: v-jmathew
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3200003"
- "7463"
ms.openlocfilehash: db025cd1278471a3c54d55409d9a9418095778a7
ms.sourcegitcommit: 9c64886a9e1a9b0ff356b28a5c1482ecc148d7ef
ms.translationtype: MT
ms.contentlocale: bg-BG
ms.lasthandoff: 12/14/2020
ms.locfileid: "49677190"
---
# <a name="no-results-returned-during-content-searchexport"></a>Няма върнати резултати по време на търсене/Експортиране на съдържание

Ако имате проблеми със следните сценарии за откриване на електронни данни:

- Търсене на съдържание/експортиране връща данни или неочаквани данни
- Търсенето на откриване на електронни данни или експортирането е неуспешно

Това може да се дължи на определени филтри за защита на съответствието, които са били настроени от определен администратор и не са били съобщени на всички администратори.

За да отстраните този проблем, прегледайте дали има някои филтри за защита, които може да предизвикат следните проблеми:

1. Свързване към центъра за сигурност и съответствие на PowerShell
2. Изпълнете следните кратки команди:

    `$org = “yourdomain.com”`

    `Get-ComplianceSecurityFilter -Organization $org`

За допълнителна информация относно филтрите за защита на съответствието вижте [филтриране на разрешения за търсене на съдържание](https://docs.microsoft.com/microsoft-365/compliance/permissions-filtering-for-content-search)
