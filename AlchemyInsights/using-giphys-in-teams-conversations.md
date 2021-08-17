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
ms.openlocfilehash: 0244b68ffa2ebd3d70bae66a24ac299004848557b63b17c2ea74fafaff22bb8c
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: bg-BG
ms.lasthandoff: 08/05/2021
ms.locfileid: "54104297"
---
# <a name="using-giphys-in-teams-conversations"></a>Използване на Giphys Teams разговори

Достъпът до Giphys в Teams чат е разрешен по подразбиране. Като администратор можете да контролирате дали Giphys [](https://docs.microsoft.com/microsoftteams/messaging-policies-in-teams#messaging-policy-settings) е наличен за потребителите, като зададете правила за съобщения и гарантирате, че **Използването на Giphys в разговорите** е **На**.

Ако GIF файлове не работят по очаквания начин в Teams разговори, проверете:

Правилата [за съобщения трябва](https://docs.microsoft.com/microsoftteams/messaging-policies-in-teams) да позволяват Giphys. За да проверите с помощта на кратки команди на PowerShell:

- Уверете се, че можете [да управлявате Teams с PowerShell](https://docs.microsoft.com/microsoftteams/teams-powershell-overview?view=o365-worldwide#manage-teams-with-powershell).
- Изпълнете командата PowerShell [Get-CsTeamsMessagingPolicy -Identity Global](https://docs.microsoft.com/powershell/module/skype/get-csteamsmessagingpolicy?view=skype-ps) и проверете дали **AllowGiphy** е зададен на **TRUE.**
- Ако **AllowGiphy** е зададено на **FALSE**, изпълнете следната команда на PowerShell [Set-CsTeamsMessagingPolicy -Identity Global -AllowGiphy $True](https://docs.microsoft.com/powershell/module/skype/set-csteamsmessagingpolicy?view=skype-ps).

[Незадължителни свързани](https://docs.microsoft.com/deployoffice/privacy/optional-connected-experiences) изживявания трябва да бъдат разрешени, за да се разреши достъп до URL адреса на Giphy.

> [!NOTE]
> Ако имате няколко правила за Teams съобщения, конфигурирани за вашия клиент, можете да определите самоличността на правилата, присвоени на засегнатия потребител, с командата [Get-CsOnlineUser -Identity](https://docs.microsoft.com/powershell/module/skype/get-csonlineuser?view=skype-ps) <user@domain.com> | Изберете TeamsMessagingPolicy.
