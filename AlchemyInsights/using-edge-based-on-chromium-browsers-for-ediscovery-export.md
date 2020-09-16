---
title: Използване на Microsoft Edge на базата на браузъри за хром за експортиране на откриването на електронни данни
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
- "3473"
- "3100022"
ms.openlocfilehash: 64aebb7f048dba37eef8cd1fa6286b36823d3f0f
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: bg-BG
ms.lasthandoff: 09/14/2020
ms.locfileid: "47734504"
---
# <a name="using-microsoft-edge-based-on-chromium-browsers-for-ediscovery-export"></a><span data-ttu-id="5afb6-102">Използване на Microsoft Edge на базата на браузъри за хром за експортиране на откриването на електронни данни</span><span class="sxs-lookup"><span data-stu-id="5afb6-102">Using Microsoft Edge based on Chromium browsers for Ediscovery export</span></span>

<span data-ttu-id="5afb6-103">Поради скорошна промяна браузърите за Microsoft Edge вече няма да имат разрешени поддръжка на инсталирана добавка ClickOnce по подразбиране.</span><span class="sxs-lookup"><span data-stu-id="5afb6-103">Due to a recent change, Microsoft Edge browsers will no longer have ClickOnce support enabled by default.</span></span> <span data-ttu-id="5afb6-104">За да продължите да използвате инструмента за експортиране на откриването на електронни данни на Microsoft 365, ще трябва или да използвате Microsoft Internet Explorer, или да разрешите поддръжката на инсталирана добавка ClickOnce в Microsoft Edge.</span><span class="sxs-lookup"><span data-stu-id="5afb6-104">To continue using the Microsoft 365 eDiscovery Export Tool, you will either need to use Microsoft Internet Explorer or enable ClickOnce Support in Microsoft Edge.</span></span> 

<span data-ttu-id="5afb6-105">За да разрешите поддръжката на инсталирана добавка ClickOnce в Microsoft Edge на базата на хром:</span><span class="sxs-lookup"><span data-stu-id="5afb6-105">To enable ClickOnce Support in Microsoft Edge based on Chromium:</span></span> 
1. <span data-ttu-id="5afb6-106">В браузъра Microsoft Edge посетете edge://flags/#edge – еднократно щракване.</span><span class="sxs-lookup"><span data-stu-id="5afb6-106">In your Microsoft Edge browser, visit edge://flags/#edge-click-once.</span></span>
2. <span data-ttu-id="5afb6-107">За опцията за поддръжка на инсталирана добавка ClickOnce променете стойността **по подразбиране** или **забранената** за **разрешена**.</span><span class="sxs-lookup"><span data-stu-id="5afb6-107">For the ClickOnce Support option, change the value from **Default** or **Disabled** to **Enabled**.</span></span> 
3. <span data-ttu-id="5afb6-108">В долната част на прозореца на браузъра изберете **Рестартирай**.</span><span class="sxs-lookup"><span data-stu-id="5afb6-108">At the bottom of the browser window, select **Restart**.</span></span> <br>
 <span data-ttu-id="5afb6-109">Промяната ще влезе в сила след рестартиране на Microsoft Edge.</span><span class="sxs-lookup"><span data-stu-id="5afb6-109">The change will take effect after restarting Microsoft Edge.</span></span> 

<span data-ttu-id="5afb6-110">За информация относно това и стъпките за инсталиране на инструмента за експортиране вижте: [ експортиране на резултати от търсене на съдържание](https://docs.microsoft.com/microsoft-365/compliance/export-search-results).</span><span class="sxs-lookup"><span data-stu-id="5afb6-110">For information on this and steps for installing the  export tool, see: [ Export Content Search results](https://docs.microsoft.com/microsoft-365/compliance/export-search-results).</span></span>