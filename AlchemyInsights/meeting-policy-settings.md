---
title: Изпълнение на настройките на правилата
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "2657"
- "9000734"
ms.openlocfilehash: dac06690b51459ca166c15a5ef0f4c7e7a6d36f0
ms.sourcegitcommit: 0495112ad4fd0e695140ec66d190e62f03030584
ms.translationtype: MT
ms.contentlocale: bg-BG
ms.lasthandoff: 10/02/2019
ms.locfileid: "37376520"
---
# <a name="manage-meeting-policies-in-microsoft-teams"></a><span data-ttu-id="c1b1f-102">Управление на правилата за събрания в екипите на Microsoft</span><span class="sxs-lookup"><span data-stu-id="c1b1f-102">Manage meeting policies in Microsoft Teams</span></span>

<span data-ttu-id="c1b1f-103">Правилата за събрания се използват за управление на функциите, които са достъпни за събрания на участниците за събрания, които са планирани от потребителите във вашата организация.</span><span class="sxs-lookup"><span data-stu-id="c1b1f-103">Meeting policies are used to control the features that are available to meeting participants for meetings that are scheduled by users in your organization.</span></span> <span data-ttu-id="c1b1f-104">Някои функции на събрание правила може да не се изпълняват в центъра за администриране на екипите все още (те са маркирани "Очаквайте скоро" в документацията).</span><span class="sxs-lookup"><span data-stu-id="c1b1f-104">Some features of meeting policies might not be implemented in the Teams admin center yet (these are labeled "coming soon" in the documentation).</span></span> <span data-ttu-id="c1b1f-105">В този случай или ако получавате грешка като "не можем да актуализираме правилата в момента, но опитайте отново по-късно" в центъра за администриране на екипи на Microsoft, препоръчваме да използвате PowerShell за създаване или модифициране на правила за събрания на екипи.</span><span class="sxs-lookup"><span data-stu-id="c1b1f-105">In this case, or if you are getting an error like "We can't update the policy right now but try it again later" in the Microsoft Teams admin center, we recommend that you use PowerShell to create or modify Teams meeting policies.</span></span> 

<span data-ttu-id="c1b1f-106">За повече информация относно правилата за събрания вижте следните ресурси:</span><span class="sxs-lookup"><span data-stu-id="c1b1f-106">For more information about meeting policies, see the following resources:</span></span>

- <span data-ttu-id="c1b1f-107">За да научите как да създавате правила, да правите промени и да присвоявате потребители на правилата, вижте [управление на правила за събрания в екипи](https://docs.microsoft.com/en-us/microsoftteams/meeting-policies-in-teams).</span><span class="sxs-lookup"><span data-stu-id="c1b1f-107">To learn about creating policies, making changes, and assigning users to the policy, see [Manage meeting policies in Teams](https://docs.microsoft.com/en-us/microsoftteams/meeting-policies-in-teams).</span></span>

- <span data-ttu-id="c1b1f-108">За да промените правилата с помощта на кратки команди PowerShell, вижте [екипи PowerShell преглед](https://docs.microsoft.com/microsoftteams/teams-powershell-overview).</span><span class="sxs-lookup"><span data-stu-id="c1b1f-108">To make policy changes using PowerShell cmdlets, see [Teams PowerShell Overview](https://docs.microsoft.com/microsoftteams/teams-powershell-overview).</span></span> 
    - <span data-ttu-id="c1b1f-109">Трябва да използвате [Skype за бизнес PowerShell модул](https://www.microsoft.com/download/details.aspx?id=39366) за екипи събрание правила.</span><span class="sxs-lookup"><span data-stu-id="c1b1f-109">You need to use the [Skype for Business PowerShell module](https://www.microsoft.com/download/details.aspx?id=39366) for Teams meeting policies.</span></span> 
    - <span data-ttu-id="c1b1f-110">Прегледайте [документацията на \*-парапарцияправила кратки команди](https://docs.microsoft.com/search/?search=CsTeamsMeetingPolicy&view=skype-ps) за повече информация.</span><span class="sxs-lookup"><span data-stu-id="c1b1f-110">Review the [\*-CsTeamsMeetingPolicy cmdlets documentation](https://docs.microsoft.com/search/?search=CsTeamsMeetingPolicy&view=skype-ps) for more information.</span></span>

<span data-ttu-id="c1b1f-111">**Забележка:** Може да отнеме до 24 часа, когато промените в правилата влязат в сила за потребителите.</span><span class="sxs-lookup"><span data-stu-id="c1b1f-111">**Note:** It can take up to 24 hours for policy changes to take effect for users.</span></span> <span data-ttu-id="c1b1f-112">Възможно е да не успеете да направите незабавно промени в новосъздадените правила; Изчакайте 4 часа и опитайте отново да промените новосъздадената политика.</span><span class="sxs-lookup"><span data-stu-id="c1b1f-112">You might not be able to make changes to newly created policies immediately; wait 4 hours and attempt to modify a newly created policy again.</span></span> <span data-ttu-id="c1b1f-113">Ако все още имате проблеми, опитайте PowerShell.</span><span class="sxs-lookup"><span data-stu-id="c1b1f-113">If you're still having problems, try PowerShell.</span></span>  