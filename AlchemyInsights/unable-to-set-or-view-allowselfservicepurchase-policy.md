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
ms.openlocfilehash: a9b6e36e8034e71b3e72c49e3cc68a126ef97aca
ms.sourcegitcommit: cb9505f9eca032af3a4194c68d18c91789365690
ms.translationtype: MT
ms.contentlocale: bg-BG
ms.lasthandoff: 02/16/2020
ms.locfileid: "42091662"
---
# <a name="unable-to-set-or-view-the-allowselfservicepurchase-policy"></a>Не може да се зададе или да се визуализира правилата на AllowSelfServicePurchase

При опит за задаване или преглед на AllowSelfServicePurchase политика, получавате следното съобщение за грешка:

*HandleError: Неуспешно извличане на продуктови правила с PolicyId "AllowSelfServicePurchase", съобщение за грешка - основната връзка е прекъсната: възникна неочаквана грешка при изпращане.*

Това може да се дължи на по-стара версия на защита на транспортния слой (TLS). За да свържете MSCommerce услугата, трябва да използвате TLS 1.2 или по-нова версия.  

Опитайте следните стъпки, за да разрешите/зададете TLS протокола 1.2, проверете и опитайте отново.
 1. В командния ред на PowerShell\) (PS C: въведете следната команда, за да зададете протокола TLS версия 1.2:

    \[Net.ServicePointManager]::ЗащитаПротокол \[= Net. ЗащитаТип протокол]:Tls12

2. Проверете TLS протокола, които се използват, със следната команда:

    \[Протокол за защита на мрежовите точки на обслужване 

3. Опитайте отново да получите или актуализирате командите, ако е необходимо.

