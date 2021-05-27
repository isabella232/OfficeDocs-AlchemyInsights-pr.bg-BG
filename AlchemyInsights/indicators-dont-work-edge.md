---
title: Индикаторите не работят с помощта на браузъра Edge
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 05/25/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "11230"
- "9005470"
ms.openlocfilehash: df62d965e0dc2ddb656571af99b1e4c3cb52ea35
ms.sourcegitcommit: 4b504650e11adb9894c37b6d8608b53f9d5fc13d
ms.translationtype: MT
ms.contentlocale: bg-BG
ms.lasthandoff: 05/25/2021
ms.locfileid: "52676076"
---
# <a name="indicators-dont-work-using-edge-browser"></a><span data-ttu-id="de0e0-102">Индикаторите не работят с помощта на браузъра Edge</span><span class="sxs-lookup"><span data-stu-id="de0e0-102">Indicators don't work using Edge browser</span></span>

<span data-ttu-id="de0e0-103">След като сте създали индикатор, не е зачетен от Edge (Smartscreen).</span><span class="sxs-lookup"><span data-stu-id="de0e0-103">After you created an Indicator, it's not honored by Edge (Smartscreen).</span></span> <span data-ttu-id="de0e0-104">За повече информация вижте Създаване [на индикатори за ИД и URL адреси/домейни.](/microsoft-365/security/defender-endpoint/indicator-ip-domain)</span><span class="sxs-lookup"><span data-stu-id="de0e0-104">For more information, see [Create indicators for IPs and URLs/domains](/microsoft-365/security/defender-endpoint/indicator-ip-domain).</span></span>

## <a name="step-1-ensure-the-following"></a><span data-ttu-id="de0e0-105">Стъпка 1: Уверете се, че:</span><span class="sxs-lookup"><span data-stu-id="de0e0-105">Step 1: Ensure the following</span></span>

- <span data-ttu-id="de0e0-106">Уверете се, че индикаторът е правилен (без печатни грешки в IP/URL адрес, правилно действие, правилните групи на RBAC).</span><span class="sxs-lookup"><span data-stu-id="de0e0-106">Verify that the indicator is correct (no typos in IP/URL, correct action, the correct RBAC groups).</span></span>
- <span data-ttu-id="de0e0-107">Изчакайте най-малко 2 часа след създаването на индикатора, за да се вземе предвид евентуалното закъснение.</span><span class="sxs-lookup"><span data-stu-id="de0e0-107">Wait the minimum 2 hours after creating the indicator to take into account any possible latency.</span></span>
- <span data-ttu-id="de0e0-108">Уверете се, че системата(ите) са внедрани в Microsoft Defender за крайна точка.</span><span class="sxs-lookup"><span data-stu-id="de0e0-108">Confirm that the system(s) are onboarded to Microsoft Defender for Endpoint.</span></span>
- <span data-ttu-id="de0e0-109">Уверете се, че системата(ите) могат да комуникират с облака.</span><span class="sxs-lookup"><span data-stu-id="de0e0-109">Verify that system(s) can communicate with the Cloud.</span></span>
- <span data-ttu-id="de0e0-110">Уверете се, че Smartscreen е разрешен и до който може да се достигне, като стигнете [до тестовия сайт](https://demo.smartscreen.msft.net).</span><span class="sxs-lookup"><span data-stu-id="de0e0-110">Verify that Smartscreen is enabled and reachable by going to the [test site](https://demo.smartscreen.msft.net).</span></span>

## <a name="step-2-troubleshoot-the-potential-issue"></a><span data-ttu-id="de0e0-111">Стъпка 2: Отстраняване на потенциалния проблем</span><span class="sxs-lookup"><span data-stu-id="de0e0-111">Step 2: Troubleshoot the potential issue</span></span>

- <span data-ttu-id="de0e0-112">Уверете се, че клиентът отговаря на изискванията.</span><span class="sxs-lookup"><span data-stu-id="de0e0-112">Make sure the client meets the requirements.</span></span> <span data-ttu-id="de0e0-113">За подробности вижте Създаване [на индикатори за ИД и URL адреси/домейни.](/microsoft-365/security/defender-endpoint/indicator-ip-domain)</span><span class="sxs-lookup"><span data-stu-id="de0e0-113">For details, see [Create indicators for IPs and URLs/domains](/microsoft-365/security/defender-endpoint/indicator-ip-domain).</span></span>
- <span data-ttu-id="de0e0-114">Уверете се, че използвате най-новата версия на браузъра Edge.</span><span class="sxs-lookup"><span data-stu-id="de0e0-114">Make sure you're running the latest version of the Edge browser.</span></span> <span data-ttu-id="de0e0-115">За да разберете най-новата версия, [вижте Разберете коя версия на Microsoft Edge имате](https://support.microsoft.com/microsoft-edge/find-out-which-version-of-microsoft-edge-you-have-c726bee8-c42e-e472-e954-4cf5123497eb).</span><span class="sxs-lookup"><span data-stu-id="de0e0-115">To find out the latest version, see [Find out which version of Microsoft Edge you have](https://support.microsoft.com/microsoft-edge/find-out-which-version-of-microsoft-edge-you-have-c726bee8-c42e-e472-e954-4cf5123497eb).</span></span>
- <span data-ttu-id="de0e0-116">Рестартирайте браузъра Edge.</span><span class="sxs-lookup"><span data-stu-id="de0e0-116">Restart the Edge browser.</span></span>
- <span data-ttu-id="de0e0-117">Навигирайте до сайта, за който имате настройка на индикатор.</span><span class="sxs-lookup"><span data-stu-id="de0e0-117">Navigate to the site for which you have setup an indicator.</span></span> <span data-ttu-id="de0e0-118">Ако сайтът не се показва по очаквания начин, продължете със стъпка 3.</span><span class="sxs-lookup"><span data-stu-id="de0e0-118">If the site does not appear as expected, continue to Step 3.</span></span> 

## <a name="step-3-collect-data"></a><span data-ttu-id="de0e0-119">Стъпка 3: Събиране на данни</span><span class="sxs-lookup"><span data-stu-id="de0e0-119">Step 3: Collect data</span></span>

- <span data-ttu-id="de0e0-120">Събиране **на диагностични данни от MDEClientAnalyzer.**</span><span class="sxs-lookup"><span data-stu-id="de0e0-120">Collect **MDEClientAnalyzer** diagnostic data.</span></span> <span data-ttu-id="de0e0-121">За инструкции вижте Проблеми [с компютрите за табло към Microsoft Defender за крайна точка.](issues-with-onboarding-machines.md)</span><span class="sxs-lookup"><span data-stu-id="de0e0-121">For instructions, see [Issues with onboarding machines to Microsoft Defender for Endpoint](issues-with-onboarding-machines.md).</span></span>
- <span data-ttu-id="de0e0-122">Ако ви е удобно да инсталирате и събирате проследяване на Fiddler, вижте [Telerik Fiddler](http://www.telerik.com/fiddler).</span><span class="sxs-lookup"><span data-stu-id="de0e0-122">If you are comfortable installing and collecting a Fiddler trace, see [Telerik Fiddler](http://www.telerik.com/fiddler).</span></span>
- <span data-ttu-id="de0e0-123">Ако предпочитате указания от поддръжката на Microsoft, изберете иконата Поддръжка по-долу, за да отворите калъф за поддръжка.</span><span class="sxs-lookup"><span data-stu-id="de0e0-123">If you prefer guidance from Microsoft Support, select the Support icon below to open a support case.</span></span>
