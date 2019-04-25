---
title: 1491-Search-not-returning-Expected-results
ms.author: markjjo
author: markjjo
manager: lauraw
ms.date: ''
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: 1491
ms.assetid: ''
ms.openlocfilehash: 517d9b75fc3aef09c0c2d5870aa695cc0ab10f06
ms.sourcegitcommit: 9d78905c512192ffc4675468abd2efc5f2e4baf4
ms.translationtype: MT
ms.contentlocale: bg-BG
ms.lasthandoff: 04/23/2019
ms.locfileid: "32383824"
---
# <a name="content-search-not-returning-expected-results"></a>Съдържание за търсене не връщат очакваните резултати

Когато изпълнява съдържание търсения от Office 365 сигурност & съответствие център, можете да получите неочаквани резултати. Помислете за следните неща, които може да повлияе резултатите от вашето търсене:

- **Съдържание места и условия за търсене**: Уверете се, че сте избрали правилното съдържание места и условия за търсене. Ако сте стартирали голям търсене (с много места), помислете за това разделяне на няколко търсения.

- **Частично индексирани елементи**: [частично индексирани елементи](https://docs.microsoft.com/office365/securitycompliance/partially-indexed-items-in-content-search) от пощенските кутии са включени в очакваните резултати. Въпреки това частично индексирани елементи от сайтове на SharePoint и OneDrive не са включени в търсене прогноза.

- **Търсене повреди**: при търсене на голям брой пощенски кутии (над 100 000 кутии), може да получите търсене грешки, с кодове за грешка CS008-009 и CS012-002). В този случай опитайте отново търсене само за неуспешни местонахождения на съдържание. Вижте [тази статия](https://docs.microsoft.com/office365/securitycompliance/retry-failed-content-search) за повече информация.
