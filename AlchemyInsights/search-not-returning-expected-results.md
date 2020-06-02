---
title: 1491-търсене-не връщащи се очаквани-резултати
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
ms.openlocfilehash: 57421d459ef03049d6f931db659a5f9b253f5002
ms.sourcegitcommit: bc7d6f4f3c9f7060d073f5130e1ec856e248d020
ms.translationtype: MT
ms.contentlocale: bg-BG
ms.lasthandoff: 06/02/2020
ms.locfileid: "44510561"
---
# <a name="content-search-not-returning-expected-results"></a>Търсенето на съдържание не връща очакваните резултати

Когато изпълнявате търсене на съдържание от центъра за съответствие на Microsoft 365 & за защита, можете да получите неочаквани резултати от търсенето. Обмислете следните неща, които могат да повлияят на резултатите от търсенето:

- **Местоположения на съдържанието и условия за търсене:** Уверете се, че сте избрали правилните местоположения на съдържанието и условията за търсене. Ако сте извършили голямо търсене (с много местоположения), помислете дали да го разделите на няколко търсения.

- **Частично индексирани елементи:** [Частично индексирани елементи](https://docs.microsoft.com/microsoft-365/compliance/partially-indexed-items-in-content-search) от пощенски кутии са включени в очакваните резултати от търсенето. Обаче частично индексирани елементи от сайтове в SharePoint и OneDrive не са включени в оценката на търсенето.

- **Търсене грешки:** При търсене на голям брой пощенски кутии (над 100 000 пощенски кутии), можете да получите грешки при търсене, с кодове за грешка като CS008-009 и CS012-002). В този случай опитайте отново само за неуспешно съдържание местоположения. Вижте [тази статия](https://docs.microsoft.com/microsoft-365/compliance/retry-failed-content-search) за повече информация.
