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
# <a name="diagnostics-for-different-ports-access-issues"></a><span data-ttu-id="e817b-102">Диагностициране на проблеми с достъпа до различните портове</span><span class="sxs-lookup"><span data-stu-id="e817b-102">Diagnostics for different ports access issues</span></span>

<span data-ttu-id="e817b-103">За да разрешите различните проблеми с достъпа до портовете, изпълнете следните стъпки:</span><span class="sxs-lookup"><span data-stu-id="e817b-103">To resolve the different port access issues, perform the following steps:</span></span>

1. <span data-ttu-id="e817b-104">Спрете/деразпределите виртуалната машина (VM) от портала, Рестартирайте VM и Изпробвайте отново.</span><span class="sxs-lookup"><span data-stu-id="e817b-104">Stop/deallocate the virtual machine (VM) from the portal, restart the VM, and test again.</span></span> 
2. <span data-ttu-id="e817b-105">Проверете мрежовите настройки на вашата VM, за да определите дали имате блокиращи трафика групи за мрежова защита (NSGs).</span><span class="sxs-lookup"><span data-stu-id="e817b-105">Check your VM's network settings to determine if you have Network Security Groups (NSGs) blocking traffic.</span></span> <span data-ttu-id="e817b-106">Можете също да използвате [инструмента за проверка на IP Flow за наблюдение на мрежата](https://docs.microsoft.com/azure/network-watcher/network-watcher-ip-flow-verify-overview?WT.mc_id=Portal-Microsoft_Azure_Support) , за да проверите за блокиран трафик на NSGs, User-Defined маршрути (UDRs) пренасочване на трафика ви обратно към локален ("маршрут по подразбиране" 0.0.0.0/0) или към мрежово устройство.</span><span class="sxs-lookup"><span data-stu-id="e817b-106">You can also use [Network Watcher's IP flow verify tool](https://docs.microsoft.com/azure/network-watcher/network-watcher-ip-flow-verify-overview?WT.mc_id=Portal-Microsoft_Azure_Support) to check for NSGs blocking traffic, User-Defined Routes (UDRs) rerouting your traffic back to on-premises ('Default Route' 0.0.0.0/0), or to a network appliance.</span></span>
<span data-ttu-id="e817b-107">Ако все още имате проблеми, след като сте изпробвали стъпките по-горе, моля, въведете името на VM и TCP порта, към който се опитвате да изпратите поща, за да направите по-нататъшни диагнози.</span><span class="sxs-lookup"><span data-stu-id="e817b-107">If you still experience issues after trying the steps above, please provide the VM name and the TCP port you are attempting to send mail on for further diagnosis.</span></span>

<span data-ttu-id="e817b-108">**Препоръчителни документи**</span><span class="sxs-lookup"><span data-stu-id="e817b-108">**Recommended Documents**</span></span>

[<span data-ttu-id="e817b-109">Ограничения и препоръки за изпращане на изходящи имейли през порт 25</span><span class="sxs-lookup"><span data-stu-id="e817b-109">Limitations and recommendations for sending outbound email over port 25</span></span>](https://docs.microsoft.com/azure/virtual-network/troubleshoot-outbound-smtp-connectivity)