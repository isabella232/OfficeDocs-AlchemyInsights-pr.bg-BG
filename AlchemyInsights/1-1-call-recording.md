---
title: 1:1 запис на повикване
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
ms.openlocfilehash: 18c68fee514681b2a81c3cfa022c29ce83834f22
ms.sourcegitcommit: 610a5d950cdf488870601762ef52d881e3e22a48
ms.translationtype: MT
ms.contentlocale: bg-BG
ms.lasthandoff: 05/28/2021
ms.locfileid: "52696911"
---
# <a name="11-call-recording"></a><span data-ttu-id="cc66e-102">1:1 запис на повикване</span><span class="sxs-lookup"><span data-stu-id="cc66e-102">1:1 call recording</span></span>

<span data-ttu-id="cc66e-103">Ако **бутонът "Старт** запис" е в сиво в разговор в 1:1, трябва да промените настройките на правилата за засегнатия потребител.</span><span class="sxs-lookup"><span data-stu-id="cc66e-103">If the **Start Recording** button is grayed out in a 1:1 call, you need to change the policy settings for the impacted user.</span></span>   

<span data-ttu-id="cc66e-104">От 31 май 2021 г. ще започнем да изискваме нов Teams за обаждания *AllowCloudRecordingForCalls*.</span><span class="sxs-lookup"><span data-stu-id="cc66e-104">Beginning May 31, 2021, we'll start enforcing a new Teams Calling Policy *AllowCloudRecordingForCalls*.</span></span> <span data-ttu-id="cc66e-105">Преди тази промяна записът на разговор в 1:1 се управлява от *AllowCloudRecording Teams* за събрание.</span><span class="sxs-lookup"><span data-stu-id="cc66e-105">Prior to this change, 1:1 call recording is controlled by the *AllowCloudRecording* Teams Meeting Policy.</span></span> <span data-ttu-id="cc66e-106">Тази промяна е документирана в публикацията в центъра за съобщения: [(актуализирана) 1:1 Въведение в правилата за записване на повикването.](https://portal.microsoft.com/Adminportal/Home?ref=MessageCenter/:/messages/MC238796)</span><span class="sxs-lookup"><span data-stu-id="cc66e-106">This change is documented in the Message Center post: [(Updated) 1:1 Call recording policy introduction](https://portal.microsoft.com/Adminportal/Home?ref=MessageCenter/:/messages/MC238796).</span></span>  

<span data-ttu-id="cc66e-107">*AllowCloudRecordingForCalls*   опцията за правила за обаждания е **зададена $False по** подразбиране.</span><span class="sxs-lookup"><span data-stu-id="cc66e-107">*AllowCloudRecordingForCalls* calling policy option is set to **$False** by default.</span></span> <span data-ttu-id="cc66e-108">Ако предпочитате да блокирате записването на повиквания от всички потребители 1:1, не е необходимо да предприемате никакви действия.</span><span class="sxs-lookup"><span data-stu-id="cc66e-108">If you prefer to block all users from recording 1:1 calls, you don't need to take any action.</span></span>  

<span data-ttu-id="cc66e-109">За да разрешите записването на повиквания за всички потребители в 1:1 повиквания, използвайте Teams PowerShell, за да изпълните следната кратка команда:</span><span class="sxs-lookup"><span data-stu-id="cc66e-109">To enable call recording for all users in 1:1 calls use Teams PowerShell to run the following cmdlet:</span></span> 

<span data-ttu-id="cc66e-110">**Set-CsTeamsCallingPolicy -Identity Global -AllowCloudRecordingForCalls $True**</span><span class="sxs-lookup"><span data-stu-id="cc66e-110">**Set-CsTeamsCallingPolicy -Identity Global -AllowCloudRecordingForCalls $True**</span></span> 

<span data-ttu-id="cc66e-111">Като алтернатива можете да създадете нова политика и да зададете **-AllowCloudRecordingForCalls** **да $true** и да присвоите тези правила на вашите потребители.</span><span class="sxs-lookup"><span data-stu-id="cc66e-111">Alternatively, you can create a new policy and set **-AllowCloudRecordingForCalls** to **$true** and assign that policy to your users.</span></span> 

<span data-ttu-id="cc66e-112">За повече информация вижте [1:1 Контролите за правила за записване на повикване са (почти!) Тук](https://techcommunity.microsoft.com/t5/microsoft-teams-support/1-1-call-recording-policy-controls-are-almost-here/ba-p/2217668).</span><span class="sxs-lookup"><span data-stu-id="cc66e-112">For more information, see [1:1 Call Recording Policy Controls Are (Almost!) Here](https://techcommunity.microsoft.com/t5/microsoft-teams-support/1-1-call-recording-policy-controls-are-almost-here/ba-p/2217668).</span></span>
