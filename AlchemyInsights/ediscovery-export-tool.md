---
title: Инструмент за експортиране на откриване на електронни данни
ms.author: pebaum
author: pebaum
manager: scotv
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
ms.openlocfilehash: b1100175c75fb77a499e706380305eb016cf1b2b
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: bg-BG
ms.lasthandoff: 04/15/2021
ms.locfileid: "51814577"
---
# <a name="cant-install-or-run-the-ediscovery-export-tool"></a>Не можете да инсталирате или изпълните инструмента за експортиране на електронни данни?

Ако не можете да инсталирате или изпълните инструмента за експортиране на електронни данни, за да изтеглите резултатите от търсенето, проверете следните неща:
  
- Компютърът, който използвате, отговаря на следните предварителни изисквания:

  - 32- или 64-битови версии на Windows 7 и по-нови версии

  - Microsoft .NET Framework 4.7

  - Поддържан браузър:

  - Microsoft Edge

    Или

  - Internet Explorer 10 и по-нови версии

    Други браузъри, като например Google Chrome и Mozilla Firefox, не се поддържат.

- Вашата организация може да се свърже с крайната точка в Azure, която е **\* .blob.core.windows.net** (заместващ символ представлява уникален идентификатор за вашата задача за експортиране).

- На вас ви е възложена ролята експортиране в центъра за съответствие на защитата на Microsoft 365. &amp; По подразбиране тази роля се присвоява само на ролевата група на диспечера за откриване на електронни данни. Вижте [Задаване на разрешения за откриване на електронни информация](https://docs.microsoft.com/microsoft-365/compliance/assign-ediscovery-permissions).

За повече информация вижте Експортиране [на резултатите от търсенето на съдържание](https://docs.microsoft.com/microsoft-365/compliance/export-search-results).

Ако експортирате повече от 100K пощенски кутии, ще трябва да използвате следните Powershell, за да изтеглите резултатите от експортирането: Експортиране на резултати от повече от [100 000 пощенски кутии.](https://docs.microsoft.com/microsoft-365/compliance/export-search-results?view=o365-worldwide%23exporting-results-from-more-than-100000-mailboxes)