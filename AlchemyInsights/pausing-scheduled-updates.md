---
title: Пауза на планираните актуализации
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/30/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "1129"
- "6700007"
ms.openlocfilehash: 9dc0f387cf63557e2a1f81ca8f3c3ca9998170ca
ms.sourcegitcommit: d1c51266e2890f61662f77dceea2ad0c88210015
ms.translationtype: MT
ms.contentlocale: bg-BG
ms.lasthandoff: 07/30/2020
ms.locfileid: "46554810"
---
# <a name="pausing-scheduled-updates"></a><span data-ttu-id="16ac4-102">Пауза на планираните актуализации</span><span class="sxs-lookup"><span data-stu-id="16ac4-102">Pausing scheduled updates</span></span>

<span data-ttu-id="16ac4-103">Когато се издава команда за пауза, устройствата не обработват командата до следващото им чекиране в Intune.</span><span class="sxs-lookup"><span data-stu-id="16ac4-103">When a pause command is issued, devices don't process the command until the next time they check in to Intune.</span></span> <span data-ttu-id="16ac4-104">Поради това вашите устройства може да имат:</span><span class="sxs-lookup"><span data-stu-id="16ac4-104">Because of this, your devices might have:</span></span>

- <span data-ttu-id="16ac4-105">Инсталирали са планираните актуализации преди регистрацията.</span><span class="sxs-lookup"><span data-stu-id="16ac4-105">Installed the scheduled updates prior to check-in.</span></span>
- <span data-ttu-id="16ac4-106">Когато издадехте командата за пауза, е изключена.</span><span class="sxs-lookup"><span data-stu-id="16ac4-106">Been powered off when you issued the pause command.</span></span> <span data-ttu-id="16ac4-107">В този случай, когато устройствата са били включени, те може да са изтеглили и инсталирали планираните актуализации преди регистрацията.</span><span class="sxs-lookup"><span data-stu-id="16ac4-107">In this case, when the devices were powered on, they might have downloaded and installed the scheduled updates prior to check-in.</span></span>