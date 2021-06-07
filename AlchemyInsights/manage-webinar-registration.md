---
title: Управление на регистрацията на уебинар
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 06/02/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "11512"
- "9006672"
ms.openlocfilehash: c5b0721d286b07d7e0f84199885b6f527a2b42a2
ms.sourcegitcommit: f7a9e97d04b7b6cbb633b32094d40f1874bf0fce
ms.translationtype: HT
ms.contentlocale: bg-BG
ms.lasthandoff: 06/06/2021
ms.locfileid: "52793566"
---
# <a name="manage-webinar-registration"></a>Управление на регистрацията на уебинар

Можете да управлявате кой може да се регистрира Teams уебинари с помощта на Teams команди на Powershell. За да инсталирате Teams Powershell, [вижте Teams PowerShell](/microsoftteams/teams-powershell-install). 

По подразбиране *WhoCanRegister е разрешен* и настроен на **EveryoneInCompany**. За да позволите на всеки, включително анонимни потребители, да се регистрира, трябва да зададете правилата за събрание на **всеки** с помощта на командата Powershell:

`Set-CsTeamsMeetingPolicy -WhoCanRegister Everyone`

**Забележка:** Ако анонимното присъединяване е изключено в настройките на събранието, анонимните потребители не могат да се присъединят към уебинари. За да научите повече и да разрешите тази настройка, вижте [Управление на настройките на събранието Microsoft Teams](/microsoftteams/meeting-settings-in-teams).

Ако искате да изключите регистрирането на събрание, *задайте AllowMeetingRegistration на* **False**.

За да научите повече за конфигурирането кой може да се регистрира за уебинари, вижте [Конфигуриране кой може да се регистрира за уебинари](/microsoftteams/set-up-webinars?source=docs#configure-who-can-register-for-webinars). За повече информация относно настройките за списъци на Microsoft вижте Управление [на настройките за списъци на Microsoft](/sharepoint/control-lists).
