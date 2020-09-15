---
title: Обхождане на фоайето
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
- "2673"
- "9000740"
ms.openlocfilehash: 44a930355f1faf8ad747885b72753aaeeb80a6f0
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: bg-BG
ms.lasthandoff: 09/14/2020
ms.locfileid: "47684939"
---
# <a name="control-lobby-settings-and-level-of-participation-in-teams"></a>Управление на настройки за фоайе и ниво на участие в Teams

Ако искате да позволите на всички, включително външни и анонимни потребители да **заобикалят фоайето**, използвайте PowerShell, за да изпълните тази задача. Ето един пример за модифициране на правилата за глобално събрание за вашата организация.

`Set-CsTeamsMeetingPolicy -Identity Global -AutoAdmittedUsers "Everyone" -AllowPSTNUsersToBypassLobby $True`

Тази кратка команда в момента изисква използването на модула на PowerShell за Skype за бизнеса. За да се подготвите да използвате тази кратка команда, прегледайте [управление на правила чрез PowerShell](https://docs.microsoft.com/microsoftteams/teams-powershell-overview#managing-policies-via-powershell).

След като сте настроили правила, трябва да я приложите към потребители; а ако сте променили глобалните правила, те ще се прилагат автоматично към потребителите. За всяка промяна на правилата трябва да изчакате най-малко **4 часа до 24 часа** , за да влязат в сила правилата. 

Не забравяйте да прегледате документацията по-долу, преди да направите тези промени, за да разберете точно какво позволява това.


## <a name="understanding-teams-meeting-lobby-policy-controls"></a>Запознаване с контролите за правилата за събрания на Teams

Тези настройки контролират кои участници в събранието изчакват във фоайето, преди да бъдат допуснати до събранието и нивото на участие, което са позволени в събранието. Можете да използвате PowerShell, за да актуализирате настройките за правилата за събрания, които още не са изпълнени (означени като "Очаквайте скоро") в центъра за администриране на Teams. Вижте по-долу за команда на PowerShell за пример, която позволява на всички потребители да заобикалят фоайето.

- [Автоматично](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#automatically-admit-people) приемане на хора е политика на организатора, която контролира дали хората се присъединяват към събранието директно или изчакват във фоайето, докато не бъдат допуснати от удостоверен потребител.

- [Разрешаване на анонимни хора да започнат събрание](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#allow-anonymous-people-to-start-a-meeting) е политика на организатора, която контролира дали анонимните хора, включително B2B и външни потребители, могат да се присъединят към събранието на потребителя, без да има удостоверен потребител от организацията в обслужването.

- [Позволяване на потребители с външно избиране да заобикалят фоайето](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#allow-dial-in-users-to-bypass-the-lobby-coming-soon) (**Очаквайте скоро**) е политика на организатора, която контролира дали хората, които се обаждат по телефона, се присъединяват към събранието директно или изчакват във фоайето, независимо от настройката за автоматично приемане на **хора** .

- [Позволи на организаторите да заместят настройките за фоайе](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#allow-organizers-to-override-lobby-settings-coming-soon) (**Очаквайте скоро**) е политика на организатора, която контролира дали организаторът на събранието може да замести настройките за лобито, зададени от администратора, за автоматично приемане на **хора** и **Позволяване на потребители с външно избиране да заобикалят фоайето** , когато планират ново събрание.

**Забележка:** Прочетете [правилата за управление на събрания в Teams](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams) , за да видите пълен преглед на правилата за събрания в Microsoft Teams.
