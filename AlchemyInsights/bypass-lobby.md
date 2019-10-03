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
ms.openlocfilehash: de665ca6defcd0d00d227435473e5a4ccf61bc82
ms.sourcegitcommit: 0495112ad4fd0e695140ec66d190e62f03030584
ms.translationtype: MT
ms.contentlocale: bg-BG
ms.lasthandoff: 10/02/2019
ms.locfileid: "37376525"
---
# <a name="control-lobby-settings-and-level-of-participation"></a><span data-ttu-id="fc1fd-102">Управление на настройките на лобито и нивото на участие</span><span class="sxs-lookup"><span data-stu-id="fc1fd-102">Control lobby settings and level of participation</span></span>

<span data-ttu-id="fc1fd-103">Тези настройки контролират кои участници в събранието чакат в лобито, преди да бъдат допуснати до събранието, и нивото на участие, което са позволени в събранието.</span><span class="sxs-lookup"><span data-stu-id="fc1fd-103">These settings control which meeting participants wait in the lobby before they are admitted to the meeting and the level of participation they are allowed in a meeting.</span></span> <span data-ttu-id="fc1fd-104">Можете да използвате PowerShell да актуализирате настройките на правилата за събрания, които все още не са изпълнени (с надпис "Очаквайте скоро") в центъра за администриране на екипите.</span><span class="sxs-lookup"><span data-stu-id="fc1fd-104">You can use Powershell to update meeting policy settings that haven't yet been implemented (labeled "coming soon") in the Teams admin center.</span></span>  <span data-ttu-id="fc1fd-105">Вижте по-долу за пример PowerShell команда, която позволява на всички потребители да заобиколят лобито.</span><span class="sxs-lookup"><span data-stu-id="fc1fd-105">See below for an example PowerShell cmdlet that allows all users to bypass the lobby.</span></span>  

- <span data-ttu-id="fc1fd-106">[Автоматично признават](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#automatically-admit-people) , че хората са правила за организатора, които контролират дали хората да се присъединят към събрание директно или да изчакат в лобито, докато не бъдат допуснати от удостоверен потребител.</span><span class="sxs-lookup"><span data-stu-id="fc1fd-106">[Automatically admit people](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#automatically-admit-people) is a per-organizer policy that controls whether people join a meeting directly or wait in the lobby until they are admitted by an authenticated user.</span></span>

- <span data-ttu-id="fc1fd-107">[Позволяване на анонимни хора да стартират среща](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#allow-anonymous-people-to-start-a-meeting) е политика за организатора, която контролира дали анонимните хора, включително B2B и външни потребители, могат да се присъединят към събранието на потребителя без удостоверен потребител от посещаемостта на организацията.</span><span class="sxs-lookup"><span data-stu-id="fc1fd-107">[Allow anonymous people to start a meeting](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#allow-anonymous-people-to-start-a-meeting) is a per-organizer policy that controls whether anonymous people, including B2B and federated users, can join the user's meeting without an authenticated user from the organization in attendance.</span></span>

- <span data-ttu-id="fc1fd-108">[Позволяване на потребителите на комутируема връзка да заобиколят лобито](https://docs.microsoft.com/en-us/microsoftteams/meeting-policies-in-teams#allow-dial-in-users-to-bypass-the-lobby-coming-soon) (**Очаквайте скоро**) е политика за организатора, която контролира дали хората, които се набират по телефона, се присъединяват към събранието директно или чакат в лобито, независимо от настройката за **автоматично допускане на хора** .</span><span class="sxs-lookup"><span data-stu-id="fc1fd-108">[Allow dial-in users to bypass the lobby](https://docs.microsoft.com/en-us/microsoftteams/meeting-policies-in-teams#allow-dial-in-users-to-bypass-the-lobby-coming-soon) (**coming soon**) is a per-organizer policy that controls whether people who dial in by phone join the meeting directly or wait in the lobby regardless of the **Automatically admit people** setting.</span></span>

- <span data-ttu-id="fc1fd-109">[Позволяване на организаторите да отменят настройките на лобито](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#allow-organizers-to-override-lobby-settings-coming-soon) (**Очаквайте скоро**) е политика на организатора, която контролира дали организаторът на събранието може да замести настройките на лобито, които администраторът е зададен автоматично, за да **признае хората** и да **позволи комутируема връзка потребителите да заобиколят лобито** , когато планират ново събрание.</span><span class="sxs-lookup"><span data-stu-id="fc1fd-109">[Allow organizers to override lobby settings](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#allow-organizers-to-override-lobby-settings-coming-soon) (**coming soon**) is a per-organizer policy that controls whether the meeting organizer can override the lobby settings that an admin set in **Automatically admit people** and **Allow dial-in users to bypass the lobby** when they schedule a new meeting.</span></span>

<span data-ttu-id="fc1fd-110">**Забележка:** Прочетете [управление на правилата за събрания в екипи](https://docs.microsoft.com/en-us/microsoftteams/meeting-policies-in-teams) за пълен преглед на правилата за срещи на Microsoft екипи.</span><span class="sxs-lookup"><span data-stu-id="fc1fd-110">**Note:** Read [Manage meeting policies in Teams](https://docs.microsoft.com/en-us/microsoftteams/meeting-policies-in-teams) for a complete overview of Microsoft Teams meeting policies.</span></span> 


<span data-ttu-id="fc1fd-111">**Пример за PowerShell**</span><span class="sxs-lookup"><span data-stu-id="fc1fd-111">**PowerShell example**</span></span>

<span data-ttu-id="fc1fd-112">Ако искате да позволите на всички, включително външни или анонимни потребители, да заобиколят лобито, можете да използвате и PowerShell, за да постигнете тази задача.</span><span class="sxs-lookup"><span data-stu-id="fc1fd-112">If you'd like to allow everyone, including external or anonymous users, to bypass the lobby, you can also use PowerShell to accomplish this task.</span></span>  <span data-ttu-id="fc1fd-113">Ето пример за модифициране на правилата за глобално събрание за вашата организация.</span><span class="sxs-lookup"><span data-stu-id="fc1fd-113">Here's an example of modifying the global meeting policy for your organization.</span></span>   

<span data-ttu-id="fc1fd-114">(Не забравяйте да прегледате документацията по-горе, преди да направите тези промени, за да разберете точно какво позволява това.)</span><span class="sxs-lookup"><span data-stu-id="fc1fd-114">(Be sure to review the documentation above before making these changes to understand exactly what this allows.)</span></span>

<span data-ttu-id="fc1fd-115">Set-Ппарапарцияполитика-идентичност глобално-автоматично призна потребителите "всички"-Алловпстнусерстобипасслобби $True</span><span class="sxs-lookup"><span data-stu-id="fc1fd-115">Set-CsTeamsMeetingPolicy -Identity Global -AutoAdmittedUsers "Everyone" -AllowPSTNUsersToBypassLobby $True</span></span>

<span data-ttu-id="fc1fd-116">За повече [информация вж.](https://docs.microsoft.com/powershell/module/skype/set-csteamsmeetingpolicy?view=skype-ps)</span><span class="sxs-lookup"><span data-stu-id="fc1fd-116">For more information, see [Set-CsTeamsMeetingPolicy](https://docs.microsoft.com/powershell/module/skype/set-csteamsmeetingpolicy?view=skype-ps).</span></span>
