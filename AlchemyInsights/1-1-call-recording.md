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
ms.openlocfilehash: 8cdadf34a059856338d7f40528446b70373465e4
ms.sourcegitcommit: d2108b13acc44e26b65f9a2739cbce9bf98959a5
ms.translationtype: MT
ms.contentlocale: bg-BG
ms.lasthandoff: 05/28/2021
ms.locfileid: "52702079"
---
# <a name="11-call-recording"></a><span data-ttu-id="719f2-102">1:1 запис на повикване</span><span class="sxs-lookup"><span data-stu-id="719f2-102">1:1 call recording</span></span>

<span data-ttu-id="719f2-103">Ако **бутонът "Старт** запис" е в сиво в разговор в 1:1, трябва да промените настройките на правилата за засегнатия потребител.</span><span class="sxs-lookup"><span data-stu-id="719f2-103">If the **Start Recording** button is grayed out in a 1:1 call, you need to change the policy settings for the impacted user.</span></span> <span data-ttu-id="719f2-104">За да проверите настройката на правилата, изпълнете настройката Диагностика за засегнатия потребител, като въведете **Diag: Teams 1:1 Записване на повикването по-горе.**</span><span class="sxs-lookup"><span data-stu-id="719f2-104">To check the policy setting, run the Diagnostic for the impacted user by typing **Diag: Teams 1:1 Call Recording** above.</span></span>     

<span data-ttu-id="719f2-105">От 31 май 2021 г. ще започнем да изискваме нов Teams за обаждания *AllowCloudRecordingForCalls*.</span><span class="sxs-lookup"><span data-stu-id="719f2-105">Beginning May 31, 2021, we'll start enforcing a new Teams Calling Policy *AllowCloudRecordingForCalls*.</span></span> <span data-ttu-id="719f2-106">Преди тази промяна записът на разговор в 1:1 се управлява от *AllowCloudRecording Teams* за събрание.</span><span class="sxs-lookup"><span data-stu-id="719f2-106">Prior to this change, 1:1 call recording is controlled by the *AllowCloudRecording* Teams Meeting Policy.</span></span> <span data-ttu-id="719f2-107">Тази промяна е документирана в публикацията в центъра за съобщения: [(актуализирана) 1:1 Въведение в правилата за записване на повикването.](https://portal.microsoft.com/Adminportal/Home?ref=MessageCenter/:/messages/MC238796)</span><span class="sxs-lookup"><span data-stu-id="719f2-107">This change is documented in the Message Center post: [(Updated) 1:1 Call recording policy introduction](https://portal.microsoft.com/Adminportal/Home?ref=MessageCenter/:/messages/MC238796).</span></span>  

<span data-ttu-id="719f2-108">*AllowCloudRecordingForCalls*   опцията за правила за обаждания е **зададена $False по** подразбиране.</span><span class="sxs-lookup"><span data-stu-id="719f2-108">*AllowCloudRecordingForCalls* calling policy option is set to **$False** by default.</span></span> <span data-ttu-id="719f2-109">Ако предпочитате да блокирате записването на повиквания от всички потребители 1:1, не е необходимо да предприемате никакви действия.</span><span class="sxs-lookup"><span data-stu-id="719f2-109">If you prefer to block all users from recording 1:1 calls, you don't need to take any action.</span></span>  

<span data-ttu-id="719f2-110">За да разрешите записването на повиквания за всички потребители в 1:1 [повиквания, използвайте Teams PowerShell,](/microsoftteams/teams-powershell-install) за да изпълните следната кратка команда:</span><span class="sxs-lookup"><span data-stu-id="719f2-110">To enable call recording for all users in 1:1 calls use [Teams PowerShell](/microsoftteams/teams-powershell-install) to run the following cmdlet:</span></span> 

<span data-ttu-id="719f2-111">**Set-CsTeamsCallingPolicy -Identity Global -AllowCloudRecordingForCalls $True**</span><span class="sxs-lookup"><span data-stu-id="719f2-111">**Set-CsTeamsCallingPolicy -Identity Global -AllowCloudRecordingForCalls $True**</span></span> 

<span data-ttu-id="719f2-112">Като алтернатива можете да създадете нова политика и да зададете **-AllowCloudRecordingForCalls** **да $true** и да присвоите тези правила на вашите потребители.</span><span class="sxs-lookup"><span data-stu-id="719f2-112">Alternatively, you can create a new policy and set **-AllowCloudRecordingForCalls** to **$true** and assign that policy to your users.</span></span> 

<span data-ttu-id="719f2-113">За повече информация вижте [1:1 Контролите за правила за записване на повикване са (почти!) Тук](https://techcommunity.microsoft.com/t5/microsoft-teams-support/1-1-call-recording-policy-controls-are-almost-here/ba-p/2217668).</span><span class="sxs-lookup"><span data-stu-id="719f2-113">For more information, see [1:1 Call Recording Policy Controls Are (Almost!) Here](https://techcommunity.microsoft.com/t5/microsoft-teams-support/1-1-call-recording-policy-controls-are-almost-here/ba-p/2217668).</span></span>
