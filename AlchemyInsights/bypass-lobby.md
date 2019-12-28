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
ms.openlocfilehash: 311af365a94b788182bb6870bca3f67b2ad802d0
ms.sourcegitcommit: 932981641dd8e973e28dfe346bbdf9c923111b13
ms.translationtype: MT
ms.contentlocale: bg-BG
ms.lasthandoff: 12/27/2019
ms.locfileid: "40889071"
---
# <a name="control-lobby-settings-and-level-of-participation-in-teams"></a><span data-ttu-id="cca03-102">Управление на настройките на лобито и нивото на участие в отборите</span><span class="sxs-lookup"><span data-stu-id="cca03-102">Control lobby settings and level of participation in Teams</span></span>

<span data-ttu-id="cca03-103">Ако искате да позволите на всички, включително комутируема връзка, външни и анонимни потребители, да **заобиколят лобито**, използвайте PowerShell, за да изпълните тази задача.</span><span class="sxs-lookup"><span data-stu-id="cca03-103">If you'd like to allow everyone, including Dial-in, external, and anonymous users, to **bypass the lobby**, use PowerShell to accomplish this task.</span></span> <span data-ttu-id="cca03-104">Ето пример за модифициране на правилата за глобално събрание за вашата организация.</span><span class="sxs-lookup"><span data-stu-id="cca03-104">Here's an example of modifying the global meeting policy for your organization.</span></span>

`Set-CsTeamsMeetingPolicy -Identity Global -AutoAdmittedUsers "Everyone" -AllowPSTNUsersToBypassLobby $True`

