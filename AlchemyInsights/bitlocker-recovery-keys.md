---
title: Ключове за възстановяване на BitLocker
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "1922"
- "9000220"
ms.openlocfilehash: 4e06e0e43b63836b9e9cf923e554dd474b82c671
ms.sourcegitcommit: 123e9fe46e99719dd271e75a66555861e968f4a2
ms.translationtype: MT
ms.contentlocale: bg-BG
ms.lasthandoff: 12/30/2019
ms.locfileid: "40908804"
---
# <a name="accessing-bitlocker-recovery-keys"></a>Достъп до клавишите за възстановяване на BitLocker

При конфигуриране на настройките на BitLocker InTune endpoint Protection правила, е възможно да определите дали информацията за възстановяване на BitLocker трябва да се съхранява в Azure Active Directory.

Ако тази настройка е конфигурирана, съхранените данни за възстановяване трябва да бъдат видими за InTune Admin като част от данните за запис на данни в острието на InTune устройства по два начина:

Устройства-Azure AD устройства-> "устройство" или устройства-> всички устройства-> "устройство"-> ключове за възстановяване

Алтернативно, ако има администраторски достъп до самото устройство, ключ за възстановяване (Password) може да се види като изпълните следната команда от команден ред с повишени права:

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
Ако устройството е шифровано преди записването в InTune, ключът за възстановяване може да е свързан с "акаунт в Microsoft" (МУИ), използван за влизане в устройството по време на процеса на OOBE. Ако случаят е такъв, достъпът https://onedrive.live.com/recoverykey и влизането с този Муи трябва да показват устройствата, за които са били съхранени ключовете за възстановяване.
 
Ако устройството е шифровано в резултат на конфигурация чрез базирани на домейна групови правила, информацията за възстановяване може да се съхранява в локалната Active Directory.
 

