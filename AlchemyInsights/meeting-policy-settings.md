---
title: Настройки на правилата за събрания
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000734"
- "2657"
ms.openlocfilehash: 509bd0c686830c04ed27f97372411677c0a7f4a4
ms.sourcegitcommit: 9aaa61d717e0fd475d2e9f0507c42aa40d073b5f
ms.translationtype: MT
ms.contentlocale: bg-BG
ms.lasthandoff: 02/15/2020
ms.locfileid: "42042833"
---
# <a name="manage-meeting-policies-in-microsoft-teams"></a>Управление на правилата за събрание в екипи на Microsoft

**Забележка: Може да отнеме до 24 часа, за да влязат в сила промените на правилата за потребителите.** Възможно е да не можете да правите промени в новосъздадените правила незабавно; изчакайте 4 часа и се опитайте да промените новосъздадената политика отново.

Правилата за събрания се използват за управление на функциите, които са налични за срещи на участниците за събрания, които са планирани от потребители във вашата организация. Някои функции на правилата за събрание може да не бъдат приложени в центъра за администриране на Екипи все още (те са означени като "очаквайте скоро" в документацията). В този случай или ако получавате грешка като "Не можем да актуализираме правилата в момента, но опитайте отново по-късно" в центъра за администриране на Microsoft Teams, препоръчваме да използвате PowerShell за създаване или промяна на правила за събрание на Екипи. 

За повече информация относно правилата за събрание вижте следните ресурси:

- За да научите за създаването на правила, извършването на промени и присвояването на потребители на правилата, вижте Управление на правилата за [събрание в Teams](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams).

- За да промените правилата с кратки команди на PowerShell, вижте [Преглед на PowerShell на екипи](https://docs.microsoft.com/microsoftteams/teams-powershell-overview). 
    - Трябва да използвате [Skype за бизнес PowerShell модул](https://www.microsoft.com/download/details.aspx?id=39366) за правила за срещи на екипи. 
    - Прегледайте документацията за [кратки команди *-CsTeamsMeetingPolicy](https://docs.microsoft.com/search/?search=CsTeamsMeetingPolicy&view=skype-ps) за повече информация.

