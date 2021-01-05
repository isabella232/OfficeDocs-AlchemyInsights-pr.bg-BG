---
title: Промяна на имейл адреса на група на Microsoft 365 или Microsoft Teams
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
ms.openlocfilehash: ff7abaf3d8e0ed977eba5712bdd19185738fa75c
ms.sourcegitcommit: 8be59778b7d39213a27a471802eae7fc006eb1ff
ms.translationtype: HT
ms.contentlocale: bg-BG
ms.lasthandoff: 01/05/2021
ms.locfileid: "49756546"
---
# <a name="change-email-address-of-a-microsoft-365-group-or-microsoft-teams"></a>Промяна на имейл адреса на група на Microsoft 365 или Microsoft Teams

Можете да промените имейл адреса на група на Microsoft 365 или на Microsoft Teams, като използвате [Център за администриране на Microsoft 365](https://admin.microsoft.com/). Просто изберете групата и изберете @редактиране на имейл адрес.

Можете също да използвате следната EXO PowerShell команда за промяна на основния SMTP адрес на група на Microsoft 365/Teams:

`Set-UnifiedGroup <Group Name> -PrimarySmtpAddress <new SMTP Address>`

Пример:

`Set-UnifiedGroup Marketing -PrimarySmtpAddress marketing@contoso.com`
