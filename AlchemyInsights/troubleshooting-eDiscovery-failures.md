---
title: 1490-troubleshooting-eDiscovery-failures
ms.author: markjjo
author: markjjo
manager: lauraw
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "1490"
- "3200003"
ms.assetid: ''
ms.openlocfilehash: 7b819b9bb18b5c0a635e708eccc0f23271267874707e5f3a7d41b633a05f2822
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: bg-BG
ms.lasthandoff: 08/05/2021
ms.locfileid: "54105557"
---
# <a name="troubleshoot-content-search-errors"></a>Отстраняване на грешки при търсене на съдържание

Имате проблеми с търсенето на съдържание или получавате грешки, когато експортирате резултатите от търсенето?

Получавате ли например следното, когато изпълнявате търсения?

- Грешки в CS008 или CS012

- Грешки при заетост/изчакване на сървъра

- Възникна грешка в приложението

Или когато търсите или експортирате резултати от голям брой пощенски кутии (над 100 000 пощенски кутии), получавате ли грешки при експортиране?

За тези типове грешки опитайте отново да потърсите местоположенията на съдържанието, които са неуспешни. Вижте  [тази статия](https://docs.microsoft.com/microsoft-365/compliance/retry-failed-content-search) за повече информация.

Ако експортирате повече от 100K пощенски кутии, ще трябва да използвате следните Powershell, за да изтеглите резултатите от експортирането: Експортиране на резултати от повече от [100 000 пощенски кутии.](https://docs.microsoft.com/microsoft-365/compliance/export-search-results?view=o365-worldwide%23exporting-results-from-more-than-100000-mailboxes)
