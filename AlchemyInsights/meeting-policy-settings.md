---
title: Настройки на правилата за събрание
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
- "9000734"
- "2657"
ms.openlocfilehash: 39151d3a56cc09a8ae2dd77fb7bf1e99066cc77a
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: bg-BG
ms.lasthandoff: 04/15/2021
ms.locfileid: "51825432"
---
# <a name="manage-meeting-policies-in-microsoft-teams"></a>Управление на правилата за събрания в Microsoft Teams

**Забележка: Може да отнеме до 24 часа, за да влязат в сила промените в правилата за потребителите.** Възможно е да не можете да правите промени в новосъздадените правила веднага; изчакайте 4 часа и опитайте да промените новосъздадените правила отново.

Правилата за събрания се използват за управление на функциите, които са налични за участниците в събранието за събрания, които са планирани от потребителите във вашата организация. Някои функции на правилата за събрания може все още да не се внедлят в центъра за администриране на Teams (те са обозначени като "очаквайте скоро" в документацията). В този случай или ако получавате грешка като "В момента не можем да актуализираме правилата, но да го изпробваме отново по-късно" в центъра за администриране на Microsoft Teams ви препоръчваме да използвате PowerShell, за да създавате или променяте правила за събрания на Teams. 

За повече информация относно правилата за събрания вижте следните ресурси:

- За да научите за създаването на правила, извършването на промени и присвояването на потребители на правилата, вижте Управление [на правила за събрания в Teams](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams).

- За да направите промени в правилата с помощта на кратки команди на PowerShell, вижте Общ [преглед на PowerShell на Teams](https://docs.microsoft.com/microsoftteams/teams-powershell-overview). 
    - Трябва да използвате модула [на PowerShell на Skype за бизнеса за правилата](https://docs.microsoft.com/skypeforbusiness/set-up-your-computer-for-windows-powershell/download-and-install-the-skype-for-business-online-connector) за събрания на Teams. 
    - Прегледайте документацията на кратките команди [*-CsTeamsMeetingPolicy](https://docs.microsoft.com/search/?search=CsTeamsMeetingPolicy&view=skype-ps) за повече информация.

