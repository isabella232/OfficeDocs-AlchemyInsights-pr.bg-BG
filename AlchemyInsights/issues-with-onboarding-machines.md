---
title: Проблеми с вградените машини за Microsoft Defender за крайни точки
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
ms.openlocfilehash: 7ccec69f8ab43f277978176519a7f8f8df443846
ms.sourcegitcommit: 1d73771d147325cfd8578e6816becd8331913890
ms.translationtype: MT
ms.contentlocale: bg-BG
ms.lasthandoff: 03/19/2021
ms.locfileid: "50901556"
---
# <a name="issues-with-onboarding-machines-to-microsoft-defender-for-endpoints"></a><span data-ttu-id="64be6-102">Проблеми с вградените машини за Microsoft Defender за крайни точки</span><span class="sxs-lookup"><span data-stu-id="64be6-102">Issues with onboarding machines to Microsoft Defender for Endpoints</span></span>

<span data-ttu-id="64be6-103">Възможно е да имате проблеми с вградените машини в MDE услугата.</span><span class="sxs-lookup"><span data-stu-id="64be6-103">You might have issues with onboarding machines to MDE service.</span></span> <span data-ttu-id="64be6-104">Ако имате достъп до крайния потребител, изпълнете следните стъпки:</span><span class="sxs-lookup"><span data-stu-id="64be6-104">If you can access the end-user machine, follow these steps:</span></span>

1. <span data-ttu-id="64be6-105">Изтеглете най-новата версия на предварителния преглед на инструмента за диагностика на [анализатори за клиента](https://aka.ms/betamdeanalyzer) .</span><span class="sxs-lookup"><span data-stu-id="64be6-105">Download the latest preview version of the [MDE Client Analyzer](https://aka.ms/betamdeanalyzer) diagnostic tool.</span></span>
2. <span data-ttu-id="64be6-106">Щракнете с десния бутон върху **MDEClientAnalyzer. cmd** и изберете "Изпълнявай като администратор".</span><span class="sxs-lookup"><span data-stu-id="64be6-106">Right click **MDEClientAnalyzer.cmd** and select ‘Run as administrator’.</span></span>
3. <span data-ttu-id="64be6-107">Следвайте указанията, предложени в **MDEClientAnalyzer.htm**.</span><span class="sxs-lookup"><span data-stu-id="64be6-107">Follow any guidance suggested in **MDEClientAnalyzer.htm**.</span></span>
4. <span data-ttu-id="64be6-108">За по-подробна информация за регистрите прегледайте създадената подпапка с име **MDEClientAnalyzerResult**.</span><span class="sxs-lookup"><span data-stu-id="64be6-108">For more verbose logs, review the created sub-folder named **MDEClientAnalyzerResult**.</span></span>
5. <span data-ttu-id="64be6-109">Ако са необходими допълнителни указания, се обърнете към [поддръжката на Microsoft Defender за крайна точка](https://docs.microsoft.com/windows/security/threat-protection/microsoft-defender-atp/contact-support) и предоставете получения MDEClientAnalyzerResult.zip файл за анализ.</span><span class="sxs-lookup"><span data-stu-id="64be6-109">If additional guidance is needed, contact [Microsoft Defender for Endpoint support](https://docs.microsoft.com/windows/security/threat-protection/microsoft-defender-atp/contact-support) and provide the resulting MDEClientAnalyzerResult.zip file for analysis.</span></span>
