---
title: Промяна на имейл адреса на група на Microsoft 365
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "1200024"
- "4704"
ms.openlocfilehash: 32968f085a4e9d49f60ef88e4e78bf6c67629556
ms.sourcegitcommit: f28dafa0f727870038f72bc904da926daf4ec07b
ms.translationtype: HT
ms.contentlocale: bg-BG
ms.lasthandoff: 06/05/2020
ms.locfileid: "44580646"
---
# <a name="change-email-address-of-a-microsoft-365-group"></a>Промяна на имейл адреса на група на Microsoft 365

Можете да промените имейл адреса на група на Microsoft 365 с помощта на центъра за администриране. Просто изберете групата и изберете @edit имейл адрес.

Можете да използвате и следната команда EXO PowerShell да промените основния SMTP адрес на група на Microsoft 365:

Групи за задаване <Group Name> – основен адрес<new SMTP Address>

Пример:

```
    Set-UnifiedGroup Marketing -PrimarySmtpAddress marketing@contoso.com
```
