---
title: Грешки при синхронизиране на устройства на Apple за автоматично записване
ms.author: v-jmathew
author: v-jmathew
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000654"
- "7256"
ms.openlocfilehash: d7a9398046a1073e30fdbe2950f750bb55d4fa2f
ms.sourcegitcommit: 87c8d0a1e6668211b9dd5427f98984ccdcadb02d
ms.translationtype: MT
ms.contentlocale: bg-BG
ms.lasthandoff: 12/17/2020
ms.locfileid: "49714667"
---
# <a name="apple-automatic-device-enrollment-sync-errors"></a><span data-ttu-id="89164-102">Грешки при синхронизиране на устройства на Apple за автоматично записване</span><span class="sxs-lookup"><span data-stu-id="89164-102">Apple Automatic Device Enrollment sync errors</span></span>

<span data-ttu-id="89164-103">"Установихме, че имате един или повече маркери за ЕЙД/DEP, които са в състояние на грешка.</span><span class="sxs-lookup"><span data-stu-id="89164-103">“We have detected that you have one or more ADE/DEP Tokens which are in an error state.</span></span> <span data-ttu-id="89164-104">Докато не бъде решено състоянието на грешката за всеки от засегнатите маркери, функцията ЕЙД няма да работи за един и същ ".</span><span class="sxs-lookup"><span data-stu-id="89164-104">Until the error state is resolved for each affected token, the ADE functionality will not work for the same”.</span></span>

<span data-ttu-id="89164-105">Тази грешка може да се покаже по много начини, включително:</span><span class="sxs-lookup"><span data-stu-id="89164-105">This error might manifest in a number of ways including:</span></span>

1. <span data-ttu-id="89164-106">Устройства, които не могат да се синхронизират от УД/ASM за настройване</span><span class="sxs-lookup"><span data-stu-id="89164-106">Devices may not sync from ABM/ASM to Intune</span></span>
2. <span data-ttu-id="89164-107">Присвояване на профил на записването може да е неуспешно</span><span class="sxs-lookup"><span data-stu-id="89164-107">Enrollment profile assignments may be failing</span></span>
3. <span data-ttu-id="89164-108">Устройството може да не завърши успешно записването на ЕЙД</span><span class="sxs-lookup"><span data-stu-id="89164-108">Devices may not complete ADE enrollment successfully</span></span>

<span data-ttu-id="89164-109">Проверете дали грешката при синхронизиране е съобщена в конзолата за настройване под **устройства > запишат устройства > iTunes записващи > маркери за програма за записване** и прегледайте следната документация, за да видите всяко евентуално саниране:</span><span class="sxs-lookup"><span data-stu-id="89164-109">Check for the sync error reported in the Intune console under **Devices > Enroll Devices > Apple enrollment > Enrollment program tokens** and review the following documentation to see any potential remediation:</span></span>

[<span data-ttu-id="89164-110">Грешки при синхронизиране на УД/ASM за iOS/iPadOS и автоматични маркери за записване на устройства с macOS</span><span class="sxs-lookup"><span data-stu-id="89164-110">ABM/ASM Sync Errors for iOS/iPadOS and macOS Automated Device Enrollment Tokens</span></span>](https://docs.microsoft.com/mem/intune/enrollment/troubleshoot-ios-enrollment-errors#resolutions-when-syncing-tokens-between-intune-and-abmasm-for-automated-device-enrollment)
