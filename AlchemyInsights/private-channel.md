---
title: Личен канал
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9001223"
- "3205"
ms.openlocfilehash: be518df0d40123c1f0da6596bd6e2e91a0c2c8fa
ms.sourcegitcommit: 057d87c9d866fa1371d02350420d13774545c028
ms.translationtype: MT
ms.contentlocale: bg-BG
ms.lasthandoff: 05/02/2020
ms.locfileid: "44005427"
---
# <a name="private-channels-in-microsoft-teams"></a><span data-ttu-id="6227a-102">Лични канали в Microsoft Teams</span><span class="sxs-lookup"><span data-stu-id="6227a-102">Private channels in Microsoft Teams</span></span>

<span data-ttu-id="6227a-103">Частните канали са нова функция в Microsoft Teams.</span><span class="sxs-lookup"><span data-stu-id="6227a-103">Private channels is a new feature in Microsoft Teams.</span></span> <span data-ttu-id="6227a-104">Имайте предвид, че частните канали не могат да бъдат конвертирани от стандартни канали, нито обратно.</span><span class="sxs-lookup"><span data-stu-id="6227a-104">Note that private channels cannot be converted from standard channels or vice versa.</span></span>

<span data-ttu-id="6227a-105">За подробности относно поверителните канали, като например информация за [създаването на частни канали и за членството](https://docs.microsoft.com/MicrosoftTeams/private-channels#private-channel-creation-and-membership) и [частния канал на SharePoint](https://docs.microsoft.com/MicrosoftTeams/private-channels#private-channel-sharepoint-sites), вижте [лични канали в Microsoft Teams](https://docs.microsoft.com/MicrosoftTeams/private-channels).</span><span class="sxs-lookup"><span data-stu-id="6227a-105">For details about private channels, such as information on [private channel creation and membership](https://docs.microsoft.com/MicrosoftTeams/private-channels#private-channel-creation-and-membership) and [private channel SharePoint sites](https://docs.microsoft.com/MicrosoftTeams/private-channels#private-channel-sharepoint-sites), see [Private channels in Microsoft Teams](https://docs.microsoft.com/MicrosoftTeams/private-channels).</span></span> 

<span data-ttu-id="6227a-106">**Забележка:** Тъй като конфигурацията за запазване на съобщения в частния канал все още не се поддържа, за клиенти с разрешени правила за съхранение няма да има разрешени частни канали по подразбиране.</span><span class="sxs-lookup"><span data-stu-id="6227a-106">**Note:** Because configuration for retention of private channel messages is not yet supported, tenants with retention policies enabled will not have private channels enabled by default.</span></span> <span data-ttu-id="6227a-107">Частните канали могат да бъдат разрешени в центъра за администриране на Teams.</span><span class="sxs-lookup"><span data-stu-id="6227a-107">Private channels can be enabled in the Teams admin center.</span></span> <span data-ttu-id="6227a-108">Също така имайте предвид, че докато запазването на съобщенията в частния канал не се поддържа, се поддържа съхранение на файлове, споделени в частни канали.</span><span class="sxs-lookup"><span data-stu-id="6227a-108">Also, note that while retention of private channel messages is not supported, retention of files shared in private channels is supported.</span></span>

<span data-ttu-id="6227a-109">**Нуждаете се от нов собственик на екип?**</span><span class="sxs-lookup"><span data-stu-id="6227a-109">**Need a new team owner?**</span></span>

<span data-ttu-id="6227a-110">Ако вашият личен собственик на канал ви оставя, можете да добавите нов собственик на екип чрез Teams PowerShell.</span><span class="sxs-lookup"><span data-stu-id="6227a-110">If your private channel owner leaves, you can add a new team owner via Teams Powershell.</span></span>


- <span data-ttu-id="6227a-111">Отидете [тук](https://www.powershellgallery.com/packages/MicrosoftTeams/1.0.6) , за да инсталирате Teams PowerShell.</span><span class="sxs-lookup"><span data-stu-id="6227a-111">Go [here](https://www.powershellgallery.com/packages/MicrosoftTeams/1.0.6) to install Teams Powershell.</span></span>

<span data-ttu-id="6227a-112">Ето кратката команда, която ще ви трябва:</span><span class="sxs-lookup"><span data-stu-id="6227a-112">Here is the cmdlet you will need:</span></span>

`
    Add-TeamChannelUser -GroupId <group_id> -DisplayName "<channel_name>" -User <UPN> -Role Owner
`

<span data-ttu-id="6227a-113">За повече информация относно Teams PowerShell вижте [общ преглед на Teams PowerShell](https://docs.microsoft.com/microsoftteams/teams-powershell-overview).</span><span class="sxs-lookup"><span data-stu-id="6227a-113">For more information on Teams Powershell, see [Teams PowerShell Overview](https://docs.microsoft.com/microsoftteams/teams-powershell-overview).</span></span>
