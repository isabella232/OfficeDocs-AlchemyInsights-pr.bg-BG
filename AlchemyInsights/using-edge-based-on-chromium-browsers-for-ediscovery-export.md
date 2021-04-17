---
title: Използване на Microsoft Edge на базата на браузъри chromium за експортиране на Ediscovery
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
- "3473"
- "3100022"
ms.openlocfilehash: 7ee724e5109effce8883be50e360948313c84b34
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: bg-BG
ms.lasthandoff: 04/15/2021
ms.locfileid: "51834360"
---
# <a name="using-microsoft-edge-based-on-chromium-browsers-for-ediscovery-export"></a><span data-ttu-id="e4c82-102">Използване на Microsoft Edge на базата на браузъри chromium за експортиране на Ediscovery</span><span class="sxs-lookup"><span data-stu-id="e4c82-102">Using Microsoft Edge based on Chromium browsers for Ediscovery export</span></span>

<span data-ttu-id="e4c82-103">Поради скорошна промяна браузърите на Microsoft Edge вече няма да имат поддръжка на ClickOnce разрешена по подразбиране.</span><span class="sxs-lookup"><span data-stu-id="e4c82-103">Due to a recent change, Microsoft Edge browsers will no longer have ClickOnce support enabled by default.</span></span> <span data-ttu-id="e4c82-104">За да продължите да използвате инструмента за експортиране на електронни данни на Microsoft 365, ще трябва да използвате Microsoft Internet Explorer или да разрешите поддръжката на ClickOnce в Microsoft Edge.</span><span class="sxs-lookup"><span data-stu-id="e4c82-104">To continue using the Microsoft 365 eDiscovery Export Tool, you will either need to use Microsoft Internet Explorer or enable ClickOnce Support in Microsoft Edge.</span></span> 

<span data-ttu-id="e4c82-105">За да разрешите поддръжката на ClickOnce в Microsoft Edge на базата на Хром:</span><span class="sxs-lookup"><span data-stu-id="e4c82-105">To enable ClickOnce Support in Microsoft Edge based on Chromium:</span></span> 
1. <span data-ttu-id="e4c82-106">В браузъра Microsoft Edge посетете edge://flags/#edge-click-once.</span><span class="sxs-lookup"><span data-stu-id="e4c82-106">In your Microsoft Edge browser, visit edge://flags/#edge-click-once.</span></span>
2. <span data-ttu-id="e4c82-107">За опцията Поддръжка на ClickOnce променете стойността от По подразбиране **или** **Забранено** на **Разрешено.**</span><span class="sxs-lookup"><span data-stu-id="e4c82-107">For the ClickOnce Support option, change the value from **Default** or **Disabled** to **Enabled**.</span></span> 
3. <span data-ttu-id="e4c82-108">В долната част на прозореца на браузъра изберете **Рестартиране**.</span><span class="sxs-lookup"><span data-stu-id="e4c82-108">At the bottom of the browser window, select **Restart**.</span></span> <br>
 <span data-ttu-id="e4c82-109">Промяната ще в сила след рестартирането на Microsoft Edge.</span><span class="sxs-lookup"><span data-stu-id="e4c82-109">The change will take effect after restarting Microsoft Edge.</span></span> 

<span data-ttu-id="e4c82-110">За информация относно това и стъпките за инсталиране на инструмента за експортиране вижте: Експортиране на [ резултатите от търсенето на съдържание](https://docs.microsoft.com/microsoft-365/compliance/export-search-results).</span><span class="sxs-lookup"><span data-stu-id="e4c82-110">For information on this and steps for installing the  export tool, see: [ Export Content Search results](https://docs.microsoft.com/microsoft-365/compliance/export-search-results).</span></span>