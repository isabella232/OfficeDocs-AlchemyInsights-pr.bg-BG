---
title: Отстраняването на неизправности с ediscovery има грешки
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 05/20/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "11274"
- "3200003"
ms.openlocfilehash: 1df2b7153cac99419adc4f72b1c3732e7c746eac
ms.sourcegitcommit: 730efbac8eec016b2b4f83f1b0e01e077f28c444
ms.translationtype: MT
ms.contentlocale: bg-BG
ms.lasthandoff: 05/20/2021
ms.locfileid: "52676035"
---
# <a name="troubleshooting-ediscovery-holds-errors"></a><span data-ttu-id="2c179-102">Отстраняването на неизправности с ediscovery има грешки</span><span class="sxs-lookup"><span data-stu-id="2c179-102">Troubleshooting ediscovery holds errors</span></span>

<span data-ttu-id="2c179-103">Имате проблеми с задържането на електронни данни?</span><span class="sxs-lookup"><span data-stu-id="2c179-103">Experiencing issues with eDiscovery holds?</span></span> <span data-ttu-id="2c179-104">Ето някои най-добри практики, които трябва да имате предвид:</span><span class="sxs-lookup"><span data-stu-id="2c179-104">Here are some best practices to consider:</span></span>

- <span data-ttu-id="2c179-105">Проверете състоянието на задържане на разпределението.</span><span class="sxs-lookup"><span data-stu-id="2c179-105">Check the hold distribution status.</span></span>  <span data-ttu-id="2c179-106">Ако състоянието е **On (Pending)** или **Off (Pending)**, изчакайте, за да завърши разпределението на задържането.</span><span class="sxs-lookup"><span data-stu-id="2c179-106">If status is **On (Pending)** or **Off (Pending)**, wait for hold distribution to complete.</span></span>
- <span data-ttu-id="2c179-107">Обединяването на откриване на електронни данни задържа актуализациите в едно групово искане, вместо да актуализира правилата неколкократно за всяка транзакция.</span><span class="sxs-lookup"><span data-stu-id="2c179-107">Merge eDiscovery hold updates into a single bulk request instead of updating the policy repeatedly for each transaction.</span></span>
- <span data-ttu-id="2c179-108">Изпълнете Set-CaseHoldPolicy <policyname> -RetryDistribution в Powershell на центъра за защита и съответствие.</span><span class="sxs-lookup"><span data-stu-id="2c179-108">Run Set-CaseHoldPolicy <policyname> -RetryDistribution in the Security and Compliance Center Powershell.</span></span> <span data-ttu-id="2c179-109">За подробности вижте Информация [Свързване центъра за & съответствие на PowerShell.](/powershell/exchange/connect-to-scc-powershell)</span><span class="sxs-lookup"><span data-stu-id="2c179-109">For details, see [Connect to Security & Compliance Center PowerShell](/powershell/exchange/connect-to-scc-powershell).</span></span>

<span data-ttu-id="2c179-110">За стъпки за проверка на тези настройки и допълнителни най-добри практики за ограничаване и разрешаване на откриване на електронни данни има проблеми, вижте Отстраняване на грешки при откриване [на електронни данни.](/microsoft-365/compliance/hold-distribution-errors)</span><span class="sxs-lookup"><span data-stu-id="2c179-110">For steps to check these settings and additional best practices for mitigating and resolving eDiscovery holds issues, see [Troubleshoot eDiscovery hold errors](/microsoft-365/compliance/hold-distribution-errors).</span></span>
<span data-ttu-id="2c179-111">За информация относно отстраняването на други често срещани проблеми с откриване на електронни данни вижте Изследване, отстраняване на неизправности и отстраняване на [често срещани проблеми с откриване на електронни данни](/microsoft-365/compliance/ediscovery-troubleshooting-common-issues).</span><span class="sxs-lookup"><span data-stu-id="2c179-111">For info about troubleshooting other common eDiscovery issues, see [Investigate, troubleshoot, and resolve common eDiscovery issues](/microsoft-365/compliance/ediscovery-troubleshooting-common-issues).</span></span>
