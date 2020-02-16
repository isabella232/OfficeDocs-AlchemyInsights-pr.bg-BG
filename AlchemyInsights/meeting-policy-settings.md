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
# <a name="manage-meeting-policies-in-microsoft-teams"></a><span data-ttu-id="e1712-102">Управление на правилата за събрание в екипи на Microsoft</span><span class="sxs-lookup"><span data-stu-id="e1712-102">Manage meeting policies in Microsoft Teams</span></span>

<span data-ttu-id="e1712-103">**Забележка: Може да отнеме до 24 часа, за да влязат в сила промените на правилата за потребителите.**</span><span class="sxs-lookup"><span data-stu-id="e1712-103">**Note: It can take up to 24 hours for policy changes to take effect for users.**</span></span> <span data-ttu-id="e1712-104">Възможно е да не можете да правите промени в новосъздадените правила незабавно; изчакайте 4 часа и се опитайте да промените новосъздадената политика отново.</span><span class="sxs-lookup"><span data-stu-id="e1712-104">You might not be able to make changes to newly created policies immediately; wait 4 hours and attempt to modify a newly created policy again.</span></span>

<span data-ttu-id="e1712-105">Правилата за събрания се използват за управление на функциите, които са налични за срещи на участниците за събрания, които са планирани от потребители във вашата организация.</span><span class="sxs-lookup"><span data-stu-id="e1712-105">Meeting policies are used to control the features that are available to meeting participants for meetings that are scheduled by users in your organization.</span></span> <span data-ttu-id="e1712-106">Някои функции на правилата за събрание може да не бъдат приложени в центъра за администриране на Екипи все още (те са означени като "очаквайте скоро" в документацията).</span><span class="sxs-lookup"><span data-stu-id="e1712-106">Some features of meeting policies might not be implemented in the Teams admin center yet (these are labeled "coming soon" in the documentation).</span></span> <span data-ttu-id="e1712-107">В този случай или ако получавате грешка като "Не можем да актуализираме правилата в момента, но опитайте отново по-късно" в центъра за администриране на Microsoft Teams, препоръчваме да използвате PowerShell за създаване или промяна на правила за събрание на Екипи.</span><span class="sxs-lookup"><span data-stu-id="e1712-107">In this case, or if you are getting an error like "We can't update the policy right now but try it again later" in the Microsoft Teams admin center, we recommend that you use PowerShell to create or modify Teams meeting policies.</span></span> 

<span data-ttu-id="e1712-108">За повече информация относно правилата за събрание вижте следните ресурси:</span><span class="sxs-lookup"><span data-stu-id="e1712-108">For more information about meeting policies, see the following resources:</span></span>

- <span data-ttu-id="e1712-109">За да научите за създаването на правила, извършването на промени и присвояването на потребители на правилата, вижте Управление на правилата за [събрание в Teams](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams).</span><span class="sxs-lookup"><span data-stu-id="e1712-109">To learn about creating policies, making changes, and assigning users to the policy, see [Manage meeting policies in Teams](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams).</span></span>

- <span data-ttu-id="e1712-110">За да промените правилата с кратки команди на PowerShell, вижте [Преглед на PowerShell на екипи](https://docs.microsoft.com/microsoftteams/teams-powershell-overview).</span><span class="sxs-lookup"><span data-stu-id="e1712-110">To make policy changes using PowerShell cmdlets, see [Teams PowerShell Overview](https://docs.microsoft.com/microsoftteams/teams-powershell-overview).</span></span> 
    - <span data-ttu-id="e1712-111">Трябва да използвате [Skype за бизнес PowerShell модул](https://www.microsoft.com/download/details.aspx?id=39366) за правила за срещи на екипи.</span><span class="sxs-lookup"><span data-stu-id="e1712-111">You need to use the [Skype for Business PowerShell module](https://www.microsoft.com/download/details.aspx?id=39366) for Teams meeting policies.</span></span> 
    - <span data-ttu-id="e1712-112">Прегледайте документацията за [кратки команди \*-CsTeamsMeetingPolicy](https://docs.microsoft.com/search/?search=CsTeamsMeetingPolicy&view=skype-ps) за повече информация.</span><span class="sxs-lookup"><span data-stu-id="e1712-112">Review the [\*-CsTeamsMeetingPolicy cmdlets documentation](https://docs.microsoft.com/search/?search=CsTeamsMeetingPolicy&view=skype-ps) for more information.</span></span>

