---
title: Коригиране на транспортни правила
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
ms.openlocfilehash: 635009ed4b78d2b05b0eef1f3298765b10f86ede
ms.sourcegitcommit: bd6a9cb5d357baee5134c0dea430afc2a035c810
ms.translationtype: MT
ms.contentlocale: bg-BG
ms.lasthandoff: 03/09/2021
ms.locfileid: "50692825"
---
# <a name="fix-transport-rules"></a><span data-ttu-id="0994b-102">Коригиране на транспортни правила</span><span class="sxs-lookup"><span data-stu-id="0994b-102">Fix transport rules</span></span>

<span data-ttu-id="0994b-103">Правилото за пощенския поток по избор е засегнало това съобщение.</span><span class="sxs-lookup"><span data-stu-id="0994b-103">A custom mail flow rule affected this message.</span></span> <span data-ttu-id="0994b-104">За да прегледате точното правило, направете следното:</span><span class="sxs-lookup"><span data-stu-id="0994b-104">To review the exact rule, do the following:</span></span>

1. <span data-ttu-id="0994b-105">В резултатите от представянето под **допълнителна информация** отбележете **GUID** или **името на правилата**.</span><span class="sxs-lookup"><span data-stu-id="0994b-105">In the submission results, under **Additional information**, note the **GUID** or the **Policy Name**.</span></span>
2. <span data-ttu-id="0994b-106">Стартиране на обвивката за управление на Exchange.</span><span class="sxs-lookup"><span data-stu-id="0994b-106">Launch Exchange Management Shell.</span></span> <span data-ttu-id="0994b-107">За повече информация вижте [Отваряне на обвивката за управление на Exchange](https://go.microsoft.com/fwlink/?linkid=2101432).</span><span class="sxs-lookup"><span data-stu-id="0994b-107">For more information, see [Open the Exchange Management Shell](https://go.microsoft.com/fwlink/?linkid=2101432).</span></span>
3. <span data-ttu-id="0994b-108">Изпълнете тази команда (като използвате GUID от подаването си):  **get-TransportRule-самоличност "GUID" | FL \* описание**\*</span><span class="sxs-lookup"><span data-stu-id="0994b-108">Run this command (using the GUID from your submission):  **Get-TransportRule -identity "GUID" | fl \* Description**\*</span></span>
4. <span data-ttu-id="0994b-109">Прегледайте описанието, за да видите конфигурираните условия, които са засегнали съобщението.</span><span class="sxs-lookup"><span data-stu-id="0994b-109">Review the description to see the configured conditions that affected the message.</span></span>

<span data-ttu-id="0994b-110">За да научите повече, вижте [get-TransportRule](https://go.microsoft.com/fwlink/?linkid=2101523).</span><span class="sxs-lookup"><span data-stu-id="0994b-110">To learn more, see [Get-TransportRule](https://go.microsoft.com/fwlink/?linkid=2101523).</span></span>
