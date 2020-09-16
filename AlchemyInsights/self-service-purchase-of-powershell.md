---
title: Самостоятелно закупуване на PowerShell
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9001212"
- "3516"
ms.openlocfilehash: e6cc504ebef19cbe78f576d9b207fe2d951d0ef5
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: bg-BG
ms.lasthandoff: 09/14/2020
ms.locfileid: "47739959"
---
# <a name="self-service-purchase-of-powershell"></a><span data-ttu-id="f346d-102">Самостоятелно закупуване на PowerShell</span><span class="sxs-lookup"><span data-stu-id="f346d-102">Self-service purchase of PowerShell</span></span>

<span data-ttu-id="f346d-103">За да използвате модула на MSCommerce PowerShell, трябва да го инсталирате на устройство с Windows 10 с TLS 1,2 (изисква се локални разрешения за администратора).</span><span class="sxs-lookup"><span data-stu-id="f346d-103">To use the MSCommerce PowerShell module, you need to install it on a Windows 10 device with TLS 1.2 (local administrator permissions required).</span></span>  <span data-ttu-id="f346d-104">Импортиране и свързване към модула на MSCommerce.</span><span class="sxs-lookup"><span data-stu-id="f346d-104">Import and connect to the MSCommerce module.</span></span>  <span data-ttu-id="f346d-105">Когато получите подкана да влезете, ще трябва да използвате глобални или идентификационни данни за роля на администратор на фактуриране.</span><span class="sxs-lookup"><span data-stu-id="f346d-105">When prompted to log in, you will need to use Global or Billing Admin role credentials.</span></span>  

<span data-ttu-id="f346d-106">Ако нямате TLS 1,2, може да получите следната грешка, когато се опитвате да получите или актуализирате правилата:</span><span class="sxs-lookup"><span data-stu-id="f346d-106">If you don't have TLS 1.2, you may receive the following error when attempting to get or update the policy:</span></span>

<span data-ttu-id="f346d-107">*ErrorMessage – основната връзка е затворена: Възникна неочаквана грешка при изпращане*.</span><span class="sxs-lookup"><span data-stu-id="f346d-107">*ErrorMessage -The underlying connection was closed: An unexpected error occurred on a send*.</span></span>



