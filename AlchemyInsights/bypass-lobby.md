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
# <a name="control-lobby-settings-and-level-of-participation-in-teams"></a><span data-ttu-id="7f710-102">Управление на настройки за фоайе и ниво на участие в Teams</span><span class="sxs-lookup"><span data-stu-id="7f710-102">Control lobby settings and level of participation in Teams</span></span>

<span data-ttu-id="7f710-103">Ако искате да позволите на всички, включително външни и анонимни потребители да **заобикалят фоайето**, използвайте PowerShell, за да изпълните тази задача.</span><span class="sxs-lookup"><span data-stu-id="7f710-103">If you'd like to allow everyone, including Dial-in, external, and anonymous users, to **bypass the lobby**, use PowerShell to accomplish this task.</span></span> <span data-ttu-id="7f710-104">Ето един пример за модифициране на правилата за глобално събрание за вашата организация.</span><span class="sxs-lookup"><span data-stu-id="7f710-104">Here's an example of modifying the global meeting policy for your organization.</span></span>

`Set-CsTeamsMeetingPolicy -Identity Global -AutoAdmittedUsers "Everyone" -AllowPSTNUsersToBypassLobby $True`

<span data-ttu-id="7f710-105">Тази кратка команда в момента изисква използването на модула на PowerShell за Skype за бизнеса.</span><span class="sxs-lookup"><span data-stu-id="7f710-105">This cmdlet currently requires the use of Skype for Business PowerShell module.</span></span> <span data-ttu-id="7f710-106">За да се подготвите да използвате тази кратка команда, прегледайте [управление на правила чрез PowerShell](https://docs.microsoft.com/microsoftteams/teams-powershell-overview#managing-policies-via-powershell).</span><span class="sxs-lookup"><span data-stu-id="7f710-106">To get set up to use this cmdlet, check out [Managing policies via PowerShell](https://docs.microsoft.com/microsoftteams/teams-powershell-overview#managing-policies-via-powershell).</span></span>

<span data-ttu-id="7f710-107">След като сте настроили правила, трябва да я приложите към потребители; а ако сте променили глобалните правила, те ще се прилагат автоматично към потребителите.</span><span class="sxs-lookup"><span data-stu-id="7f710-107">Once you’ve set up a policy, you need to apply it to users; or, if you modified the Global policy, it will automatically apply to users.</span></span> <span data-ttu-id="7f710-108">За всяка промяна на правилата трябва да изчакате най-малко **4 часа до 24 часа** , за да влязат в сила правилата.</span><span class="sxs-lookup"><span data-stu-id="7f710-108">For any policy change, you need to wait at least **4 hours up to 24 hours** for the policies to take effect.</span></span> 

<span data-ttu-id="7f710-109">Не забравяйте да прегледате документацията по-долу, преди да направите тези промени, за да разберете точно какво позволява това.</span><span class="sxs-lookup"><span data-stu-id="7f710-109">Be sure to review the documentation below before making these changes to understand exactly what this allows.</span></span>


## <a name="understanding-teams-meeting-lobby-policy-controls"></a><span data-ttu-id="7f710-110">Запознаване с контролите за правилата за събрания на Teams</span><span class="sxs-lookup"><span data-stu-id="7f710-110">Understanding Teams meeting lobby policy controls</span></span>

<span data-ttu-id="7f710-111">Тези настройки контролират кои участници в събранието изчакват във фоайето, преди да бъдат допуснати до събранието и нивото на участие, което са позволени в събранието.</span><span class="sxs-lookup"><span data-stu-id="7f710-111">These settings control which meeting participants wait in the lobby before they are admitted to the meeting and the level of participation they are allowed in a meeting.</span></span> <span data-ttu-id="7f710-112">Можете да използвате PowerShell, за да актуализирате настройките за правилата за събрания, които още не са изпълнени (означени като "Очаквайте скоро") в центъра за администриране на Teams.</span><span class="sxs-lookup"><span data-stu-id="7f710-112">You can use PowerShell to update meeting policy settings that haven't yet been implemented (labeled "coming soon") in the Teams admin center.</span></span> <span data-ttu-id="7f710-113">Вижте по-долу за команда на PowerShell за пример, която позволява на всички потребители да заобикалят фоайето.</span><span class="sxs-lookup"><span data-stu-id="7f710-113">See below for an example PowerShell cmdlet that allows all users to bypass the lobby.</span></span>

- <span data-ttu-id="7f710-114">[Автоматично](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#automatically-admit-people) приемане на хора е политика на организатора, която контролира дали хората се присъединяват към събранието директно или изчакват във фоайето, докато не бъдат допуснати от удостоверен потребител.</span><span class="sxs-lookup"><span data-stu-id="7f710-114">[Automatically admit people](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#automatically-admit-people) is a per-organizer policy that controls whether people join a meeting directly or wait in the lobby until they are admitted by an authenticated user.</span></span>

- <span data-ttu-id="7f710-115">[Разрешаване на анонимни хора да започнат събрание](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#allow-anonymous-people-to-start-a-meeting) е политика на организатора, която контролира дали анонимните хора, включително B2B и външни потребители, могат да се присъединят към събранието на потребителя, без да има удостоверен потребител от организацията в обслужването.</span><span class="sxs-lookup"><span data-stu-id="7f710-115">[Allow anonymous people to start a meeting](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#allow-anonymous-people-to-start-a-meeting) is a per-organizer policy that controls whether anonymous people, including B2B and federated users, can join the user's meeting without an authenticated user from the organization in attendance.</span></span>

- <span data-ttu-id="7f710-116">[Позволяване на потребители с външно избиране да заобикалят фоайето](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#allow-dial-in-users-to-bypass-the-lobby-coming-soon) (**Очаквайте скоро**) е политика на организатора, която контролира дали хората, които се обаждат по телефона, се присъединяват към събранието директно или изчакват във фоайето, независимо от настройката за автоматично приемане на **хора** .</span><span class="sxs-lookup"><span data-stu-id="7f710-116">[Allow dial-in users to bypass the lobby](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#allow-dial-in-users-to-bypass-the-lobby-coming-soon) (**coming soon**) is a per-organizer policy that controls whether people who dial in by phone join the meeting directly or wait in the lobby regardless of the **Automatically admit people** setting.</span></span>

- <span data-ttu-id="7f710-117">[Позволи на организаторите да заместят настройките за фоайе](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#allow-organizers-to-override-lobby-settings-coming-soon) (**Очаквайте скоро**) е политика на организатора, която контролира дали организаторът на събранието може да замести настройките за лобито, зададени от администратора, за автоматично приемане на **хора** и **Позволяване на потребители с външно избиране да заобикалят фоайето** , когато планират ново събрание.</span><span class="sxs-lookup"><span data-stu-id="7f710-117">[Allow organizers to override lobby settings](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#allow-organizers-to-override-lobby-settings-coming-soon) (**coming soon**) is a per-organizer policy that controls whether the meeting organizer can override the lobby settings that an admin set in **Automatically admit people** and **Allow dial-in users to bypass the lobby** when they schedule a new meeting.</span></span>

<span data-ttu-id="7f710-118">**Забележка:** Прочетете [правилата за управление на събрания в Teams](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams) , за да видите пълен преглед на правилата за събрания в Microsoft Teams.</span><span class="sxs-lookup"><span data-stu-id="7f710-118">**Note:** Read [Manage meeting policies in Teams](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams) for a complete overview of Microsoft Teams meeting policies.</span></span>
