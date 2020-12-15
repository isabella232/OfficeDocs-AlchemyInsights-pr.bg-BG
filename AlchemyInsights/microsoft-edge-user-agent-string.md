---
title: Низ за потребителски агент на Microsoft Edge (настолна версия)
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 12/03/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9003862"
- "6914"
ms.openlocfilehash: b4106dde1e09e0ce07b4b9adc2b2984cc5609c3b
ms.sourcegitcommit: 3c6e777d6679a24108171e9aa3f9379a8d44e001
ms.translationtype: MT
ms.contentlocale: bg-BG
ms.lasthandoff: 12/09/2020
ms.locfileid: "49676876"
---
# <a name="microsoft-edge-user-agent-string-desktop"></a><span data-ttu-id="24318-102">Низ за потребителски агент на Microsoft Edge (настолна версия)</span><span class="sxs-lookup"><span data-stu-id="24318-102">Microsoft Edge user agent string (Desktop)</span></span>

<span data-ttu-id="24318-103">За откриване на версията на конкретен браузър за определена операционна система се използва потребителски агент (UA).</span><span class="sxs-lookup"><span data-stu-id="24318-103">User agent (UA) strings can be used to detect what version of a specific browser is being used on a certain operating system.</span></span> <span data-ttu-id="24318-104">Подобно на други браузъри, Microsoft Edge включва тази информация в HTTP заглавката "User-Agent" всеки път, когато направи заявка към сайта.</span><span class="sxs-lookup"><span data-stu-id="24318-104">Like other browsers, Microsoft Edge includes this information in the "User-Agent" HTTP header whenever it makes a request to a site.</span></span> <span data-ttu-id="24318-105">Информацията за версията на браузъра може да бъде достъпна и чрез JavaScript чрез заявка за стойността на "Navigator. userAgent".</span><span class="sxs-lookup"><span data-stu-id="24318-105">The browser-version information can also be accessed via JavaScript by querying the value of "navigator.userAgent".</span></span>

<span data-ttu-id="24318-106">Препоръчваме уеб разработчиците да се възползват от откриването на функции, когато е възможно, за да подобрят възможностите за поддържане на кода, да намалят уязвимостта на кода и да елиминират риска от прекъсване на кода в случай на бъдещи актуализации на низ.</span><span class="sxs-lookup"><span data-stu-id="24318-106">We recommend that web developers make use of feature detection whenever possible to improve code maintainability, reduce code fragility, and eliminate the risk of code breakage in the event of future UA string updates.</span></span>

<span data-ttu-id="24318-107">За повече информация вижте [низ за потребителски агент на Microsoft Edge (настолна версия)](https://docs.microsoft.com/microsoft-edge/web-platform/user-agent-string).</span><span class="sxs-lookup"><span data-stu-id="24318-107">For more information, see [Microsoft Edge User Agent String (Desktop)](https://docs.microsoft.com/microsoft-edge/web-platform/user-agent-string).</span></span>