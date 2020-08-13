---
title: Личен канал
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9001223"
- "3205"
ms.openlocfilehash: be518df0d40123c1f0da6596bd6e2e91a0c2c8fa
ms.sourcegitcommit: 057d87c9d866fa1371d02350420d13774545c028
ms.translationtype: MT
ms.contentlocale: bg-BG
ms.lasthandoff: 05/02/2020
ms.locfileid: "44005427"
---
# <a name="private-channels-in-microsoft-teams"></a>Лични канали в Microsoft Teams

Частните канали са нова функция в Microsoft Teams. Имайте предвид, че частните канали не могат да бъдат конвертирани от стандартни канали, нито обратно.

За подробности относно поверителните канали, като например информация за [създаването на частни канали и за членството](https://docs.microsoft.com/MicrosoftTeams/private-channels#private-channel-creation-and-membership) и [частния канал на SharePoint](https://docs.microsoft.com/MicrosoftTeams/private-channels#private-channel-sharepoint-sites), вижте [лични канали в Microsoft Teams](https://docs.microsoft.com/MicrosoftTeams/private-channels). 

**Забележка:** Тъй като конфигурацията за запазване на съобщения в частния канал все още не се поддържа, за клиенти с разрешени правила за съхранение няма да има разрешени частни канали по подразбиране. Частните канали могат да бъдат разрешени в центъра за администриране на Teams. Също така имайте предвид, че докато запазването на съобщенията в частния канал не се поддържа, се поддържа съхранение на файлове, споделени в частни канали.

**Нуждаете се от нов собственик на екип?**

Ако вашият личен собственик на канал ви оставя, можете да добавите нов собственик на екип чрез Teams PowerShell.


- Отидете [тук](https://www.powershellgallery.com/packages/MicrosoftTeams/1.0.6) , за да инсталирате Teams PowerShell.

Ето кратката команда, която ще ви трябва:

`
    Add-TeamChannelUser -GroupId <group_id> -DisplayName "<channel_name>" -User <UPN> -Role Owner
`

За повече информация относно Teams PowerShell вижте [общ преглед на Teams PowerShell](https://docs.microsoft.com/microsoftteams/teams-powershell-overview).
