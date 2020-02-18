---
title: Самостоятелно закупуване на PowerShell
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9001212"
- "3516"
ms.openlocfilehash: 5e47e08e3309b3d58908e10ee06021da00f230bb
ms.sourcegitcommit: cb9505f9eca032af3a4194c68d18c91789365690
ms.translationtype: MT
ms.contentlocale: bg-BG
ms.lasthandoff: 02/16/2020
ms.locfileid: "42091661"
---
# <a name="self-service-purchase-of-powershell"></a><span data-ttu-id="f56b6-102">Самостоятелно закупуване на PowerShell</span><span class="sxs-lookup"><span data-stu-id="f56b6-102">Self-service purchase of PowerShell</span></span>

<span data-ttu-id="f56b6-103">За да използвате модула MSCommerce PowerShell, трябва да го инсталирате на устройство с Windows 10 с TLS 1.2 (изисква се разрешения за локален администратор).</span><span class="sxs-lookup"><span data-stu-id="f56b6-103">To use the MSCommerce PowerShell module, you need to install it on a Windows 10 device with TLS 1.2 (local administrator permissions required).</span></span>  <span data-ttu-id="f56b6-104">Импортиране и свързване с MSCommerce модула.</span><span class="sxs-lookup"><span data-stu-id="f56b6-104">Import and connect to the MSCommerce module.</span></span>  <span data-ttu-id="f56b6-105">Когато получите подкана да влезете, ще трябва да използвате идентификационните данни за роля на глобален или администратор на плащания.</span><span class="sxs-lookup"><span data-stu-id="f56b6-105">When prompted to log in, you will need to use Global or Billing Admin role credentials.</span></span>  

<span data-ttu-id="f56b6-106">Ако нямате TLS 1.2, можете да получите следното съобщение за грешка при опит за получаване или актуализиране на правилата:</span><span class="sxs-lookup"><span data-stu-id="f56b6-106">If you don't have TLS 1.2, you may receive the following error when attempting to get or update the policy:</span></span>

<span data-ttu-id="f56b6-107">*ErrorMessage -основната връзка е затворена: Възникна неочаквана грешка при изпращане*.</span><span class="sxs-lookup"><span data-stu-id="f56b6-107">*ErrorMessage -The underlying connection was closed: An unexpected error occurred on a send*.</span></span>



