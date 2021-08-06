---
title: Правилата allowSelfServicePurchase не могат да се задават или преглеждат
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9001212"
- "3526"
ms.openlocfilehash: 255dbe35b808b3fe6b5707779251bf3f4a7e1c269c8b6f0ac2cb43ca03c469e9
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: bg-BG
ms.lasthandoff: 08/05/2021
ms.locfileid: "54020181"
---
# <a name="unable-to-set-or-view-the-allowselfservicepurchase-policy"></a>Правилата allowSelfServicePurchase не могат да се задават или преглеждат

Когато се опитвате да зададете или прегледате правилата allowSelfServicePurchase, получавате следното съобщение за грешка:

*МанипулаторError: Неуспешно извличане на продуктови правила с PolicyId "AllowSelfServicePurchase", ErrorMessage – базовата връзка е затворена: Възникна неочаквана грешка при изпращане.*

Това може да се дължи на по-стара версия на защитата на транспортния слой (TLS). За да свържете услугата MSCommerce, трябва да използвате TLS 1.2 или по-нова версия.  

Опитайте следните стъпки, за да разрешите/зададете TLS протокола на 1.2, проверете и опитайте отново.
 1. В командния прозорец на PowerShell (PS C: \) въведете следната команда, за да зададете TLS протокола на версия 1.2:

    `[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12`

2. Проверете използвания(те) TLS протокол(и) със следната команда:

    `[Net.ServicePointManager]::SecurityProtocol` 

3. Опитайте отново командите Получаване или Актуализиране, ако е необходимо.

