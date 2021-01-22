---
title: Включване на технология НДИ
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
- "9004403"
- "7947"
ms.openlocfilehash: ea694898baffa50fca71957175eba3664dece44e
ms.sourcegitcommit: 112f18dce8257b98fab32d44910ee879efb44cb8
ms.translationtype: MT
ms.contentlocale: bg-BG
ms.lasthandoff: 01/21/2021
ms.locfileid: "49935074"
---
# <a name="turn-on-ndi-technology"></a><span data-ttu-id="0cdf1-102">Включване на технология НДИ</span><span class="sxs-lookup"><span data-stu-id="0cdf1-102">Turn on NDI technology</span></span>

<span data-ttu-id="0cdf1-103">НДИ технология изисква две стъпки, които трябва да бъдат включвани за потребител:</span><span class="sxs-lookup"><span data-stu-id="0cdf1-103">NDI technology requires two steps to be turned on for a user:</span></span>

1. <span data-ttu-id="0cdf1-104">Администраторът на клиент трябва да разреши свойството "AllowNDIStreaming" в CsTeamsMeetingPolicy.</span><span class="sxs-lookup"><span data-stu-id="0cdf1-104">The tenant admin must enable the 'AllowNDIStreaming' property in CsTeamsMeetingPolicy.</span></span>

    `Set-CsTeamsMeetingPolicy -Identity MEETING_POLICY -AllowNDIStreaming $true`

2. <span data-ttu-id="0cdf1-105">След като тази промяна бъде запълнена, крайният потребител трябва да включи НДИ® технология за своя конкретен клиент от **настройките > разрешения**.</span><span class="sxs-lookup"><span data-stu-id="0cdf1-105">After this change has populated, the end user must turn on NDI® technology for their specific client from **Settings > Permissions**.</span></span>

<span data-ttu-id="0cdf1-106">За повече информация вижте [използване на технология на НДИ в Microsoft Teams](https://docs.microsoft.com/microsoftteams/use-ndi-in-meetings).</span><span class="sxs-lookup"><span data-stu-id="0cdf1-106">For more information, see [Use NDI technology in Microsoft Teams](https://docs.microsoft.com/microsoftteams/use-ndi-in-meetings).</span></span>
