---
title: инструмент за експортиране на откриването на електронни данни
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
- "263"
- "928"
- "1100001"
- "3100022"
ms.assetid: b16d310d-1134-4959-be68-d1c0ad463930
ms.openlocfilehash: 67e59182a5053111a08f5fb2be814931a1aa815d
ms.sourcegitcommit: fbe6925797cab0b38172386f1b059dc122e452a4
ms.translationtype: MT
ms.contentlocale: bg-BG
ms.lasthandoff: 09/25/2020
ms.locfileid: "48277927"
---
# <a name="cant-install-or-run-the-ediscovery-export-tool"></a>Не можете да инсталирате или да изпълните инструмента за експортиране на откриването на електронни данни?

Ако не можете да инсталирате или да изпълните инструмента за експортиране на откриването на електронни данни, за да изтеглите резултатите от търсенето, проверете следните неща:
  
- Компютърът, който използвате, отговаря на тези предварителни изисквания:

  - 32-или 64-битова версия на Windows 7 и по-нови версии

  - Microsoft .NET Framework 4.7

  - Поддържан браузър:

  - Microsoft Edge

    Или

  - Internet Explorer 10 и по-нови версии

    Други браузъри, като например Google Chrome и Mozilla Firefox, не се поддържат.

- Вашата организация може да се свърже с крайната точка в Azure, която е ** \* . blob.Core.Windows.net** (Заместващият символ представлява уникален идентификатор за вашето задание за експортиране).

- Присвоявате ви роля за експортиране в центъра за съответствие на защитата на Microsoft 365 &amp; . По подразбиране тази роля се присвоява само към ролевата група "Диспечер за откриване на електронни данни". Вижте даване на [разрешения за откриване](https://docs.microsoft.com/microsoft-365/compliance/assign-ediscovery-permissions)на електронни данни.

За повече информация вижте [експортиране на резултати от търсене на съдържание](https://docs.microsoft.com/microsoft-365/compliance/export-search-results).

Ако експортирате повече от 100K пощенски кутии, ще трябва да използвате следния PowerShell, за да изтеглите резултатите от износа:  [експортиране на резултати от повече от 100k пощенски кутии](https://docs.microsoft.com/microsoft-365/compliance/export-search-results?view=o365-worldwide%23exporting-results-from-more-than-100000-mailboxes).