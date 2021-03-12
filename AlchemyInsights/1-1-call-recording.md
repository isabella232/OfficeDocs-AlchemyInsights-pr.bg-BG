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
# <a name="11-call-recording"></a>запис за обаждане на 1:1

Администраторите трябва да предприемат действие сега, за да продължат да позволяват на потребителите да записват 1:1 повиквания.
 
От 12 Април 2021 г. ние започваме да прилагаме опцията за правила за *AllowCloudRecordingForCalls* за набиране на нови отбори. 

В момента възможностите за записване на повиквания на 1:1 се контролират от опцията *AllowCloudRecording* в правилата за събрания в Teams. Ако вашите потребители имат разрешение за записване на събрания на Teams, те също могат да записват 1:1 повиквания.

Ако предпочитате да блокирате всички потребители от записването на повиквания на 1:1, не е необходимо да предприемате никакви действия. Опцията за правила за *AllowCloudRecordingForCalls* повиквания ще бъде $FALSE по подразбиране.

Тази промяна е документирана в следния център за съобщения Публикувай: [(актуализиран) 1:1 за записване на правила за запис на повикването](https://portal.microsoft.com/Adminportal/Home?ref=MessageCenter/:/messages/MC238796) , за да зададете опцията за правила за обаждания на Teams, трябва да използвате [Teams PowerShell](https://docs.microsoft.com/microsoftteams/teams-powershell-install).

**За да разрешите записването на повикванията в 1:1 повиквания:** Set-CsTeamsCallingPolicy в Global-AllowCloudRecordingForCalls $True

**За да забраните записването на повиквания в 1:1 обаждания:** Set-CsTeamsCallingPolicy за глобално AllowCloudRecordingForCalls $FALSE

