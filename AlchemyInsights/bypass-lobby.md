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
# <a name="control-lobby-settings-and-level-of-participation"></a><span data-ttu-id="b725b-102">Управление на настройките на лобито и нивото на участие</span><span class="sxs-lookup"><span data-stu-id="b725b-102">Control lobby settings and level of participation</span></span>

<span data-ttu-id="b725b-103">Ако искате да позволите на всички, включително комутируема връзка, външни и анонимни потребители да заобиколят лобито, можете да използвате PowerShell, за да го направите.</span><span class="sxs-lookup"><span data-stu-id="b725b-103">If you'd like to allow everyone, including Dial-in, external, and anonymous users to bypass the lobby, you can use PowerShell to do it.</span></span> <span data-ttu-id="b725b-104">Ето един пример за модифициране на правилата за глобално събрание за вашата организация:</span><span class="sxs-lookup"><span data-stu-id="b725b-104">Here's an example of modifying the global meeting policy for your organization:</span></span>

`Set-CsTeamsMeetingPolicy -Identity Global -AutoAdmittedUsers "Everyone" -AllowPSTNUsersToBypassLobby $True`

<span data-ttu-id="b725b-105">Тази команда в момента изисква използването на Skype за бизнес PowerShell модул.</span><span class="sxs-lookup"><span data-stu-id="b725b-105">This cmdlet currently requires the use of Skype for Business PowerShell module.</span></span> <span data-ttu-id="b725b-106">За да получите настройка за използване на тази команда, вижте [управление на правила чрез PowerShell](https://docs.microsoft.com/en-us/microsoftteams/teams-powershell-overview#managing-policies-via-powershell).</span><span class="sxs-lookup"><span data-stu-id="b725b-106">To get setup to use this cmdlet, check out [Managing policies via PowerShell](https://docs.microsoft.com/en-us/microsoftteams/teams-powershell-overview#managing-policies-via-powershell).</span></span>

<span data-ttu-id="b725b-107">Можете да настроите нова политика, която след това ще трябва да я приложите към потребителите.</span><span class="sxs-lookup"><span data-stu-id="b725b-107">You can set up a new policy, which you'll then need to apply it to users.</span></span> <span data-ttu-id="b725b-108">Ако промените глобалната политика, тя ще се прилага автоматично за потребителите.</span><span class="sxs-lookup"><span data-stu-id="b725b-108">If you modify the Global policy it'll automatically apply to users.</span></span> <span data-ttu-id="b725b-109">За всяка промяна на политиката трябва да изчакате поне 4 часа и до 24 часа, за да влязат в сила правилата.</span><span class="sxs-lookup"><span data-stu-id="b725b-109">For any policy change you need to wait at least 4 hours and up to 24 hours for the policies to take effect.</span></span>

<span data-ttu-id="b725b-110">Не забравяйте да прегледате документацията по-долу, преди да направите тези промени, за да разберете точно какво позволява това.</span><span class="sxs-lookup"><span data-stu-id="b725b-110">Be sure to review the documentation below before making these changes to understand exactly what this allows.</span></span>

## <a name="understanding-teams-meeting-lobby-policy-controls"></a><span data-ttu-id="b725b-111">Разбиране на екипите за изпълнение на правилата на лобито</span><span class="sxs-lookup"><span data-stu-id="b725b-111">Understanding Teams meeting lobby policy controls</span></span>

- <span data-ttu-id="b725b-112">[Автоматично признават](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#automatically-admit-people) , че хората са правила за организатора, които контролират дали хората да се присъединят към събрание директно или да изчакат в лобито, докато не бъдат допуснати от удостоверен потребител.</span><span class="sxs-lookup"><span data-stu-id="b725b-112">[Automatically admit people](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#automatically-admit-people) is a per-organizer policy that controls whether people join a meeting directly or wait in the lobby until they are admitted by an authenticated user.</span></span>

- <span data-ttu-id="b725b-113">[Позволяване на анонимни хора да стартират среща](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#allow-anonymous-people-to-start-a-meeting) е политика за организатора, която контролира дали анонимните хора, включително B2B и външни потребители, могат да се присъединят към събранието на потребителя без удостоверен потребител от посещаемостта на организацията.</span><span class="sxs-lookup"><span data-stu-id="b725b-113">[Allow anonymous people to start a meeting](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#allow-anonymous-people-to-start-a-meeting) is a per-organizer policy that controls whether anonymous people, including B2B and federated users, can join the user's meeting without an authenticated user from the organization in attendance.</span></span>

- <span data-ttu-id="b725b-114">[Позволяване на потребителите на комутируема връзка да заобиколят лобито](https://docs.microsoft.com/en-us/microsoftteams/meeting-policies-in-teams#allow-dial-in-users-to-bypass-the-lobby-coming-soon) (**Очаквайте скоро**) е политика за организатора, която контролира дали хората, които се набират по телефона, се присъединяват към събранието директно или чакат в лобито, независимо от настройката за **автоматично допускане на хора** .</span><span class="sxs-lookup"><span data-stu-id="b725b-114">[Allow dial-in users to bypass the lobby](https://docs.microsoft.com/en-us/microsoftteams/meeting-policies-in-teams#allow-dial-in-users-to-bypass-the-lobby-coming-soon) (**coming soon**) is a per-organizer policy that controls whether people who dial in by phone join the meeting directly or wait in the lobby regardless of the **Automatically admit people** setting.</span></span>

- <span data-ttu-id="b725b-115">[Позволяване на организаторите да отменят настройките на лобито](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#allow-organizers-to-override-lobby-settings-coming-soon) (**Очаквайте скоро**) е политика на организатора, която контролира дали организаторът на събранието може да замести настройките на лобито, които администраторът е зададен автоматично, за да **признае хората** и да **позволи комутируема връзка потребителите да заобиколят лобито** , когато планират ново събрание.</span><span class="sxs-lookup"><span data-stu-id="b725b-115">[Allow organizers to override lobby settings](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#allow-organizers-to-override-lobby-settings-coming-soon) (**coming soon**) is a per-organizer policy that controls whether the meeting organizer can override the lobby settings that an admin set in **Automatically admit people** and **Allow dial-in users to bypass the lobby** when they schedule a new meeting.</span></span>

<span data-ttu-id="b725b-116">**Забележка:** Прочетете [управление на правилата за събрания в екипи](https://docs.microsoft.com/en-us/microsoftteams/meeting-policies-in-teams) за пълен преглед на правилата за срещи на Microsoft екипи.</span><span class="sxs-lookup"><span data-stu-id="b725b-116">**Note:** Read [Manage meeting policies in Teams](https://docs.microsoft.com/en-us/microsoftteams/meeting-policies-in-teams) for a complete overview of Microsoft Teams meeting policies.</span></span>
