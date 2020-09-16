---
title: Пауза на планирани актуализации
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/30/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "1129"
- "6700007"
ms.openlocfilehash: 13abc7c9201b1897a9c766add4d105ef12f0d66f
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: bg-BG
ms.lasthandoff: 09/14/2020
ms.locfileid: "47721544"
---
# <a name="pausing-scheduled-updates"></a><span data-ttu-id="f09a0-102">Пауза на планирани актуализации</span><span class="sxs-lookup"><span data-stu-id="f09a0-102">Pausing scheduled updates</span></span>

<span data-ttu-id="f09a0-103">Когато е издадена команда за пауза, устройствата не обработват командата до следващия път, когато вкарват в списъка.</span><span class="sxs-lookup"><span data-stu-id="f09a0-103">When a pause command is issued, devices don't process the command until the next time they check in to Intune.</span></span> <span data-ttu-id="f09a0-104">Поради това вашите устройства може да имат:</span><span class="sxs-lookup"><span data-stu-id="f09a0-104">Because of this, your devices might have:</span></span>

- <span data-ttu-id="f09a0-105">Инсталирали планирани актуализации преди вкарването.</span><span class="sxs-lookup"><span data-stu-id="f09a0-105">Installed the scheduled updates prior to check-in.</span></span>
- <span data-ttu-id="f09a0-106">Изключено, когато сте издали командата пауза.</span><span class="sxs-lookup"><span data-stu-id="f09a0-106">Been powered off when you issued the pause command.</span></span> <span data-ttu-id="f09a0-107">В този случай, когато устройствата са включени, може да са изтеглили и инсталирали планираните актуализации преди вкарването.</span><span class="sxs-lookup"><span data-stu-id="f09a0-107">In this case, when the devices were powered on, they might have downloaded and installed the scheduled updates prior to check-in.</span></span>