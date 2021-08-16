---
title: Включване на NDI технологията
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
ms.openlocfilehash: ed932592aae1158bc0c0da4817467b69d20208533bc080cb0e424f552af8601a
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: bg-BG
ms.lasthandoff: 08/05/2021
ms.locfileid: "54023511"
---
# <a name="turn-on-ndi-technology"></a>Включване на NDI технологията

Технологията NDI изисква две стъпки да бъдат включени за потребител:

1. Администраторът на клиента трябва да разреши свойството "AllowNDIStreaming" в CsTeamsMeetingPolicy.

    `Set-CsTeamsMeetingPolicy -Identity MEETING_POLICY -AllowNDIStreaming $true`

2. След като тази промяна е попълнена, крайният потребител трябва да включи NDI® технология за своя конкретен **клиент от Настройки > разрешения**.

За повече информация вижте [Използване на NDI технология в Microsoft Teams.](https://docs.microsoft.com/microsoftteams/use-ndi-in-meetings)
