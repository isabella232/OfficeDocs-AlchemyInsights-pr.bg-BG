---
title: Проблеми с вградените машини
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/14/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "6023"
- "9002913"
ms.openlocfilehash: c3203ed68eb19d5f6d75eb2269094bb0422b14cc
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: bg-BG
ms.lasthandoff: 09/14/2020
ms.locfileid: "47676871"
---
# <a name="issues-with-onboarding-machines"></a><span data-ttu-id="35a91-102">Проблеми с вградените машини</span><span class="sxs-lookup"><span data-stu-id="35a91-102">Issues with onboarding machines</span></span>

<span data-ttu-id="35a91-103">Възможно е да имате проблеми с вградените машини към услугата MDATP.</span><span class="sxs-lookup"><span data-stu-id="35a91-103">You might have issues with onboarding machines to MDATP service.</span></span> <span data-ttu-id="35a91-104">Ако имате достъп до крайния потребител, изпълнете следните стъпки:</span><span class="sxs-lookup"><span data-stu-id="35a91-104">If you can access the end-user machine, follow these steps:</span></span>

1. <span data-ttu-id="35a91-105">Изтеглете диагностичния инструмент за [анализатор на свързването на клиенти](https://aka.ms/mdatpanalyzer) .</span><span class="sxs-lookup"><span data-stu-id="35a91-105">Download the [Client Connectivity Analyzer](https://aka.ms/mdatpanalyzer) diagnostic tool.</span></span>
2. <span data-ttu-id="35a91-106">Extract и Run MDATPAnalyzer. cmd.</span><span class="sxs-lookup"><span data-stu-id="35a91-106">Extract and run MDATPAnalyzer.cmd.</span></span>
3. <span data-ttu-id="35a91-107">Намерете диагностичния регистрационен файл в папката, наречена MDATPClientAnalyzerResult, в същата папка, където се изтегля инструментът Analyzer.</span><span class="sxs-lookup"><span data-stu-id="35a91-107">Locate the diagnostic log in the folder called MDATPClientAnalyzerResult, the same folder where the Analyzer tool is downloaded.</span></span>
4. <span data-ttu-id="35a91-108">Прегледайте регистрационния файл MDATPClientAnalyzer.txt, за да намерите проблеми с настройките за свързване или интернет прокси сървъра.</span><span class="sxs-lookup"><span data-stu-id="35a91-108">Review the log file, MDATPClientAnalyzer.txt, to find connectivity or internet proxy settings issues.</span></span>