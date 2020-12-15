---
title: Как се разрешава хоствана гласова поща
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
ms.openlocfilehash: 26eb22054d246a6ca5a2491c68a5d9e4ed90d45b
ms.sourcegitcommit: 523098560e54a50184a99c974809dfbfffadacb5
ms.translationtype: MT
ms.contentlocale: bg-BG
ms.lasthandoff: 12/09/2020
ms.locfileid: "49676862"
---
# <a name="how-to-enable-hosted-voicemail"></a>Как се разрешава хоствана гласова поща

За да разрешите гласовата поща, **HostedVoicemail** трябва да бъде настроено на $True.

Свойството **HostedVoicemail** на потребителя чрез отдалечен POWERSHELL (RPS).

За повече информация относно свързването с RPS вижте [общ преглед на Microsoft Teams PowerShell](https://docs.microsoft.com/microsoftteams/teams-powershell-overview) за повече информация относно свързването с RPS.

1. Администраторът на Teams трябва да бъде влязъл в отдалечен PowerShell за Teams.
1. От PowerShell подкана администраторът на Teams може да изпълни **Set-csuser user@contoso.com-HostedVoiceMail $True** , където SIP URI е от въпросния потребител.

> [!NOTE]
> Промените в правилата могат да са необходими до 24 часа, за да се копират.