---
title: Ключове за възстановяване на Bitlocker
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "1922"
- "9000220"
ms.openlocfilehash: 8708ed76f6abe81582823c8af89db8fffef9a3c5
ms.sourcegitcommit: 7b2e5078dd65f11af6650e692a7ea48e91f544e0
ms.translationtype: MT
ms.contentlocale: bg-BG
ms.lasthandoff: 04/02/2021
ms.locfileid: "51505057"
---
# <a name="accessing-bitlocker-recovery-keys"></a>Достъп до клавишите за възстановяване на Bitlocker

Когато конфигурирате настройките на Bitlocker Intune Endpoint Protection Policy, е възможно да определите дали информацията за възстановяване на Bitlocker трябва да се съхранява в Azure Active Directory.

Ако тази настройка е конфигурирана, съхранените данни за възстановяване трябва да са видими за администратора на Intune като част от данните за записа на устройството в диска intune Devices по два начина:

Устройства – Устройства на Azure AD – > "Устройство" OR Устройства – > Всички устройства – > "Устройство" – > Ключове за възстановяване

Като алтернатива, ако има административен достъп до самото устройство, ключът за възстановяване (Парола) може да се види, като изпълните следната команда от команден прозорец с администраторски права:

```
manage-bde -protectors c: -get
Example
Volume C: []
All Key Protectors
    TPM:
      ID: {8A5D13D6-7ED9-46C8-A74F-AC3ADF016EC8}
      PCR Validation Profile:
        0, 2, 4, 8, 9, 10, 11
    Numerical Password:
      ID: {DFA26333-XXXX-402C-YYYY-A8C40AF3ZZZZ}
      Password:
        393943-22222-281721-555554-577984-77777-194700-99999
```
Ако устройството е шифровано преди записването в Intune, ключът за възстановяване може да е свързан с "Акаунт в Microsoft" (MSA), използван за влизане в устройството по време на процеса на OOBE. Ако случаят е такъв, достъпът и влизането с този MSA трябва да показват  https://onedrive.live.com/recoverykey устройствата, за които са съхранени клавишите за възстановяване.
 
Ако устройството е шифровано в резултат на конфигуриране чрез групови правила, базирани на домейни, информацията за възстановяване може да се съхранява в предварителния Active Directory.

Ако сте конфигурирали правила за защита на крайни точки, за да съхранявате ключа за възстановяване в Azure Active Directory, но ключът за конкретно устройство не е качен, можете да задействате качването, като завъртате ключа за възстановяване за това устройство от конзолата MEM. За подробности вижте Завъртане на [клавишите за възстановяване на BitLocker](https://docs.microsoft.com/mem/intune/protect/encrypt-devices#view-details-for-recovery-keys).

