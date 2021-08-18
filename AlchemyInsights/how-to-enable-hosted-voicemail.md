---
title: Как да разрешите хостваната гласова поща
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 12/09/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9002347"
- "7563"
ms.openlocfilehash: 4042e042554f78febff2073fde6f14db72a6d4e0
ms.sourcegitcommit: ab75f66355116e995b3cb5505465b31989339e28
ms.translationtype: MT
ms.contentlocale: bg-BG
ms.lasthandoff: 08/13/2021
ms.locfileid: "58318637"
---
# <a name="how-to-enable-hosted-voicemail"></a>Как да разрешите хостваната гласова поща

За да разрешите гласовата поща, **HostedVoicemail** трябва да е настроен на $true.

Свойството **HostedVoicemail** на потребителя чрез отдалечен PowerShell (RPS).

За повече информация относно свързването към RPS вж. Microsoft Teams общ преглед на [PowerShell](https://docs.microsoft.com/microsoftteams/teams-powershell-overview) за повече информация относно свързването към RPS.

1. Администраторът Teams трябва да е влязъл в Отдалечен PowerShell за Teams.
1. От powerShell подкани администраторът на Teams може да изпълнява **set-csuser user@contoso.com -HostedVoiceMail $true** където sip uri е на въпросния потребител.

**Забележка:** Промените в правилата могат да отнемат до 24 часа, за да се възпроизвеждат.