---
title: Използване на Giphys Teams разговори
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
- "9003825"
- "6850"
ms.openlocfilehash: 296c2f80d35f1c93ab3c60e0be65fd96c953ca81
ms.sourcegitcommit: ab75f66355116e995b3cb5505465b31989339e28
ms.translationtype: MT
ms.contentlocale: bg-BG
ms.lasthandoff: 08/13/2021
ms.locfileid: "58323509"
---
# <a name="using-giphys-in-teams-conversations"></a>Използване на Giphys Teams разговори

Достъпът до Giphys Teams чат е разрешен по подразбиране. Като администратор можете да контролирате дали Giphys [](https://docs.microsoft.com/microsoftteams/messaging-policies-in-teams#messaging-policy-settings) е наличен за потребителите, като зададете правила за съобщения и гарантирате, че **Използването на Giphys в разговорите** е **На**.

Ако GIF файлове не работят по очаквания начин в Teams разговори, проверете:

Правилата [за съобщения трябва](https://docs.microsoft.com/microsoftteams/messaging-policies-in-teams) да позволяват Giphys. За да проверите с помощта на кратки команди на PowerShell:

- Уверете се, че можете [да управлявате Teams с PowerShell](https://docs.microsoft.com/microsoftteams/teams-powershell-overview?view=o365-worldwide#manage-teams-with-powershell).
- Изпълнете командата PowerShell [Get-CsTeamsMessagingPolicy -Identity Global](https://docs.microsoft.com/powershell/module/skype/get-csteamsmessagingpolicy?view=skype-ps) и проверете дали **AllowGiphy** е зададен на **TRUE.**
- Ако **AllowGiphy** е зададено на **FALSE**, изпълнете следната команда на PowerShell [Set-CsTeamsMessagingPolicy -Identity Global -AllowGiphy $True](https://docs.microsoft.com/powershell/module/skype/set-csteamsmessagingpolicy?view=skype-ps).

[Незадължителни свързани](https://docs.microsoft.com/deployoffice/privacy/optional-connected-experiences) изживявания трябва да бъдат разрешени, за да се разреши достъп до URL адреса на Giphy.

**Забележка:** Ако имате няколко правила за Teams съобщения, конфигурирани за вашия клиент, можете да определите самоличността на правилата, присвоени на засегнатия потребител с командата [Get-CsOnlineUser -Identity](https://docs.microsoft.com/powershell/module/skype/get-csonlineuser?view=skype-ps) <user@domain.com> | Изберете TeamsMessagingPolicy.
