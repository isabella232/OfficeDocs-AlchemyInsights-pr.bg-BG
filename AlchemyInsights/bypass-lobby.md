---
title: Заобикаляне на фоайето
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
- "2673"
- "9000740"
ms.openlocfilehash: bcb40c6f15e957c0a59911322c3b28f03cd562c1
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: bg-BG
ms.lasthandoff: 04/15/2021
ms.locfileid: "51820023"
---
# <a name="control-lobby-settings-and-level-of-participation-in-teams"></a><span data-ttu-id="2662f-102">Управление на настройките на фоайето и ниво на участие в Teams</span><span class="sxs-lookup"><span data-stu-id="2662f-102">Control lobby settings and level of participation in Teams</span></span>

<span data-ttu-id="2662f-103">Ако искате да позволите на всички, включително потребители с външно избиране, външни и анонимни потребители, да заобикалят **фоайето**, използвайте PowerShell, за да изпълните тази задача.</span><span class="sxs-lookup"><span data-stu-id="2662f-103">If you'd like to allow everyone, including Dial-in, external, and anonymous users, to **bypass the lobby**, use PowerShell to accomplish this task.</span></span> <span data-ttu-id="2662f-104">Ето пример за промяна на правилата за глобално събрание за вашата организация.</span><span class="sxs-lookup"><span data-stu-id="2662f-104">Here's an example of modifying the global meeting policy for your organization.</span></span>

`Set-CsTeamsMeetingPolicy -Identity Global -AutoAdmittedUsers "Everyone" -AllowPSTNUsersToBypassLobby $True`

