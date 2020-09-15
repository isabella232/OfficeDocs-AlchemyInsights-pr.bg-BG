---
title: Ключове за възстановяване на BitLocker
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
ms.openlocfilehash: 7c56e68cf303939d8e7d4ee0a7301e367ecfe9f9
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: bg-BG
ms.lasthandoff: 09/14/2020
ms.locfileid: "47685875"
---
# <a name="accessing-bitlocker-recovery-keys"></a>Достъп до ключове за възстановяване на BitLocker

Когато конфигурирате настройките за защитено стартиране, е възможно да определите дали информацията за възстановяване на BitLocker трябва да бъде съхранена в Azure Active Directory.

Ако тази настройка е конфигурирана, съхранените данни за възстановяване трябва да бъдат видими за администратора на настройка като част от данните за запис на устройството в "Настройки на устройства" в Blade по два начина:

Устройства – устройства за Azure AD – > "устройство" или устройства – > на всички устройства – > "устройство" – > ключове за възстановяване

Друга възможност е да се види дали има административен достъп до самото устройство, като изпълните следната команда от команден ред:

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
Ако устройството е било шифровано преди записването в звук, ключът за възстановяване може да е свързан с "акаунт в Microsoft" (MSA), използван за влизане в устройството по време на процеса на OOBE. Ако това е така, достъпът до  https://onedrive.live.com/recoverykey и влизането с този MSA трябва да показва устройствата, за които са съхранени ключове за възстановяване.
 
Ако устройството е шифровано като резултат от конфигурирането на групови правила, базирани на домейн, информацията за възстановяване може да бъде съхранена в локалната активна директория.
 

