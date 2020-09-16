---
title: Настройки на правилата за събранието
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
- "9000734"
- "2657"
ms.openlocfilehash: 683ca12c8f6e2511311c10ab5c4599ee66c08eb8
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: bg-BG
ms.lasthandoff: 09/15/2020
ms.locfileid: "47794323"
---
# <a name="manage-meeting-policies-in-microsoft-teams"></a>Управление на правила за събрания в Microsoft Teams

**Забележка: възможно е да са необходими до 24 часа, за да влязат в сила промените в правилата за потребителите.** Възможно е да не можете да правите промени в току-що създадените правила незабавно; Изчакайте 4 часа и се опитайте отново да промените ново създадената политика.

Правилата за събрания се използват за управление на функциите, които са достъпни за участниците в събранието, за събрания, които са планирани от потребители във вашата организация. Някои функции на правилата за събрания може да не бъдат реализирани в центъра за администриране на екипи все още (те са означени с "Очаквайте скоро" в документацията). В този случай или ако получавате съобщение за грешка като "не можем да актуализираме правилата в момента, но опитайте отново по-късно" в центъра за администриране на Microsoft Teams, ви препоръчваме да използвате PowerShell, за да създавате или модифицирате правила за събрания в Teams. 

За повече информация относно правилата за събрания вижте следните ресурси:

- За да научите повече за създаването на правила, извършването на промени и присвояването на потребители на правилата, вижте [управление на правилата за събрания в Teams](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams).

- За да направите промени в правилата с помощта на кратки команди на PowerShell, вижте [общ преглед на PowerShell за Teams](https://docs.microsoft.com/microsoftteams/teams-powershell-overview). 
    - Трябва да използвате модула на [Skype за бизнеса PowerShell](https://www.microsoft.com/download/details.aspx?id=39366) за правилата за събрания в Teams. 
    - Прегледайте [документацията * – CsTeamsMeetingPolicy кратки команди](https://docs.microsoft.com/search/?search=CsTeamsMeetingPolicy&view=skype-ps) за повече информация.

