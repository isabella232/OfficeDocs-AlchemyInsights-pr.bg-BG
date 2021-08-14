---
title: Промяна на имейл адреса на Microsoft 365 група
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
ms.openlocfilehash: 6bd9301b983d09f6a0058fee17577b9fc695458ed205f96aacf79a87e4a91e34
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: bg-BG
ms.lasthandoff: 08/05/2021
ms.locfileid: "53930718"
---
# <a name="change-email-address-of-a-microsoft-365-group"></a>Промяна на имейл адреса на Microsoft 365 група

Можете да промените имейл адреса на група Microsoft 365, като използвате центъра за администриране. Просто изберете групата и изберете @редактиране на имейл адрес.

Можете също да използвате командата EXO PowerShell, за да промените основния SMTP адрес на Microsoft 365 група:

Set-UnifiedGroup <Group Name> -PrimarySmtpAddress <new SMTP Address>

Пример:

```
    Set-UnifiedGroup Marketing -PrimarySmtpAddress marketing@contoso.com
```
