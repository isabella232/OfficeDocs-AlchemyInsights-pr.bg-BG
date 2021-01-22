---
title: Включване на технология НДИ
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
- "9004403"
- "7947"
ms.openlocfilehash: ea694898baffa50fca71957175eba3664dece44e
ms.sourcegitcommit: 112f18dce8257b98fab32d44910ee879efb44cb8
ms.translationtype: MT
ms.contentlocale: bg-BG
ms.lasthandoff: 01/21/2021
ms.locfileid: "49935074"
---
# <a name="turn-on-ndi-technology"></a>Включване на технология НДИ

НДИ технология изисква две стъпки, които трябва да бъдат включвани за потребител:

1. Администраторът на клиент трябва да разреши свойството "AllowNDIStreaming" в CsTeamsMeetingPolicy.

    `Set-CsTeamsMeetingPolicy -Identity MEETING_POLICY -AllowNDIStreaming $true`

2. След като тази промяна бъде запълнена, крайният потребител трябва да включи НДИ® технология за своя конкретен клиент от **настройките > разрешения**.

За повече информация вижте [използване на технология на НДИ в Microsoft Teams](https://docs.microsoft.com/microsoftteams/use-ndi-in-meetings).
