---
title: Какво да направите, ако функциите на Azure не работят правилно в Microsoft Edge
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
- "9004128"
- "7206"
ms.openlocfilehash: 463236bcd9ff480471604c992aa1ed1ed4ac2987
ms.sourcegitcommit: 2e4a5153e530bf15744a52e982eeb0d99757e9d2
ms.translationtype: MT
ms.contentlocale: bg-BG
ms.lasthandoff: 12/04/2020
ms.locfileid: "49583189"
---
# <a name="what-to-do-if-azure-features-dont-work-properly-in-microsoft-edge"></a>Какво да направите, ако функциите на Azure не работят правилно в Microsoft Edge

Microsoft Edge има [известни проблеми](https://go.microsoft.com/fwlink/?linkid=2140608) , които са свързани със зоните за защита, и може да засегне как потребителите на Azure влизат в центъра за администриране на Windows. Ако имате проблеми с използването на функциите на Azure с Microsoft Edge, изпробвайте следните стъпки:

1. В менюто **Старт** Потърсете **Опции за интернет** и го изберете.
2. В диалоговия прозорец **свойства на интернет** отидете на раздела **защита** .
3. Изберете зоната **надеждни сайтове** и след това изберете бутона **сайтове** .
4. В диалоговия прозорец **надеждни сайтове** Добавете URL адреса на шлюза, както [https://login.microsoftonline.com](https://login.microsoftonline.com) и и [https://login.live.com](https://login.live.com) след това изберете **Затвори**.
5. В диалоговия прозорец **свойства на интернет** отидете на раздела **поверителност** .
6. В секцията за **блокиране на изскачащи** съобщения изберете **Настройки**. В диалоговия прозорец, който се отваря, добавете URL адреса на шлюза, както [https://login.microsoftonline.com](https://login.microsoftonline.com) и и [https://login.live.com](https://login.live.com) след това изберете **Затвори**.
