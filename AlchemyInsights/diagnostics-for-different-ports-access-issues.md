---
title: Диагностициране на проблеми с достъпа до различните портове
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
ms.openlocfilehash: 3673067cad7ac55f3820422dc2ec09942c393149
ms.sourcegitcommit: c08bed4071baa3bb5879496df3ed44fb828c8367
ms.translationtype: MT
ms.contentlocale: bg-BG
ms.lasthandoff: 03/19/2021
ms.locfileid: "51034874"
---
# <a name="diagnostics-for-different-ports-access-issues"></a>Диагностициране на проблеми с достъпа до различните портове

За да разрешите различните проблеми с достъпа до портовете, изпълнете следните стъпки:

1. Спрете/деразпределите виртуалната машина (VM) от портала, Рестартирайте VM и Изпробвайте отново. 
2. Проверете мрежовите настройки на вашата VM, за да определите дали имате блокиращи трафика групи за мрежова защита (NSGs). Можете също да използвате [инструмента за проверка на IP Flow за наблюдение на мрежата](https://docs.microsoft.com/azure/network-watcher/network-watcher-ip-flow-verify-overview?WT.mc_id=Portal-Microsoft_Azure_Support) , за да проверите за блокиран трафик на NSGs, User-Defined маршрути (UDRs) пренасочване на трафика ви обратно към локален ("маршрут по подразбиране" 0.0.0.0/0) или към мрежово устройство.
Ако все още имате проблеми, след като сте изпробвали стъпките по-горе, моля, въведете името на VM и TCP порта, към който се опитвате да изпратите поща, за да направите по-нататъшни диагнози.

**Препоръчителни документи**

[Ограничения и препоръки за изпращане на изходящи имейли през порт 25](https://docs.microsoft.com/azure/virtual-network/troubleshoot-outbound-smtp-connectivity)