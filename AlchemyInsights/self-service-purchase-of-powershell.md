---
title: Самостоятелно закупуване на PowerShell
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9001212"
- "3516"
ms.openlocfilehash: 48b5b0a1be1bc03d45a531a1093f18a3f750c37d
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: bg-BG
ms.lasthandoff: 04/15/2021
ms.locfileid: "51797710"
---
# <a name="self-service-purchase-of-powershell"></a><span data-ttu-id="30ec6-102">Самостоятелно закупуване на PowerShell</span><span class="sxs-lookup"><span data-stu-id="30ec6-102">Self-service purchase of PowerShell</span></span>

<span data-ttu-id="30ec6-103">За да използвате модула MSCommerce PowerShell, трябва да го инсталирате на устройство с Windows 10 с TLS 1.2 (необходими са разрешения на локален администратор).</span><span class="sxs-lookup"><span data-stu-id="30ec6-103">To use the MSCommerce PowerShell module, you need to install it on a Windows 10 device with TLS 1.2 (local administrator permissions required).</span></span>  <span data-ttu-id="30ec6-104">Импортиране и свързване към модула MSCommerce.</span><span class="sxs-lookup"><span data-stu-id="30ec6-104">Import and connect to the MSCommerce module.</span></span>  <span data-ttu-id="30ec6-105">Когато получите подкана да влезете, ще трябва да използвате идентификационните данни за роля на глобален администратор или администратор на фактуриране.</span><span class="sxs-lookup"><span data-stu-id="30ec6-105">When prompted to log in, you will need to use Global or Billing Admin role credentials.</span></span>  

<span data-ttu-id="30ec6-106">Ако нямате TLS 1.2, може да получите следната грешка, когато се опитвате да получите или актуализирате правилата:</span><span class="sxs-lookup"><span data-stu-id="30ec6-106">If you don't have TLS 1.2, you may receive the following error when attempting to get or update the policy:</span></span>

<span data-ttu-id="30ec6-107">*ErrorMessage -Базовата връзка е затворена: Възникна неочаквана грешка при изпращане*.</span><span class="sxs-lookup"><span data-stu-id="30ec6-107">*ErrorMessage -The underlying connection was closed: An unexpected error occurred on a send*.</span></span>



