---
title: Използване на Гифчета в разговорите в Teams
ms.author: v-jmathew
author: v-jmathew
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9003825"
- "6850"
ms.openlocfilehash: 2fc29974bff9484c226c9651b9b000a89cad14dc
ms.sourcegitcommit: 534e9217d99336eb471166ff83231c7e408fb1d9
ms.translationtype: MT
ms.contentlocale: bg-BG
ms.lasthandoff: 11/09/2020
ms.locfileid: "48982425"
---
# <a name="using-giphys-in-teams-conversations"></a><span data-ttu-id="ed75a-102">Използване на Гифчета в разговорите в Teams</span><span class="sxs-lookup"><span data-stu-id="ed75a-102">Using Giphys in Teams Conversations</span></span>

<span data-ttu-id="ed75a-103">Достъпът до гифчета в чата на Teams е разрешен по подразбиране.</span><span class="sxs-lookup"><span data-stu-id="ed75a-103">Giphys access in Teams chat is enabled by default.</span></span> <span data-ttu-id="ed75a-104">Като администратор можете да управлявате дали Гифчета са достъпни за потребителите чрез [Задаване на правила за съобщения](https://docs.microsoft.com/microsoftteams/messaging-policies-in-teams#messaging-policy-settings) и гарантиране, че **използването на гифчета в разговорите** е **включено**.</span><span class="sxs-lookup"><span data-stu-id="ed75a-104">As an administrator, you can control if Giphys are available to users by [setting a messaging policy](https://docs.microsoft.com/microsoftteams/messaging-policies-in-teams#messaging-policy-settings) and ensuring that **Use Giphys in conversations** is **On**.</span></span>

<span data-ttu-id="ed75a-105">Ако GIF файловете не работят по очаквания начин в разговорите в Teams, проверете следното:</span><span class="sxs-lookup"><span data-stu-id="ed75a-105">If GIFs are not working as expected in Teams conversations, verify:</span></span>

<span data-ttu-id="ed75a-106">[Правилата за съобщения](https://docs.microsoft.com/microsoftteams/messaging-policies-in-teams) трябва да позволяват на гифчета.</span><span class="sxs-lookup"><span data-stu-id="ed75a-106">The [messaging policy](https://docs.microsoft.com/microsoftteams/messaging-policies-in-teams) needs to allow Giphys.</span></span> <span data-ttu-id="ed75a-107">За да проверите с помощта на кратки команди на PowerShell:</span><span class="sxs-lookup"><span data-stu-id="ed75a-107">To verify by using PowerShell cmdlets:</span></span>

- <span data-ttu-id="ed75a-108">Проверете дали можете да [управлявате Teams с PowerShell](https://docs.microsoft.com/microsoftteams/teams-powershell-overview?view=o365-worldwide#manage-teams-with-powershell).</span><span class="sxs-lookup"><span data-stu-id="ed75a-108">Verify that you can [Manage Teams with PowerShell](https://docs.microsoft.com/microsoftteams/teams-powershell-overview?view=o365-worldwide#manage-teams-with-powershell).</span></span>
- <span data-ttu-id="ed75a-109">Изпълнете командата PowerShell [get-CsTeamsMessagingPolicy-Identity Global](https://docs.microsoft.com/powershell/module/skype/get-csteamsmessagingpolicy?view=skype-ps) и проверете дали **AllowGiphy** е зададено на **TRUE**.</span><span class="sxs-lookup"><span data-stu-id="ed75a-109">Run the PowerShell command [Get-CsTeamsMessagingPolicy -Identity Global](https://docs.microsoft.com/powershell/module/skype/get-csteamsmessagingpolicy?view=skype-ps) and verify that **AllowGiphy** is set to **TRUE**.</span></span>
- <span data-ttu-id="ed75a-110">Ако " **AllowGiphy** " е зададено на **FALSE** , изпълнете следния команден набор на PowerShell [– CsTeamsMessagingPolicy-AllowGiphy $True](https://docs.microsoft.com/powershell/module/skype/set-csteamsmessagingpolicy?view=skype-ps).</span><span class="sxs-lookup"><span data-stu-id="ed75a-110">If **AllowGiphy** is set to **FALSE** , run the following PowerShell command [Set-CsTeamsMessagingPolicy -Identity Global -AllowGiphy $True](https://docs.microsoft.com/powershell/module/skype/set-csteamsmessagingpolicy?view=skype-ps).</span></span>

<span data-ttu-id="ed75a-111">[Опционалните свързани преживявания](https://docs.microsoft.com/deployoffice/privacy/optional-connected-experiences) трябва да са разрешени за разрешаване на достъпа до URL адреса на Giphy.</span><span class="sxs-lookup"><span data-stu-id="ed75a-111">[Optional Connected Experiences](https://docs.microsoft.com/deployoffice/privacy/optional-connected-experiences) need to be enabled to allow access to the Giphy URL.</span></span>

> [!NOTE]
> <span data-ttu-id="ed75a-112">Ако имате няколко правила за съобщения, конфигурирани за вашия клиент, можете да определите самоличността на правилата, присвоени на засегнатия потребител, с помощта на командата PowerShell [get-CsOnlineUser-самоличност](https://docs.microsoft.com/powershell/module/skype/get-csonlineuser?view=skype-ps) <user@domain.com> | Изберете TeamsMessagingPolicy.</span><span class="sxs-lookup"><span data-stu-id="ed75a-112">If you have multiple Teams Messaging policies configured for your tenant, you can determine the identity of the policy assigned to the impacted user with the PowerShell command [Get-CsOnlineUser -Identity](https://docs.microsoft.com/powershell/module/skype/get-csonlineuser?view=skype-ps) <user@domain.com> | Select TeamsMessagingPolicy.</span></span>
