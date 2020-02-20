---
title: Не може да се зададе или да се визуализира правилата на AllowSelfServicePurchase
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9001212"
- "3526"
ms.openlocfilehash: 587a05cccbc71a970d4bd7723bff0df0c3b64ccc
ms.sourcegitcommit: 2a9d059262c07c33f9a740b3da4e6e3366b2f925
ms.translationtype: MT
ms.contentlocale: bg-BG
ms.lasthandoff: 02/20/2020
ms.locfileid: "42158548"
---
# <a name="unable-to-set-or-view-the-allowselfservicepurchase-policy"></a>Не може да се зададе или да се визуализира правилата на AllowSelfServicePurchase

При опит за задаване или преглед на AllowSelfServicePurchase политика, получавате следното съобщение за грешка:

*HandleError: Неуспешно извличане на продуктови правила с PolicyId "AllowSelfServicePurchase", съобщение за грешка - основната връзка е прекъсната: възникна неочаквана грешка при изпращане.*

Това може да се дължи на по-стара версия на защита на транспортния слой (TLS). За да свържете MSCommerce услугата, трябва да използвате TLS 1.2 или по-нова версия.  

Опитайте следните стъпки, за да разрешите/зададете TLS протокола 1.2, проверете и опитайте отново.
 1. В командния ред на PowerShell\) (PS C: въведете следната команда, за да зададете протокола TLS версия 1.2:

    `[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12`

2. Проверете TLS протокола, които се използват, със следната команда:

    `[Net.ServicePointManager]::SecurityProtocol` 

3. Опитайте отново да получите или актуализирате командите, ако е необходимо.

