---
title: AggregateGroupMailbox пълен NDR, получен за имейл, изпратен до Microsoft 365 група
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
ms.openlocfilehash: ace8e256e3771f82512abcb9e20b832381eedf80
ms.sourcegitcommit: ab75f66355116e995b3cb5505465b31989339e28
ms.translationtype: MT
ms.contentlocale: bg-BG
ms.lasthandoff: 08/13/2021
ms.locfileid: "58315899"
---
# <a name="aggregategroupmailbox-full-ndr-received-for-email-sent-to-microsoft-365-group"></a>AggregateGroupMailbox пълен NDR, получен за имейл, изпратен до Microsoft 365 група

Използвайте следната команда EXO Shell, за да създадете транспортно Exchange правило за тихо пускане на имейли, изпратени до агрегирани пощенски кутии на групи:

`New-TransportRule -SentTo @("AggregateGroupMailbox.A.201708181918@contoso.onmicrosoft.com") -DeleteMessage:$true -Name 'Agg1' -StopRuleProcessing:$false -Mode 'Enforce' -Comments '' -RuleErrorAction 'Ignore' -SenderAddressLocation 'Header'`

**Забележка:** Заместете SMTP адреса в **-SentTo** с SMTP адреса на пощенската кутия на агрегатната група във вашия клиент. Можете да получите SMTP адреса на пощенската кутия на агрегатната група от получената NDR.



