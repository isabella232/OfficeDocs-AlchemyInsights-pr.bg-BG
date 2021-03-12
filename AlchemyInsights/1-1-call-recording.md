---
title: запис за обаждане на 1:1
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 12/18/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9002530"
- "7648"
ms.openlocfilehash: af09e8805409446a42a62c82aa577ad27f09a17a
ms.sourcegitcommit: 6312ee31561db36104f32282d019d069ede69174
ms.translationtype: MT
ms.contentlocale: bg-BG
ms.lasthandoff: 03/11/2021
ms.locfileid: "50733838"
---
# <a name="11-call-recording"></a><span data-ttu-id="6c975-102">запис за обаждане на 1:1</span><span class="sxs-lookup"><span data-stu-id="6c975-102">1:1 call recording</span></span>

<span data-ttu-id="6c975-103">Администраторите трябва да предприемат действие сега, за да продължат да позволяват на потребителите да записват 1:1 повиквания.</span><span class="sxs-lookup"><span data-stu-id="6c975-103">Administrators need to take action now to continue allowing users to Record 1:1 calls.</span></span>
 
<span data-ttu-id="6c975-104">От 12 Април 2021 г. ние започваме да прилагаме опцията за правила за *AllowCloudRecordingForCalls* за набиране на нови отбори.</span><span class="sxs-lookup"><span data-stu-id="6c975-104">Beginning April 12, 2021, we will start enforcing a new Teams Calling Policy option *AllowCloudRecordingForCalls*.</span></span> 

<span data-ttu-id="6c975-105">В момента възможностите за записване на повиквания на 1:1 се контролират от опцията *AllowCloudRecording* в правилата за събрания в Teams.</span><span class="sxs-lookup"><span data-stu-id="6c975-105">Currently 1:1 call recording capabilities are controlled by the *AllowCloudRecording* option in Teams Meeting Policies.</span></span> <span data-ttu-id="6c975-106">Ако вашите потребители имат разрешение за записване на събрания на Teams, те също могат да записват 1:1 повиквания.</span><span class="sxs-lookup"><span data-stu-id="6c975-106">If your users are allowed to record Teams Meetings they can also record 1:1 calls.</span></span>

<span data-ttu-id="6c975-107">Ако предпочитате да блокирате всички потребители от записването на повиквания на 1:1, не е необходимо да предприемате никакви действия.</span><span class="sxs-lookup"><span data-stu-id="6c975-107">If you prefer to block all users from recording 1:1 calls, you do not need to take any action.</span></span> <span data-ttu-id="6c975-108">Опцията за правила за *AllowCloudRecordingForCalls* повиквания ще бъде $FALSE по подразбиране.</span><span class="sxs-lookup"><span data-stu-id="6c975-108">*AllowCloudRecordingForCalls* calling policy option will be $False by default.</span></span>

<span data-ttu-id="6c975-109">Тази промяна е документирана в следния център за съобщения Публикувай: [(актуализиран) 1:1 за записване на правила за запис на повикването](https://portal.microsoft.com/Adminportal/Home?ref=MessageCenter/:/messages/MC238796) , за да зададете опцията за правила за обаждания на Teams, трябва да използвате [Teams PowerShell](https://docs.microsoft.com/microsoftteams/teams-powershell-install).</span><span class="sxs-lookup"><span data-stu-id="6c975-109">This change is documented in the following Message Center Post: [(Updated) 1:1 Call recording policy introduction](https://portal.microsoft.com/Adminportal/Home?ref=MessageCenter/:/messages/MC238796) To set the Teams Calling Policy Option you must use [Teams PowerShell](https://docs.microsoft.com/microsoftteams/teams-powershell-install).</span></span>

<span data-ttu-id="6c975-110">**За да разрешите записването на повикванията в 1:1 повиквания:** Set-CsTeamsCallingPolicy в Global-AllowCloudRecordingForCalls $True</span><span class="sxs-lookup"><span data-stu-id="6c975-110">**To enable call recording in 1:1 calls:** Set-CsTeamsCallingPolicy -Identity Global -AllowCloudRecordingForCalls $True</span></span>

<span data-ttu-id="6c975-111">**За да забраните записването на повиквания в 1:1 обаждания:** Set-CsTeamsCallingPolicy за глобално AllowCloudRecordingForCalls $FALSE</span><span class="sxs-lookup"><span data-stu-id="6c975-111">**To disable call recording in 1:1 calls:** Set-CsTeamsCallingPolicy -Identity Global -AllowCloudRecordingForCalls $False</span></span>