<span data-ttu-id="2662f-105">Тази кратка команда в момента изисква използването на модула на PowerShell на Skype за бизнеса.</span><span class="sxs-lookup"><span data-stu-id="2662f-105">This cmdlet currently requires the use of Skype for Business PowerShell module.</span></span> <span data-ttu-id="2662f-106">За да се настроите да използвате тази кратка команда, прегледайте [Управление на правилата чрез PowerShell.](https://docs.microsoft.com/microsoftteams/teams-powershell-overview#managing-policies-via-powershell)</span><span class="sxs-lookup"><span data-stu-id="2662f-106">To get set up to use this cmdlet, check out [Managing policies via PowerShell](https://docs.microsoft.com/microsoftteams/teams-powershell-overview#managing-policies-via-powershell).</span></span>

<span data-ttu-id="2662f-107">След като настроите правило, трябва да го приложите към потребителите; или, ако сте променили глобалните правила, те автоматично ще важат за потребителите.</span><span class="sxs-lookup"><span data-stu-id="2662f-107">Once you’ve set up a policy, you need to apply it to users; or, if you modified the Global policy, it will automatically apply to users.</span></span> <span data-ttu-id="2662f-108">За всяка промяна на правилата трябва да изчакате най-малко **4 часа до 24 часа, за** да важат правилата.</span><span class="sxs-lookup"><span data-stu-id="2662f-108">For any policy change, you need to wait at least **4 hours up to 24 hours** for the policies to take effect.</span></span> 

<span data-ttu-id="2662f-109">Не забравяйте да прегледате документацията по-долу, преди да направите тези промени, за да разберете точно какво позволява това.</span><span class="sxs-lookup"><span data-stu-id="2662f-109">Be sure to review the documentation below before making these changes to understand exactly what this allows.</span></span>


## <a name="understanding-teams-meeting-lobby-policy-controls"></a><span data-ttu-id="2662f-110">Разбиране на контролите за правила за лобито на събранието на Teams</span><span class="sxs-lookup"><span data-stu-id="2662f-110">Understanding Teams meeting lobby policy controls</span></span>

<span data-ttu-id="2662f-111">Тези настройки контролират кои участници в събранието чакат във фоайето, преди да бъдат допуснати до събранието, и нивото на участие, което им е разрешено в събрание.</span><span class="sxs-lookup"><span data-stu-id="2662f-111">These settings control which meeting participants wait in the lobby before they are admitted to the meeting and the level of participation they are allowed in a meeting.</span></span> <span data-ttu-id="2662f-112">Можете да използвате PowerShell, за да актуализирате настройките на правилата за събрание, които все още не са внедрени (с етикет "очаквайте скоро") в центъра за администриране на Teams.</span><span class="sxs-lookup"><span data-stu-id="2662f-112">You can use PowerShell to update meeting policy settings that haven't yet been implemented (labeled "coming soon") in the Teams admin center.</span></span> <span data-ttu-id="2662f-113">Вижте по-долу за пример кратка команда на PowerShell, която позволява на всички потребители да заобикалят фоайето.</span><span class="sxs-lookup"><span data-stu-id="2662f-113">See below for an example PowerShell cmdlet that allows all users to bypass the lobby.</span></span>

- <span data-ttu-id="2662f-114">[Автоматичното приемане на](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#automatically-admit-people) хора е правило за организатор, което контролира дали хората се присъединяват към събрание директно, или чакат във фоайето, докато не бъдат допуснати от удостоверен потребител.</span><span class="sxs-lookup"><span data-stu-id="2662f-114">[Automatically admit people](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#automatically-admit-people) is a per-organizer policy that controls whether people join a meeting directly or wait in the lobby until they are admitted by an authenticated user.</span></span>

- <span data-ttu-id="2662f-115">[Позволяване на анонимни](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#allow-anonymous-people-to-start-a-meeting) хора да стартират събрание е правило за всеки организатор, което контролира дали анонимни хора, включително B2B и федерирани потребители, могат да се присъединят към събранието на потребителя без удостоверен потребител от организацията в присъствие.</span><span class="sxs-lookup"><span data-stu-id="2662f-115">[Allow anonymous people to start a meeting](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#allow-anonymous-people-to-start-a-meeting) is a per-organizer policy that controls whether anonymous people, including B2B and federated users, can join the user's meeting without an authenticated user from the organization in attendance.</span></span>

- <span data-ttu-id="2662f-116">[Позволяване на потребителите с](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#allow-dial-in-users-to-bypass-the-lobby-coming-soon) комутируема връзка да заобикалят фоайето **(очаквайте** скоро) е правило за всеки организатор, което определя дали хората, които се набират по телефона, се присъединяват към събранието директно или чакат във фоайето, независимо от настройката Автоматично приемане **на** хора.</span><span class="sxs-lookup"><span data-stu-id="2662f-116">[Allow dial-in users to bypass the lobby](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#allow-dial-in-users-to-bypass-the-lobby-coming-soon) (**coming soon**) is a per-organizer policy that controls whether people who dial in by phone join the meeting directly or wait in the lobby regardless of the **Automatically admit people** setting.</span></span>

- <span data-ttu-id="2662f-117">[Позволяване на организаторите](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#allow-organizers-to-override-lobby-settings-coming-soon) да заместват настройките на **фоайето**(очаквайте скоро) е правило за всеки  организатор, което  определя дали организаторът на събранието може да замести настройките на фоайето, които администраторът е задали в Автоматично допускане на хора и Позволяване на потребители с набиране да заобикалят фоайето, когато планират ново събрание.</span><span class="sxs-lookup"><span data-stu-id="2662f-117">[Allow organizers to override lobby settings](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#allow-organizers-to-override-lobby-settings-coming-soon) (**coming soon**) is a per-organizer policy that controls whether the meeting organizer can override the lobby settings that an admin set in **Automatically admit people** and **Allow dial-in users to bypass the lobby** when they schedule a new meeting.</span></span>

<span data-ttu-id="2662f-118">**Забележка:** Прочетете [Управление на правилата за събрания в Teams](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams) за пълен преглед на правилата за събрания на Microsoft Teams.</span><span class="sxs-lookup"><span data-stu-id="2662f-118">**Note:** Read [Manage meeting policies in Teams](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams) for a complete overview of Microsoft Teams meeting policies.</span></span>
