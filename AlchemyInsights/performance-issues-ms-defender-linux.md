---
title: Проблеми с производителността за Microsoft Defender за крайна точка на Linux
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 06/04/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "11491"
- "9001464"
ms.openlocfilehash: 268f44640d3b2d8764133560d0cbf500eb4afd22
ms.sourcegitcommit: 8242a824491f64be48dfe81da09766920fbd7feb
ms.translationtype: MT
ms.contentlocale: bg-BG
ms.lasthandoff: 06/06/2021
ms.locfileid: "52793576"
---
# <a name="performance-issues-for-microsoft-defender-for-endpoint-on-linux"></a><span data-ttu-id="5a063-102">Проблеми с производителността за Microsoft Defender за крайна точка на Linux</span><span class="sxs-lookup"><span data-stu-id="5a063-102">Performance issues for Microsoft Defender for Endpoint on Linux</span></span>

<span data-ttu-id="5a063-103">Тази статия ви насочва през стъпките за идентифициране на проблеми с производителността за Microsoft Defender за крайна точка на Linux.</span><span class="sxs-lookup"><span data-stu-id="5a063-103">This article guides you through the steps of identifying performance issues for Microsoft Defender for Endpoint on Linux.</span></span>

<span data-ttu-id="5a063-104">Важно е първо да проверите дали проблемът, който срещате, е решен с [най-новата версия](/microsoft-365/security/defender-endpoint/linux-whatsnew).</span><span class="sxs-lookup"><span data-stu-id="5a063-104">It's important to first verify that the problem you're experiencing is resolved with the [latest version](/microsoft-365/security/defender-endpoint/linux-whatsnew).</span></span> 

<span data-ttu-id="5a063-105">За да започнете разследването, вижте Отстраняване [на проблеми с производителността за Microsoft Defender за крайна точка на Linux.](/microsoft-365/security/defender-endpoint/linux-support-perf)</span><span class="sxs-lookup"><span data-stu-id="5a063-105">To start your investigation, see [Troubleshoot performance issues for Microsoft Defender for Endpoint on Linux](/microsoft-365/security/defender-endpoint/linux-support-perf).</span></span>

## <a name="exclusions"></a><span data-ttu-id="5a063-106">Изключения</span><span class="sxs-lookup"><span data-stu-id="5a063-106">Exclusions</span></span>

<span data-ttu-id="5a063-107">Изключенията могат да помогнат за намаляване на проблеми с производителността.</span><span class="sxs-lookup"><span data-stu-id="5a063-107">Exclusions can help to mitigate performance issues.</span></span> <span data-ttu-id="5a063-108">Прегледайте изключенията, преди да започнете, така че да се знае и документира допълнителен риск.</span><span class="sxs-lookup"><span data-stu-id="5a063-108">Review your exclusions before you begin so any additional risk is known and documented.</span></span>

<span data-ttu-id="5a063-109">За повече информация вижте Конфигуриране [и проверка на изключенията за Microsoft Defender за крайна точка на Linux.](/microsoft-365/security/defender-endpoint/linux-exclusions)</span><span class="sxs-lookup"><span data-stu-id="5a063-109">For more information, see [Configure and validate exclusions for Microsoft Defender for Endpoint on Linux](/microsoft-365/security/defender-endpoint/linux-exclusions).</span></span>

<span data-ttu-id="5a063-110">Когато имате няколко файла, & да изключите и всички те са на една и съща точка, може да е по-лесно да изключите точката на монтиране.</span><span class="sxs-lookup"><span data-stu-id="5a063-110">When you have multiple files & folders to exclude and they're all on the same mountpoint, it might be easier to exclude the mountpoint.</span></span> <span data-ttu-id="5a063-111">Започвайки от изданието от февруари 101.22.80, можете да изключите цяла точка.</span><span class="sxs-lookup"><span data-stu-id="5a063-111">Starting with February release 101.22.80, you can exclude an entire mountpoint.</span></span>

<span data-ttu-id="5a063-112">Ако например /mnt/backup е точка, можете да добавите /mnt/backup към списъка за изключване, като изпълните тази команда:</span><span class="sxs-lookup"><span data-stu-id="5a063-112">For example, if /mnt/backup is a mountpoint, you can add /mnt/backup to the exclude list by running this command:</span></span>

`$ mdatp exclusion folder add –path /mnt/backup`

<span data-ttu-id="5a063-113">**Забележка:** Добавянето на изключения увеличава риска злонамереният софтуер да не бъде откриван и трябва да се обработва и прилага внимателно.</span><span class="sxs-lookup"><span data-stu-id="5a063-113">**Note**: Adding exclusions increases the risk of malware not being detected and should be handled and implemented with care.</span></span>

## <a name="need-help"></a><span data-ttu-id="5a063-114">Имате нужда от помощ?</span><span class="sxs-lookup"><span data-stu-id="5a063-114">Need Help?</span></span>

<span data-ttu-id="5a063-115">За да ви помогне по най-ефективния начин, съберете диагностичните данни, преди да отворите калъф за поддръжка.</span><span class="sxs-lookup"><span data-stu-id="5a063-115">To assist you in the most efficient way, collect the diagnostic data before opening a support case.</span></span>
