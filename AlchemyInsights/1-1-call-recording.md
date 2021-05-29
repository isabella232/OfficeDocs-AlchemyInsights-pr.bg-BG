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
# <a name="11-call-recording"></a>1:1 запис на повикване

Ако **бутонът "Старт** запис" е в сиво в разговор в 1:1, трябва да промените настройките на правилата за засегнатия потребител. За да проверите настройката на правилата, изпълнете настройката Диагностика за засегнатия потребител, като въведете **Diag: Teams 1:1 Записване на повикването по-горе.**     

От 31 май 2021 г. ще започнем да изискваме нов Teams за обаждания *AllowCloudRecordingForCalls*. Преди тази промяна записът на разговор в 1:1 се управлява от *AllowCloudRecording Teams* за събрание. Тази промяна е документирана в публикацията в центъра за съобщения: [(актуализирана) 1:1 Въведение в правилата за записване на повикването.](https://portal.microsoft.com/Adminportal/Home?ref=MessageCenter/:/messages/MC238796)  

*AllowCloudRecordingForCalls*   опцията за правила за обаждания е **зададена $False по** подразбиране. Ако предпочитате да блокирате записването на повиквания от всички потребители 1:1, не е необходимо да предприемате никакви действия.  

За да разрешите записването на повиквания за всички потребители в 1:1 [повиквания, използвайте Teams PowerShell,](/microsoftteams/teams-powershell-install) за да изпълните следната кратка команда: 

**Set-CsTeamsCallingPolicy -Identity Global -AllowCloudRecordingForCalls $True** 

Като алтернатива можете да създадете нова политика и да зададете **-AllowCloudRecordingForCalls** **да $true** и да присвоите тези правила на вашите потребители. 

За повече информация вижте [1:1 Контролите за правила за записване на повикване са (почти!) Тук](https://techcommunity.microsoft.com/t5/microsoft-teams-support/1-1-call-recording-policy-controls-are-almost-here/ba-p/2217668).
