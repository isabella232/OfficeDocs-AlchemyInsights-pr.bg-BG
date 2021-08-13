---
title: Teams не се стартира
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 08/4/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "12673"
- "9007646"
ms.openlocfilehash: a37f980e700090da8199c703216af6f04f4aca464c21870beb3e907dd7b2d491
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: HT
ms.contentlocale: bg-BG
ms.lasthandoff: 08/05/2021
ms.locfileid: "57813341"
---
# <a name="teams-doesnt-launch"></a>Teams не се стартира

Ако се опитате да отворите Microsoft Teams, но той никога не се стартира, опитайте следното:

1. Отидете на **%appdata%\Microsoft\Teams**.
1. Изтрийте съдържанието на папката.
1. Рестартирайте компютъра и се опитайте да стартирате Teams.

Може да се наложи да преинсталирате Teams. За да преинсталирате:

1. Деинсталирайте Teams с помощта на контролния панел.
1. Отидете на **%appdata%\Microsoft\Teams\Application Cache**.
1. Изтрийте съдържанието на папката.
1. Отидете на **%appdata%\Microsoft\teams\Cache**.
1. Изтрийте съдържанието на папката.
1. Рестартирайте компютъра и след това изтеглете и инсталирайте Teams.

Ако искате да изпълните диагностика на вашия клиент за конкретен потребител, който не може да влиза, започнете ново търсене с ключовата дума **TeamsUserUnableToSignIn** и следвайте подканите.