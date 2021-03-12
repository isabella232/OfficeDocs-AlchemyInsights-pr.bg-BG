---
title: Конфигуриране и проверка на изключвания за MDATP на компютър с Линукс
ms.author: v-jmathew
author: v-jmathew
manager: dansimp
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000760"
- "7391"
ms.openlocfilehash: 4fad0a513f7c6d2f0337019488a4055c25e1650d
ms.sourcegitcommit: 6312ee31561db36104f32282d019d069ede69174
ms.translationtype: MT
ms.contentlocale: bg-BG
ms.lasthandoff: 03/11/2021
ms.locfileid: "50743351"
---
# <a name="configure-and-validate-exclusions-for-mdatp-on-a-linux-machine"></a><span data-ttu-id="e7d72-102">Конфигуриране и проверка на изключвания за MDATP на компютър с Линукс</span><span class="sxs-lookup"><span data-stu-id="e7d72-102">Configure and validate exclusions for MDATP on a Linux machine</span></span>

<span data-ttu-id="e7d72-103">Можете да изключвате определени файлове, папки, процеси и файлове, отворени чрез процеси, от сканирането на MDATP.</span><span class="sxs-lookup"><span data-stu-id="e7d72-103">You can exclude certain files, folders, processes, and process-opened files from MDATP scans.</span></span> <span data-ttu-id="e7d72-104">Изключенията помагат за предотвратяване на неправилното откриване на софтуер и файлове, които са уникални или персонализирани за вашата организация.</span><span class="sxs-lookup"><span data-stu-id="e7d72-104">Exclusions help prevent incorrect detection of software and files unique or customized to your organization.</span></span> <span data-ttu-id="e7d72-105">Изключенията също допринасят за смекчаване на проблеми с производителността, предизвикани от MDATP.</span><span class="sxs-lookup"><span data-stu-id="e7d72-105">Exclusions also help mitigate performance problems caused by MDATP.</span></span>

<span data-ttu-id="e7d72-106">За да научите повече, вижте [Конфигуриране и проверка на изключвания за MDATP за Линукс](https://go.microsoft.com/fwlink/?linkid=2144517).</span><span class="sxs-lookup"><span data-stu-id="e7d72-106">To learn more, see [Configure and validate exclusions for MDATP for Linux](https://go.microsoft.com/fwlink/?linkid=2144517).</span></span>

> [!IMPORTANT]
> <span data-ttu-id="e7d72-107">Изключенията, описани в тази статия, не се прилагат към други възможности на MDATP за Linux, включително откриване на крайни точки и отговор (EDR).</span><span class="sxs-lookup"><span data-stu-id="e7d72-107">The exclusions described in this article don't apply to other capabilities of MDATP for Linux, including endpoint detection and response (EDR).</span></span> <span data-ttu-id="e7d72-108">Файлове, които изключвате чрез методите, описани в тази статия, все още могат да активират предупреждения за EDR и други възможности за откриване.</span><span class="sxs-lookup"><span data-stu-id="e7d72-108">Files that you exclude by using the methods described in this article can still trigger EDR alerts and other detection capabilities.</span></span>
