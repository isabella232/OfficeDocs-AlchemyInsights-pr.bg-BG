---
title: Какво да направите, ако функциите на Azure не работят правилно в Microsoft Edge
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/26/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "8315"
- "9004429"
ms.openlocfilehash: 710489bd7dcb10f5c953c83e87bdad030c47cfda7dbd38e1eceae78bfe0d8790
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: bg-BG
ms.lasthandoff: 08/05/2021
ms.locfileid: "57812861"
---
# <a name="what-to-do-if-azure-features-dont-work-properly-in-microsoft-edge"></a>Какво да направите, ако функциите на Azure не работят правилно в Microsoft Edge

Microsoft Edge известни проблеми, свързани със зоните за защита, които може да повлияят на начина, по който потребителите на Azure в Windows за администриране. За повече информация вижте [Известни проблеми в Edge](https://go.microsoft.com/fwlink/?linkid=2140608). Ако имате проблеми с използването на функции на Azure с Microsoft Edge, опитайте следното:

1. В Меню , в лентата **за търсене** въведете **Опции за интернет** и след това го изберете.
1. В **Свойства на интернет** изберете **раздела** Защита.
1. Изберете **Надеждни сайтове** и след това изберете **Сайтове**.
1. Добавете URL адреса на вашия шлюз, <https://login.microsoftonline.com> както и , и изберете <https://login.live.com> **Затвори**.
1. В **Свойства на интернет** изберете раздела **Поверителност.**
1. В секцията Блокиране на изскачащи прозорци **изберете Настройки**. Добавете URL адреса на вашия шлюз, <https://login.microsoftonline.com> както и , и след това изберете <https://login.live.com> **Затвори**.