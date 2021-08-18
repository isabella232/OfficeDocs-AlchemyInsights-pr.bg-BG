---
title: Група "Изпрати като Microsoft 365"
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 08/19/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9003200"
ms.openlocfilehash: 204b2c1777f76f11663b2735b784cbb56f1f1aba891628fb46ef37b501c9ff85
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: bg-BG
ms.lasthandoff: 08/05/2021
ms.locfileid: "54086117"
---
# <a name="send-as-microsoft-365-group"></a>Група "Изпрати като Microsoft 365"

Можете да дадете разрешения за изпращане като, за да позволите на определени потребители да изпращат съобщения като Microsoft 365 група:  

1. Свързване да Exchange Online PowerShell.  

2. Изпълнете следната команда:  

    Add-RecipientPermission `<GroupName>` -Trustee `<MailboxName>` -AccessRights SendAs

За повече информация вижте Разрешаване [на членовете да изпращат като или да изпращат от името на група](https://docs.microsoft.com/microsoft-365/admin/create-groups/allow-members-to-send-as-or-send-on-behalf-of-group?view=o365-worldwide).