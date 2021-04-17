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
# <a name="manage-meeting-policies-in-microsoft-teams"></a><span data-ttu-id="816f6-102">Управление на правилата за събрания в Microsoft Teams</span><span class="sxs-lookup"><span data-stu-id="816f6-102">Manage meeting policies in Microsoft Teams</span></span>

<span data-ttu-id="816f6-103">**Забележка: Може да отнеме до 24 часа, за да влязат в сила промените в правилата за потребителите.**</span><span class="sxs-lookup"><span data-stu-id="816f6-103">**Note: It can take up to 24 hours for policy changes to take effect for users.**</span></span> <span data-ttu-id="816f6-104">Възможно е да не можете да правите промени в новосъздадените правила веднага; изчакайте 4 часа и опитайте да промените новосъздадените правила отново.</span><span class="sxs-lookup"><span data-stu-id="816f6-104">You might not be able to make changes to newly created policies immediately; wait 4 hours and attempt to modify a newly created policy again.</span></span>

<span data-ttu-id="816f6-105">Правилата за събрания се използват за управление на функциите, които са налични за участниците в събранието за събрания, които са планирани от потребителите във вашата организация.</span><span class="sxs-lookup"><span data-stu-id="816f6-105">Meeting policies are used to control the features that are available to meeting participants for meetings that are scheduled by users in your organization.</span></span> <span data-ttu-id="816f6-106">Някои функции на правилата за събрания може все още да не се внедлят в центъра за администриране на Teams (те са обозначени като "очаквайте скоро" в документацията).</span><span class="sxs-lookup"><span data-stu-id="816f6-106">Some features of meeting policies might not be implemented in the Teams admin center yet (these are labeled "coming soon" in the documentation).</span></span> <span data-ttu-id="816f6-107">В този случай или ако получавате грешка като "В момента не можем да актуализираме правилата, но да го изпробваме отново по-късно" в центъра за администриране на Microsoft Teams ви препоръчваме да използвате PowerShell, за да създавате или променяте правила за събрания на Teams.</span><span class="sxs-lookup"><span data-stu-id="816f6-107">In this case, or if you are getting an error like "We can't update the policy right now but try it again later" in the Microsoft Teams admin center, we recommend that you use PowerShell to create or modify Teams meeting policies.</span></span> 

<span data-ttu-id="816f6-108">За повече информация относно правилата за събрания вижте следните ресурси:</span><span class="sxs-lookup"><span data-stu-id="816f6-108">For more information about meeting policies, see the following resources:</span></span>

- <span data-ttu-id="816f6-109">За да научите за създаването на правила, извършването на промени и присвояването на потребители на правилата, вижте Управление [на правила за събрания в Teams](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams).</span><span class="sxs-lookup"><span data-stu-id="816f6-109">To learn about creating policies, making changes, and assigning users to the policy, see [Manage meeting policies in Teams](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams).</span></span>

- <span data-ttu-id="816f6-110">За да направите промени в правилата с помощта на кратки команди на PowerShell, вижте Общ [преглед на PowerShell на Teams](https://docs.microsoft.com/microsoftteams/teams-powershell-overview).</span><span class="sxs-lookup"><span data-stu-id="816f6-110">To make policy changes using PowerShell cmdlets, see [Teams PowerShell Overview](https://docs.microsoft.com/microsoftteams/teams-powershell-overview).</span></span> 
    - <span data-ttu-id="816f6-111">Трябва да използвате модула [на PowerShell на Skype за бизнеса за правилата](https://docs.microsoft.com/skypeforbusiness/set-up-your-computer-for-windows-powershell/download-and-install-the-skype-for-business-online-connector) за събрания на Teams.</span><span class="sxs-lookup"><span data-stu-id="816f6-111">You need to use the [Skype for Business PowerShell module](https://docs.microsoft.com/skypeforbusiness/set-up-your-computer-for-windows-powershell/download-and-install-the-skype-for-business-online-connector) for Teams meeting policies.</span></span> 
    - <span data-ttu-id="816f6-112">Прегледайте документацията на кратките команди [\*-CsTeamsMeetingPolicy](https://docs.microsoft.com/search/?search=CsTeamsMeetingPolicy&view=skype-ps) за повече информация.</span><span class="sxs-lookup"><span data-stu-id="816f6-112">Review the [\*-CsTeamsMeetingPolicy cmdlets documentation](https://docs.microsoft.com/search/?search=CsTeamsMeetingPolicy&view=skype-ps) for more information.</span></span>

