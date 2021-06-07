---
title: Разрешаване Teams уебинари
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
- "11513"
- "9006672"
ms.openlocfilehash: 5a732e6746e9fd23e54a0b2ffeabb59623012a0e
ms.sourcegitcommit: 9de78b30602f917d58705057cdcce31fec349969
ms.translationtype: MT
ms.contentlocale: bg-BG
ms.lasthandoff: 06/04/2021
ms.locfileid: "52793532"
---
# <a name="enable-teams-webinars"></a>Разрешаване Teams уебинари

Уебинарите са разрешени по подразбиране. Можете да управлявате кой може да планира и да се регистрира за Teams уебинари, като използвате Teams команди на PowerShell.

- Всички потребители, които могат да създадат събрание, също могат да създадат събрание на уебинар. Ако искате да управлявате кой може да планира Teams уебинари, използвайте *AllowMeetingRegistration*. 
- По подразбиране *WhoCanRegister е* разрешен и зададен на **Всеки**. Ако искате да изключите регистрирането на събрание, *задайте AllowMeetingRegistration на* **False**.

За да промените тези настройки, трябва да [инсталирате Teams PowerShell](/microsoftteams/teams-powershell-install). Освен това правилата за събранията се прилагат Teams уебинари. Ако например анонимното присъединяване е изключено в настройките на събранието, анонимните потребители не могат да се присъединят към уебинари.

За да научите повече за конфигурирането кой може да се регистрира за уебинари, вижте [Конфигуриране кой може да се регистрира за уебинари](/microsoftteams/set-up-webinars?source=docs#configure-who-can-register-for-webinars). За повече информация относно настройките за списъци на Microsoft вижте Управление [на настройките за списъци на Microsoft](/sharepoint/control-lists).