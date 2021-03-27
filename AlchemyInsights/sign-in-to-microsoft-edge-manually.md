---
title: Ръчно влизане в Microsoft Edge
ms.author: v-smandalika
author: v-smandalika
ms.date: 12/03/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 686e8f18-b871-4dd2-864f-8562947ab583
ms.collection: Adm_O365
ms.custom:
- "9003844"
- "6893"
- "8332"
- "9004625"
ms.openlocfilehash: f380d09dc14788205638cdee6aebe0b084ecab2f
ms.sourcegitcommit: 6bfe9cd9d0b18481e0cac6f1f5bc86ed7df31037
ms.translationtype: MT
ms.contentlocale: bg-BG
ms.lasthandoff: 03/27/2021
ms.locfileid: "51398646"
---
# <a name="sign-in-to-microsoft-edge-manually"></a>Ръчно влизане в Microsoft Edge

Ако потребителят не е влизал автоматично по време на първото изпълнение, потребителят може ръчно да влезете в настройките на браузъра или в менюто за самоличност. За да управлявате влизането, използвайте следните правила:

1. [NonRemovableProfileEnabled](https://docs.microsoft.com/deployedge/microsoft-edge-policies#nonremovableprofileenabled) – За да сте сигурни, че потребителят винаги има работен профил в Microsoft Edge.
2. [Ограничаване наSigninToPattern](https://docs.microsoft.com/deployedge/microsoft-edge-policies#restrictsignintopattern) – За да ограничите влизането до набор от надеждни акаунти.
3. [BrowserSignin](https://docs.microsoft.com/deployedge/microsoft-edge-policies#browsersignin) – За да забраните влизането или да накарате потребителите да впишат.

