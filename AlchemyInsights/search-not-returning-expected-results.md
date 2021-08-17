---
title: 1491-search-not-returning-expected-results
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
- "1491"
- "3200003"
ms.assetid: ''
ms.openlocfilehash: 846034d68a59d053cbe37aeba3a75e20a60786fd7ff24106964229b1deb77608
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: bg-BG
ms.lasthandoff: 08/05/2021
ms.locfileid: "54052699"
---
# <a name="content-search-not-returning-expected-results"></a>Търсенето на съдържание не връща очакваните резултати

Когато изпълнявате "Търсене на съдържание" от центъра Microsoft 365 защита & за съответствие, може да получите неочаквани резултати от търсенето. Помислете за следните неща, които могат да повлияят на резултатите от търсенето:

- **Местоположения на съдържанието и условия за** търсене: Уверете се, че сте избрали правилните местоположения на съдържанието и условията за търсене. Ако сте направили голямо търсене (с много местоположения), помислете дали да не го разделите на няколко търсения.

- **Частично индексирани елементи:**  [Частично индексираните елементи от](https://docs.microsoft.com/microsoft-365/compliance/partially-indexed-items-in-content-search) пощенските кутии са включени в прогнозните резултати от търсенето. Частично индексираните елементи от сайтове в SharePoint и OneDrive не са включени в прогнозата за търсене.

- **Грешки при** търсене: Когато търсите голям брой пощенски кутии (над 100 000 пощенски кутии), може да получите грешки при търсене с кодове на грешки, като например CS008-009 и CS012-002). В този случай опитайте отново търсенето само за неуспешните местоположения на съдържанието. Вижте  [тази статия](https://docs.microsoft.com/microsoft-365/compliance/retry-failed-content-search) за повече информация.
