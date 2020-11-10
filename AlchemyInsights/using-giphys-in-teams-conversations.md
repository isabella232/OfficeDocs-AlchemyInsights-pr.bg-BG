---
title: Използване на Гифчета в разговорите в Teams
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
ms.openlocfilehash: 2fc29974bff9484c226c9651b9b000a89cad14dc
ms.sourcegitcommit: 534e9217d99336eb471166ff83231c7e408fb1d9
ms.translationtype: MT
ms.contentlocale: bg-BG
ms.lasthandoff: 11/09/2020
ms.locfileid: "48982425"
---
# <a name="using-giphys-in-teams-conversations"></a>Използване на Гифчета в разговорите в Teams

Достъпът до гифчета в чата на Teams е разрешен по подразбиране. Като администратор можете да управлявате дали Гифчета са достъпни за потребителите чрез [Задаване на правила за съобщения](https://docs.microsoft.com/microsoftteams/messaging-policies-in-teams#messaging-policy-settings) и гарантиране, че **използването на гифчета в разговорите** е **включено**.

Ако GIF файловете не работят по очаквания начин в разговорите в Teams, проверете следното:

[Правилата за съобщения](https://docs.microsoft.com/microsoftteams/messaging-policies-in-teams) трябва да позволяват на гифчета. За да проверите с помощта на кратки команди на PowerShell:

- Проверете дали можете да [управлявате Teams с PowerShell](https://docs.microsoft.com/microsoftteams/teams-powershell-overview?view=o365-worldwide#manage-teams-with-powershell).
- Изпълнете командата PowerShell [get-CsTeamsMessagingPolicy-Identity Global](https://docs.microsoft.com/powershell/module/skype/get-csteamsmessagingpolicy?view=skype-ps) и проверете дали **AllowGiphy** е зададено на **TRUE**.
- Ако " **AllowGiphy** " е зададено на **FALSE** , изпълнете следния команден набор на PowerShell [– CsTeamsMessagingPolicy-AllowGiphy $True](https://docs.microsoft.com/powershell/module/skype/set-csteamsmessagingpolicy?view=skype-ps).

[Опционалните свързани преживявания](https://docs.microsoft.com/deployoffice/privacy/optional-connected-experiences) трябва да са разрешени за разрешаване на достъпа до URL адреса на Giphy.

> [!NOTE]
> Ако имате няколко правила за съобщения, конфигурирани за вашия клиент, можете да определите самоличността на правилата, присвоени на засегнатия потребител, с помощта на командата PowerShell [get-CsOnlineUser-самоличност](https://docs.microsoft.com/powershell/module/skype/get-csonlineuser?view=skype-ps) <user@domain.com> | Изберете TeamsMessagingPolicy.
