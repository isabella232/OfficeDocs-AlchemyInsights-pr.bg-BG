---
title: Промяна на имейл адреса на група на Microsoft 365
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "1200024"
- "4704"
ms.openlocfilehash: f54ca5df09d0604f6d58c6c8a41dc907485e1f04
ms.sourcegitcommit: beb9715ac0c8e8333fef6764ecd346b7401a2612
ms.translationtype: MT
ms.contentlocale: bg-BG
ms.lasthandoff: 10/10/2020
ms.locfileid: "48461749"
---
# <a name="change-email-address-of-a-microsoft-365-group"></a>Промяна на имейл адреса на група на Microsoft 365

Можете да промените имейл адреса на група на Microsoft 365 с помощта на центъра за администриране. Просто изберете групата и изберете @edit имейл адрес.

Можете също да използвате командата "следване", за да промените основния SMTP адрес на група на Microsoft 365:

`Set-UnifiedGroup <Group Name> -PrimarySmtpAddress <new SMTP Address>`

Например

`et-UnifiedGroup Marketing -PrimarySmtpAddress marketing@contoso.com`
