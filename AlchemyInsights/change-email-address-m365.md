---
title: Промяна на имейл адреса на група на Microsoft 365 или Microsoft Teams
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
ms.openlocfilehash: acb343553bfb7e100c03d0e7046ed5cbdd6b739b9a61e3faf17768bd8aadff34
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: bg-BG
ms.lasthandoff: 08/05/2021
ms.locfileid: "53995611"
---
# <a name="change-email-address-of-a-microsoft-365-group-or-microsoft-teams"></a>Промяна на имейл адреса на група на Microsoft 365 или Microsoft Teams

Можете да промените имейл адреса на група на Microsoft 365 или на Microsoft Teams, като използвате [Център за администриране на Microsoft 365](https://admin.microsoft.com/). Просто изберете групата и изберете @редактиране на имейл адрес.

Можете също да използвате следната EXO PowerShell команда за промяна на основния SMTP адрес на група на Microsoft 365/Teams:

`Set-UnifiedGroup <Group Name> -PrimarySmtpAddress <new SMTP Address>`

Пример:

`Set-UnifiedGroup Marketing -PrimarySmtpAddress marketing@contoso.com`
