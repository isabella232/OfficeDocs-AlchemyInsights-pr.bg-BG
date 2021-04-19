---
title: Устройства за конфигуриране на диспечера липсват в портала
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
- "9001495"
- "4384"
ms.openlocfilehash: d57659eb928dd8c4653499e65b6e6cd2f021f521
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: bg-BG
ms.lasthandoff: 04/15/2021
ms.locfileid: "51817233"
---
# <a name="configuration-manager-devices-missing-in-the-portal"></a><span data-ttu-id="2cdc8-102">Устройства за конфигуриране на диспечера липсват в портала</span><span class="sxs-lookup"><span data-stu-id="2cdc8-102">Configuration Manager devices missing in the portal</span></span>

<span data-ttu-id="2cdc8-103">За да работи синхронизирането на устройства, [необходимите крайни точки за интернет](https://docs.microsoft.com/configmgr/tenant-attach/device-sync-actions#internet-endpoints) трябва да са достъпни от локалния сървър, който хоства ролята на точка на свързване на услугата.</span><span class="sxs-lookup"><span data-stu-id="2cdc8-103">For device sync to work, [required internet endpoints](https://docs.microsoft.com/configmgr/tenant-attach/device-sync-actions#internet-endpoints) must be reachable from the on-premise server hosting the Service Connection Point role.</span></span> <span data-ttu-id="2cdc8-104">За да отстраните неизправности в синхронизирането на устройствата, прегледайте **CMGatewaySyncUploadWorker.log**, намиращ се в точката за свързване на услугата.</span><span class="sxs-lookup"><span data-stu-id="2cdc8-104">To troubleshoot device sync, please review the **CMGatewaySyncUploadWorker.log** located on the service connection point.</span></span>

<span data-ttu-id="2cdc8-105">Научете повече за [Прикачването на клиент в Microsoft Endpoint Manager ](https://docs.microsoft.com/configmgr/tenant-attach/).</span><span class="sxs-lookup"><span data-stu-id="2cdc8-105">Learn more about [Tenant attach in Microsoft Endpoint Manager](https://docs.microsoft.com/configmgr/tenant-attach/).</span></span>
