---
title: Байпас лоби
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "2673"
- "9000740"
ms.openlocfilehash: 6632bb0c09c7ce99f14cd55582025b37a846369d
ms.sourcegitcommit: ee719f011f766fc20d23e935e98d7e33c326183b
ms.translationtype: MT
ms.contentlocale: bg-BG
ms.lasthandoff: 10/24/2019
ms.locfileid: "37654245"
---
# <a name="control-lobby-settings-and-level-of-participation"></a>Управление на настройките на лобито и нивото на участие

Ако искате да позволите на всички, включително комутируема връзка, външни и анонимни потребители да заобиколят лобито, можете да използвате PowerShell, за да го направите. Ето един пример за модифициране на правилата за глобално събрание за вашата организация:

`Set-CsTeamsMeetingPolicy -Identity Global -AutoAdmittedUsers "Everyone" -AllowPSTNUsersToBypassLobby $True`

Тази команда в момента изисква използването на Skype за бизнес PowerShell модул. За да получите настройка за използване на тази команда, вижте [управление на правила чрез PowerShell](https://docs.microsoft.com/en-us/microsoftteams/teams-powershell-overview#managing-policies-via-powershell).

Можете да настроите нова политика, която след това ще трябва да я приложите към потребителите. Ако промените глобалната политика, тя ще се прилага автоматично за потребителите. За всяка промяна на политиката трябва да изчакате поне 4 часа и до 24 часа, за да влязат в сила правилата.

Не забравяйте да прегледате документацията по-долу, преди да направите тези промени, за да разберете точно какво позволява това.

## <a name="understanding-teams-meeting-lobby-policy-controls"></a>Разбиране на екипите за изпълнение на правилата на лобито

- [Автоматично признават](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#automatically-admit-people) , че хората са правила за организатора, които контролират дали хората да се присъединят към събрание директно или да изчакат в лобито, докато не бъдат допуснати от удостоверен потребител.

- [Позволяване на анонимни хора да стартират среща](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#allow-anonymous-people-to-start-a-meeting) е политика за организатора, която контролира дали анонимните хора, включително B2B и външни потребители, могат да се присъединят към събранието на потребителя без удостоверен потребител от посещаемостта на организацията.

- [Позволяване на потребителите на комутируема връзка да заобиколят лобито](https://docs.microsoft.com/en-us/microsoftteams/meeting-policies-in-teams#allow-dial-in-users-to-bypass-the-lobby-coming-soon) (**Очаквайте скоро**) е политика за организатора, която контролира дали хората, които се набират по телефона, се присъединяват към събранието директно или чакат в лобито, независимо от настройката за **автоматично допускане на хора** .

- [Позволяване на организаторите да отменят настройките на лобито](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#allow-organizers-to-override-lobby-settings-coming-soon) (**Очаквайте скоро**) е политика на организатора, която контролира дали организаторът на събранието може да замести настройките на лобито, които администраторът е зададен автоматично, за да **признае хората** и да **позволи комутируема връзка потребителите да заобиколят лобито** , когато планират ново събрание.

**Забележка:** Прочетете [управление на правилата за събрания в екипи](https://docs.microsoft.com/en-us/microsoftteams/meeting-policies-in-teams) за пълен преглед на правилата за срещи на Microsoft екипи.
