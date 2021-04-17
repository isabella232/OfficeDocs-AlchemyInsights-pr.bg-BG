---
title: Промяна на имейл адреса на група на Microsoft 365
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "1200024"
- "4704"
ms.openlocfilehash: 8eaafae8650a8072cdfbec281afe6d5e93fea655
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: bg-BG
ms.lasthandoff: 04/15/2021
ms.locfileid: "51819033"
---
# <a name="change-email-address-of-a-microsoft-365-group"></a>Промяна на имейл адреса на група на Microsoft 365

Можете да промените имейл адреса на група на Microsoft 365 с помощта на центъра за администриране. Просто изберете групата и изберете @редактиране на имейл адрес.

Можете също да използвате командата EXO PowerShell, за да промените основния SMTP адрес на група на Microsoft 365:

Set-UnifiedGroup <Group Name> -PrimarySmtpAddress <new SMTP Address>

Пример:

```
    Set-UnifiedGroup Marketing -PrimarySmtpAddress marketing@contoso.com
```
