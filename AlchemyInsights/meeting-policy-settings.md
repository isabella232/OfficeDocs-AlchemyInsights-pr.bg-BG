---
title: Настройки на правилата за събранието
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
- "9000734"
- "2657"
ms.openlocfilehash: 24a55417df0f89063fbdd9ade6d104be4f8ab49c
ms.sourcegitcommit: 0eb4f9bde53395b5fd4b5cd4ffc56ca96db91298
ms.translationtype: MT
ms.contentlocale: bg-BG
ms.lasthandoff: 03/10/2021
ms.locfileid: "50704595"
---
# <a name="manage-meeting-policies-in-microsoft-teams"></a><span data-ttu-id="ec84c-102">Управление на правила за събрания в Microsoft Teams</span><span class="sxs-lookup"><span data-stu-id="ec84c-102">Manage meeting policies in Microsoft Teams</span></span>

<span data-ttu-id="ec84c-103">**Забележка: възможно е да са необходими до 24 часа, за да влязат в сила промените в правилата за потребителите.**</span><span class="sxs-lookup"><span data-stu-id="ec84c-103">**Note: It can take up to 24 hours for policy changes to take effect for users.**</span></span> <span data-ttu-id="ec84c-104">Възможно е да не можете да правите промени в току-що създадените правила незабавно; Изчакайте 4 часа и се опитайте отново да промените ново създадената политика.</span><span class="sxs-lookup"><span data-stu-id="ec84c-104">You might not be able to make changes to newly created policies immediately; wait 4 hours and attempt to modify a newly created policy again.</span></span>

<span data-ttu-id="ec84c-105">Правилата за събрания се използват за управление на функциите, които са достъпни за участниците в събранието, за събрания, които са планирани от потребители във вашата организация.</span><span class="sxs-lookup"><span data-stu-id="ec84c-105">Meeting policies are used to control the features that are available to meeting participants for meetings that are scheduled by users in your organization.</span></span> <span data-ttu-id="ec84c-106">Някои функции на правилата за събрания може да не бъдат реализирани в центъра за администриране на екипи все още (те са означени с "Очаквайте скоро" в документацията).</span><span class="sxs-lookup"><span data-stu-id="ec84c-106">Some features of meeting policies might not be implemented in the Teams admin center yet (these are labeled "coming soon" in the documentation).</span></span> <span data-ttu-id="ec84c-107">В този случай или ако получавате съобщение за грешка като "не можем да актуализираме правилата в момента, но опитайте отново по-късно" в центъра за администриране на Microsoft Teams, ви препоръчваме да използвате PowerShell, за да създавате или модифицирате правила за събрания в Teams.</span><span class="sxs-lookup"><span data-stu-id="ec84c-107">In this case, or if you are getting an error like "We can't update the policy right now but try it again later" in the Microsoft Teams admin center, we recommend that you use PowerShell to create or modify Teams meeting policies.</span></span> 

<span data-ttu-id="ec84c-108">За повече информация относно правилата за събрания вижте следните ресурси:</span><span class="sxs-lookup"><span data-stu-id="ec84c-108">For more information about meeting policies, see the following resources:</span></span>

- <span data-ttu-id="ec84c-109">За да научите повече за създаването на правила, извършването на промени и присвояването на потребители на правилата, вижте [управление на правилата за събрания в Teams](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams).</span><span class="sxs-lookup"><span data-stu-id="ec84c-109">To learn about creating policies, making changes, and assigning users to the policy, see [Manage meeting policies in Teams](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams).</span></span>

- <span data-ttu-id="ec84c-110">За да направите промени в правилата с помощта на кратки команди на PowerShell, вижте [общ преглед на PowerShell за Teams](https://docs.microsoft.com/microsoftteams/teams-powershell-overview).</span><span class="sxs-lookup"><span data-stu-id="ec84c-110">To make policy changes using PowerShell cmdlets, see [Teams PowerShell Overview](https://docs.microsoft.com/microsoftteams/teams-powershell-overview).</span></span> 
    - <span data-ttu-id="ec84c-111">Трябва да използвате модула на [Skype за бизнеса PowerShell](https://docs.microsoft.com/skypeforbusiness/set-up-your-computer-for-windows-powershell/download-and-install-the-skype-for-business-online-connector) за правилата за събрания в Teams.</span><span class="sxs-lookup"><span data-stu-id="ec84c-111">You need to use the [Skype for Business PowerShell module](https://docs.microsoft.com/skypeforbusiness/set-up-your-computer-for-windows-powershell/download-and-install-the-skype-for-business-online-connector) for Teams meeting policies.</span></span> 
    - <span data-ttu-id="ec84c-112">Прегледайте [документацията \* – CsTeamsMeetingPolicy кратки команди](https://docs.microsoft.com/search/?search=CsTeamsMeetingPolicy&view=skype-ps) за повече информация.</span><span class="sxs-lookup"><span data-stu-id="ec84c-112">Review the [\*-CsTeamsMeetingPolicy cmdlets documentation](https://docs.microsoft.com/search/?search=CsTeamsMeetingPolicy&view=skype-ps) for more information.</span></span>

