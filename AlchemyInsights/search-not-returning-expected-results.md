---
title: 1491-Търсене-не-връщащи се очаквани-резултати
ms.author: markjjo
author: markjjo
manager: lauraw
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "1491"
- "3200003"
ms.assetid: ''
ms.openlocfilehash: d0707af19b0299f7257a10a20ab38f47860308fb
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: bg-BG
ms.lasthandoff: 04/22/2020
ms.locfileid: "43709216"
---
# <a name="content-search-not-returning-expected-results"></a>Търсене на съдържание, което не връща очакванирезултати

Когато изпълнявате търсения за съдържание от центъра за сигурност на Microsoft 365 & Съответствието, може да получите неочаквани резултати от търсенето. Обмислете следните неща, които могат да повлияят на резултатите от търсенето Ви:

- **Местоположения на съдържание и условия за търсене:** Уверете се, че сте избрали правилните местоположения на съдържание и условия за търсене. Ако сте направили голямо търсене (с много местоположения), помислете дали да го разделите на няколко търсения.

- **Частично индексирани елементи:** [Частично индексираните елементи](https://docs.microsoft.com/office365/securitycompliance/partially-indexed-items-in-content-search) от пощенски кутии са включени в оценката на резултатите от търсенето. Обаче частично индексираелементи от сайтове в SharePoint и OneDrive не са включени в оценката за търсене.

- **Грешки при търсене:** Когато търсите голям брой пощенски кутии (над 100 000 пощенски кутии), можете да получите търсене грешки, с кодове за грешка като CS008-009 и CS012-002). В този случай опитайте отново търсенето само за неуспешните местоположения на съдържание. Вижте [тази статия](https://docs.microsoft.com/office365/securitycompliance/retry-failed-content-search) за повече информация.
