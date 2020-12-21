---
title: AggregateGroupMailbox пълен NDR, получени за имейли, изпратени до Microsoft 365 Group
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 12/18/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004286"
- "7656"
ms.openlocfilehash: 9de09ab4cbd2f09648305b11da6273ed990907cf
ms.sourcegitcommit: 2ffdf6096de5608b117c6677d3cd7dd4c23ea024
ms.translationtype: MT
ms.contentlocale: bg-BG
ms.lasthandoff: 12/18/2020
ms.locfileid: "49721759"
---
# <a name="aggregategroupmailbox-full-ndr-received-for-email-sent-to-microsoft-365-group"></a>AggregateGroupMailbox пълен NDR, получени за имейли, изпратени до Microsoft 365 Group

Използвайте командата по-долу, за да създадете транспортно правило на Exchange, за да пуснете тихо имейли, изпратени до сборна пощенска кутия на Група:

`New-TransportRule -SentTo @("AggregateGroupMailbox.A.201708181918@contoso.onmicrosoft.com") -DeleteMessage:$true -Name 'Agg1' -StopRuleProcessing:$false -Mode 'Enforce' -Comments '' -RuleErrorAction 'Ignore' -SenderAddressLocation 'Header'`

> [!NOTE]
> Заместете SMTP адреса **SentTo** с SMTP адрес на сборна пощенска кутия на групата във вашия клиент. Можете да получите SMTP адреса на сборната пощенска кутия на групата от получените NDR.



