---
title: Не можете да задавате или преглеждате правилата за AllowSelfServicePurchase
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9001212"
- "3526"
ms.openlocfilehash: 5ec16b3071f95ef52af2771e95137116222a3c5b
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: bg-BG
ms.lasthandoff: 09/14/2020
ms.locfileid: "47735188"
---
# <a name="unable-to-set-or-view-the-allowselfservicepurchase-policy"></a>Не можете да задавате или преглеждате правилата за AllowSelfServicePurchase

Когато се опитвате да зададете или видите правилата за AllowSelfServicePurchase, получавате следното съобщение за грешка:

*HandleError: неуспех при извличане на правилата за продукти с PolicyId "AllowSelfServicePurchase", ErrorMessage – основната връзка е затворена: неочаквана грешка при изпращане.*

Това може да се дължи на по-стара версия на защитата на транспортния слой (TLS). За да свържете услугата MSCommerce, трябва да използвате TLS 1,2 или по-нова версия.  

Изпробвайте следните стъпки, за да разрешите/зададете TLS протокола към 1,2, проверете и опитайте отново.
 1. В командния прозорец на PowerShell (PS C: \) Въведете следната команда, за да зададете ПРОТОКОЛА TLS към версия 1,2:

    `[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12`

2. Проверете използвания TLS протокол (и) със следната команда:

    `[Net.ServicePointManager]::SecurityProtocol` 

3. Опитайте отново с командите получаване или актуализиране, ако е необходимо.

