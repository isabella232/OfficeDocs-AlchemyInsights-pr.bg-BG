---
title: Диагностика за различни проблеми с достъпа до портове
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 03/19/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9035"
- "9005220"
ms.openlocfilehash: 07c108d5292965d20340da039b67744d93c0a4fc61edb8115796671f2f7f1552
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: HT
ms.contentlocale: bg-BG
ms.lasthandoff: 08/05/2021
ms.locfileid: "54030891"
---
# <a name="diagnostics-for-different-ports-access-issues"></a>Диагностика за различни проблеми с достъпа до портове

За да отстраните различните проблеми с достъпа до порт, изпълнете следните стъпки:

1. Спрете/разпределете виртуалната машина (VM) от портала, рестартирайте VM и тествайте отново. 
2. Проверете мрежовите настройки на вашата VM, за да определите дали имате блокиране на трафика на групите за защита на мрежата (NSGs). Можете също да използвате инструмента за проверка на IP потока на Network [Watcher,](https://docs.microsoft.com/azure/network-watcher/network-watcher-ip-flow-verify-overview?WT.mc_id=Portal-Microsoft_Azure_Support) за да проверите за NSGs, блокиращи трафика, User-Defined Маршрути (UDRs), които пренасочите трафика обратно към локалния (0.0.0.0/0 маршрут по подразбиране маршрут) или към мрежов уред.
Ако все още имате проблеми, след като сте опитали стъпките по-горе, посочете името на VM и TCP порта, на който се опитвате да изпратите поща за по-нататъшно диагностициране.

**Препоръчителни документи**

[Ограничения и препоръки за изпращане на изходящ имейл през порт 25](https://docs.microsoft.com/azure/virtual-network/troubleshoot-outbound-smtp-connectivity)