<span data-ttu-id="cca03-105">Тази команда в момента изисква използването на Skype за бизнес PowerShell модул.</span><span class="sxs-lookup"><span data-stu-id="cca03-105">This cmdlet currently requires the use of Skype for Business PowerShell module.</span></span> <span data-ttu-id="cca03-106">За да се настроите да използвате тази команда, вижте [управление на правила чрез PowerShell](https://docs.microsoft.com/microsoftteams/teams-powershell-overview#managing-policies-via-powershell).</span><span class="sxs-lookup"><span data-stu-id="cca03-106">To get set up to use this cmdlet, check out [Managing policies via PowerShell](https://docs.microsoft.com/microsoftteams/teams-powershell-overview#managing-policies-via-powershell).</span></span>

<span data-ttu-id="cca03-107">След като сте настроили правила, трябва да я приложите към потребителите; или, ако сте променили глобалната политика, тя ще се прилага автоматично за потребителите.</span><span class="sxs-lookup"><span data-stu-id="cca03-107">Once you’ve set up a policy, you need to apply it to users; or, if you modified the Global policy, it will automatically apply to users.</span></span> <span data-ttu-id="cca03-108">За всяка промяна в правилата трябва да изчакате поне **4 часа до 24 часа** , за да влязат в сила правилата.</span><span class="sxs-lookup"><span data-stu-id="cca03-108">For any policy change, you need to wait at least **4 hours up to 24 hours** for the policies to take effect.</span></span> 

<span data-ttu-id="cca03-109">Не забравяйте да прегледате документацията по-долу, преди да направите тези промени, за да разберете точно какво позволява това.</span><span class="sxs-lookup"><span data-stu-id="cca03-109">Be sure to review the documentation below before making these changes to understand exactly what this allows.</span></span>


## <a name="understanding-teams-meeting-lobby-policy-controls"></a><span data-ttu-id="cca03-110">Разбиране на екипите за изпълнение на правилата на лобито</span><span class="sxs-lookup"><span data-stu-id="cca03-110">Understanding Teams meeting lobby policy controls</span></span>

<span data-ttu-id="cca03-111">Тези настройки контролират кои участници в събранието чакат в лобито, преди да бъдат допуснати до събранието, и нивото на участие, което са позволени в събранието.</span><span class="sxs-lookup"><span data-stu-id="cca03-111">These settings control which meeting participants wait in the lobby before they are admitted to the meeting and the level of participation they are allowed in a meeting.</span></span> <span data-ttu-id="cca03-112">Можете да използвате PowerShell, за да актуализирате настройките на правилата за събрания, които все още не са изпълнени (с надпис "Очаквайте скоро") в центъра за администриране на екипите.</span><span class="sxs-lookup"><span data-stu-id="cca03-112">You can use PowerShell to update meeting policy settings that haven't yet been implemented (labeled "coming soon") in the Teams admin center.</span></span> <span data-ttu-id="cca03-113">Вижте по-долу за пример PowerShell команда, която позволява на всички потребители да заобиколят лобито.</span><span class="sxs-lookup"><span data-stu-id="cca03-113">See below for an example PowerShell cmdlet that allows all users to bypass the lobby.</span></span>

- <span data-ttu-id="cca03-114">[Автоматично признават](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#automatically-admit-people) , че хората са правила за организатора, които контролират дали хората да се присъединят към събрание директно или да изчакат в лобито, докато не бъдат допуснати от удостоверен потребител.</span><span class="sxs-lookup"><span data-stu-id="cca03-114">[Automatically admit people](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#automatically-admit-people) is a per-organizer policy that controls whether people join a meeting directly or wait in the lobby until they are admitted by an authenticated user.</span></span>

- <span data-ttu-id="cca03-115">[Позволяване на анонимни хора да стартират среща](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#allow-anonymous-people-to-start-a-meeting) е политика за организатора, която контролира дали анонимните хора, включително B2B и външни потребители, могат да се присъединят към събранието на потребителя без удостоверен потребител от посещаемостта на организацията.</span><span class="sxs-lookup"><span data-stu-id="cca03-115">[Allow anonymous people to start a meeting](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#allow-anonymous-people-to-start-a-meeting) is a per-organizer policy that controls whether anonymous people, including B2B and federated users, can join the user's meeting without an authenticated user from the organization in attendance.</span></span>

- <span data-ttu-id="cca03-116">[Позволяване на потребителите на комутируема връзка да заобиколят лобито](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#allow-dial-in-users-to-bypass-the-lobby-coming-soon) (**Очаквайте скоро**) е политика за организатора, която контролира дали хората, които се набират по телефона, се присъединяват към събранието директно или чакат в лобито, независимо от настройката за **автоматично допускане на хора** .</span><span class="sxs-lookup"><span data-stu-id="cca03-116">[Allow dial-in users to bypass the lobby](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#allow-dial-in-users-to-bypass-the-lobby-coming-soon) (**coming soon**) is a per-organizer policy that controls whether people who dial in by phone join the meeting directly or wait in the lobby regardless of the **Automatically admit people** setting.</span></span>

- <span data-ttu-id="cca03-117">[Позволяване на организаторите да отменят настройките на лобито](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#allow-organizers-to-override-lobby-settings-coming-soon) (**Очаквайте скоро**) е политика на организатора, която контролира дали организаторът на събранието може да замести настройките на лобито, които администраторът е зададен автоматично, за да **признае хората** и **да позволи на потребителите на комутируема връзка да заобиколят лобито** , когато планират ново събрание.</span><span class="sxs-lookup"><span data-stu-id="cca03-117">[Allow organizers to override lobby settings](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#allow-organizers-to-override-lobby-settings-coming-soon) (**coming soon**) is a per-organizer policy that controls whether the meeting organizer can override the lobby settings that an admin set in **Automatically admit people** and **Allow dial-in users to bypass the lobby** when they schedule a new meeting.</span></span>

<span data-ttu-id="cca03-118">**Забележка:** Прочетете [управление на правилата за събрания в екипи](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams) за пълен преглед на правилата за срещи на Microsoft екипи.</span><span class="sxs-lookup"><span data-stu-id="cca03-118">**Note:** Read [Manage meeting policies in Teams](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams) for a complete overview of Microsoft Teams meeting policies.</span></span>
