---
title: Offboard устройства, които не са с Windows, от Microsoft Defender Advanced Protection (ATP)
ms.author: v-jmathew
author: v-jmathew
manager: dansimp
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000760"
- "7391"
ms.openlocfilehash: 435957c555cd80155a985a49bd94b041a4ada31d
ms.sourcegitcommit: 6312ee31561db36104f32282d019d069ede69174
ms.translationtype: MT
ms.contentlocale: bg-BG
ms.lasthandoff: 03/11/2021
ms.locfileid: "50743292"
---
# <a name="offboard-non-windows-devices-from-microsoft-defender-advanced-threat-protection-atp"></a><span data-ttu-id="c3c7a-102">Offboard устройства, които не са с Windows, от Microsoft Defender Advanced Protection (ATP)</span><span class="sxs-lookup"><span data-stu-id="c3c7a-102">Offboard non-Windows devices from Microsoft Defender Advanced Threat Protection (ATP)</span></span>

<span data-ttu-id="c3c7a-103">Ето как:</span><span class="sxs-lookup"><span data-stu-id="c3c7a-103">Here's how:</span></span>

1. <span data-ttu-id="c3c7a-104">Следвайте документацията на други разработчици за прекъсване на връзката с решението на друг доставчик от Microsoft Defender ATP.</span><span class="sxs-lookup"><span data-stu-id="c3c7a-104">Follow the third-party documentation for disconnecting the third-party solution from Microsoft Defender ATP.</span></span>
2. <span data-ttu-id="c3c7a-105">От вашия клиент на Azure Active Directory премахнете разрешения за решението на друг доставчик:</span><span class="sxs-lookup"><span data-stu-id="c3c7a-105">From your Azure Active Directory tenant, remove permissions for the third-party solution:</span></span>

    1. <span data-ttu-id="c3c7a-106">Влезте в портала на [Azure](https://go.microsoft.com/fwlink/?linkid=2125612).</span><span class="sxs-lookup"><span data-stu-id="c3c7a-106">Sign in to the [Azure portal](https://go.microsoft.com/fwlink/?linkid=2125612).</span></span>
    1. <span data-ttu-id="c3c7a-107">Изберете **всички Services**  >  **Azure Active Directory**  >  **Enterprise приложения**.</span><span class="sxs-lookup"><span data-stu-id="c3c7a-107">Select **All services** > **Azure Active Directory** > **Enterprise Applications**.</span></span>
    1. <span data-ttu-id="c3c7a-108">Изберете приложението, което искате да offboard.</span><span class="sxs-lookup"><span data-stu-id="c3c7a-108">Select the application you'd like to offboard.</span></span>
    1. <span data-ttu-id="c3c7a-109">Изберете **Изтрий**.</span><span class="sxs-lookup"><span data-stu-id="c3c7a-109">Select **Delete**.</span></span>

<span data-ttu-id="c3c7a-110">За да научите повече, вижте [offboard устройства, които не са с Windows](https://go.microsoft.com/fwlink/?linkid=2143630).</span><span class="sxs-lookup"><span data-stu-id="c3c7a-110">To learn more, see [Offboard non-Windows devices](https://go.microsoft.com/fwlink/?linkid=2143630).</span></span>
