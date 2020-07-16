---
title: Проблеми с бордовите машини
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/14/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "6023"
- "9002913"
ms.openlocfilehash: 19b516dc21472e2c80a8b9046f802b329d15e4d6
ms.sourcegitcommit: 45c2aaeee58c0be466b76c7f0cd71e796d3c8f76
ms.translationtype: MT
ms.contentlocale: bg-BG
ms.lasthandoff: 07/15/2020
ms.locfileid: "45141321"
---
# <a name="issues-with-onboarding-machines"></a><span data-ttu-id="88f63-102">Проблеми с бордовите машини</span><span class="sxs-lookup"><span data-stu-id="88f63-102">Issues with onboarding machines</span></span>

<span data-ttu-id="88f63-103">Може да имате проблеми с бордовите машини за MDATP услуга.</span><span class="sxs-lookup"><span data-stu-id="88f63-103">You might have issues with onboarding machines to MDATP service.</span></span> <span data-ttu-id="88f63-104">Ако имате достъп до машината на крайния потребител, изпълнете следните стъпки:</span><span class="sxs-lookup"><span data-stu-id="88f63-104">If you can access the end-user machine, follow these steps:</span></span>

1. <span data-ttu-id="88f63-105">Изтеглете инструмента за диагностика на [клиент връзка анализатор.](https://aka.ms/mdatpanalyzer)</span><span class="sxs-lookup"><span data-stu-id="88f63-105">Download the [Client Connectivity Analyzer](https://aka.ms/mdatpanalyzer) diagnostic tool.</span></span>
2. <span data-ttu-id="88f63-106">Извличане и изпълнение MDATPAnalyzer.cmd.</span><span class="sxs-lookup"><span data-stu-id="88f63-106">Extract and run MDATPAnalyzer.cmd.</span></span>
3. <span data-ttu-id="88f63-107">Намерете диагностичен регистрационен файл в папката, наречена MDATPClientAnalyzerResult, същата папка, където инструментът анализатор се изтегля.</span><span class="sxs-lookup"><span data-stu-id="88f63-107">Locate the diagnostic log in the folder called MDATPClientAnalyzerResult, the same folder where the Analyzer tool is downloaded.</span></span>
4. <span data-ttu-id="88f63-108">Прегледайте регистрационния файл, MDATPClientAnalyzer.txt, да намерите проблеми с връзката или интернет прокси настройките.</span><span class="sxs-lookup"><span data-stu-id="88f63-108">Review the log file, MDATPClientAnalyzer.txt, to find connectivity or internet proxy settings issues.</span></span>