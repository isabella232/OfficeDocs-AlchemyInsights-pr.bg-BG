---
title: Грешки при синхронизиране на устройства на Apple за автоматично записване
ms.author: v-jmathew
author: v-jmathew
manager: scotv
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000654"
- "7256"
ms.openlocfilehash: 912c9e56b4c468fb333769f15bd7c212594dc11a
ms.sourcegitcommit: 6741a997fff871d263f92d3ff7fb61e7755956a9
ms.translationtype: MT
ms.contentlocale: bg-BG
ms.lasthandoff: 03/04/2021
ms.locfileid: "50448911"
---
# <a name="apple-automatic-device-enrollment-sync-errors"></a><span data-ttu-id="003ce-102">Грешки при синхронизиране на устройства на Apple за автоматично записване</span><span class="sxs-lookup"><span data-stu-id="003ce-102">Apple Automatic Device Enrollment sync errors</span></span>

<span data-ttu-id="003ce-103">"Установихме, че имате един или повече маркери за ЕЙД/DEP, които са в състояние на грешка.</span><span class="sxs-lookup"><span data-stu-id="003ce-103">“We have detected that you have one or more ADE/DEP Tokens which are in an error state.</span></span> <span data-ttu-id="003ce-104">Докато не бъде решено състоянието на грешката за всеки от засегнатите маркери, функцията ЕЙД няма да работи по очаквания начин.</span><span class="sxs-lookup"><span data-stu-id="003ce-104">Until the error state is resolved for each affected token, the ADE functionality will not work as expected.”.</span></span>

<span data-ttu-id="003ce-105">Тази грешка може да се покаже по много начини, включително:</span><span class="sxs-lookup"><span data-stu-id="003ce-105">This error might manifest in a number of ways including:</span></span>

1. <span data-ttu-id="003ce-106">Устройства, които не могат да се синхронизират от УД/ASM за настройване</span><span class="sxs-lookup"><span data-stu-id="003ce-106">Devices may not sync from ABM/ASM to Intune</span></span>
2. <span data-ttu-id="003ce-107">Присвояване на профил на записването може да е неуспешно</span><span class="sxs-lookup"><span data-stu-id="003ce-107">Enrollment profile assignments may be failing</span></span>
3. <span data-ttu-id="003ce-108">Устройството може да не завърши успешно записването на ЕЙД</span><span class="sxs-lookup"><span data-stu-id="003ce-108">Devices may not complete ADE enrollment successfully</span></span>

<span data-ttu-id="003ce-109">Проверете дали грешката при синхронизиране е съобщена в конзолата за настройване под **устройства > запишат устройства > iTunes записващи програми > маркери** за записвания.</span><span class="sxs-lookup"><span data-stu-id="003ce-109">Check for the sync error reported in the Intune console under **Devices > Enroll Devices > Apple enrollment > Enrollment program tokens**.</span></span>

<span data-ttu-id="003ce-110">Една от най-често срещаните причини за грешка при синхронизиране е изтичането на текущия маркер.</span><span class="sxs-lookup"><span data-stu-id="003ce-110">One of the most common causes of sync error is expiration of the current token.</span></span> <span data-ttu-id="003ce-111">В много случаи подновяването на засегнатия маркер ще реши проблема.</span><span class="sxs-lookup"><span data-stu-id="003ce-111">In many cases,renewal of the affected token will resolve the issue.</span></span>

<span data-ttu-id="003ce-112">Ако един или повече от вашите маркери е изтекъл, вижте следната документация, която ще ви помогне да ги подновите по подходящ начин:</span><span class="sxs-lookup"><span data-stu-id="003ce-112">If one or more of your tokens has expired,  see the following documentation to help you renew them as appropriate:</span></span>

[<span data-ttu-id="003ce-113">Подновяване на маркер за автоматично записване на устройство</span><span class="sxs-lookup"><span data-stu-id="003ce-113">Renew an Automated Device Enrollment token</span></span>](https://docs.microsoft.com/mem/intune/enrollment/device-enrollment-program-enroll-ios#renew-an-automated-device-enrollment-token)

<span data-ttu-id="003ce-114">Освен това можете да видите следната документация, за да видите потенциални отстраняване на грешки, които причиняват неуспехи при синхронизиране на маркери:</span><span class="sxs-lookup"><span data-stu-id="003ce-114">In addition, you can see the following documentation to see potential remediations for other errors causing token synchronization failures:</span></span>

[<span data-ttu-id="003ce-115">Грешки при синхронизиране на УД/ASM за iOS/iPadOS и автоматични маркери за записване на устройства с macOS</span><span class="sxs-lookup"><span data-stu-id="003ce-115">ABM/ASM Sync Errors for iOS/iPadOS and macOS Automated Device Enrollment Tokens</span></span>](https://docs.microsoft.com/mem/intune/enrollment/troubleshoot-ios-enrollment-errors#sync-token-errors-between-intune-and-ade-dep)







[<span data-ttu-id="003ce-116">Грешки при синхронизиране на УД/ASM за iOS/iPadOS и автоматични маркери за записване на устройства с macOS</span><span class="sxs-lookup"><span data-stu-id="003ce-116">ABM/ASM Sync Errors for iOS/iPadOS and macOS Automated Device Enrollment Tokens</span></span>](https://docs.microsoft.com/mem/intune/enrollment/troubleshoot-ios-enrollment-errors#resolutions-when-syncing-tokens-between-intune-and-abmasm-for-automated-device-enrollment)
