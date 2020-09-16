---
title: 1491-Search-not-Re-Re---Up-очаквани резултати
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
ms.openlocfilehash: 5c4452726c1dbe2232ee63e8a9ee4d089f5c76db
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: bg-BG
ms.lasthandoff: 09/14/2020
ms.locfileid: "47740463"
---
# <a name="content-search-not-returning-expected-results"></a>Търсенето на съдържание не връща очакваните резултати

При изпълнение на търсения на съдържание от центъра за съответствие на Microsoft 365 Security &, е възможно да получите неочаквани резултати от търсенето. Обмислете следните неща, които могат да повлияят на резултатите от търсенето:

- **Местоположения на съдържание и условия за търсене**: Уверете се, че сте избрали правилните местоположения и условия за търсене на съдържание. Ако сте стартирали голямо търсене (с много местоположения), обмислете разделянето му на няколко търсения.

- **Частично индексирани елементи**:  [частично индексираните елементи](https://docs.microsoft.com/microsoft-365/compliance/partially-indexed-items-in-content-search) от пощенските кутии се включват в прогнозните резултати от търсенето. Обаче частично индексираните елементи от сайтове в SharePoint и OneDrive не се включват в прогнозната стойност на търсенето.

- **Неизправности при търсене**: когато се търсят голям брой пощенски кутии (над 100 000 пощенски кутии), може да получите грешки при търсенето с кодове на грешки, като например CS008-009 и CS012-002). В този случай Повторете търсенето само за местоположенията с неуспешно съдържание. Вижте  [тази статия](https://docs.microsoft.com/microsoft-365/compliance/retry-failed-content-search) за повече информация.
