---
title: Търсене на съдържание Без резултати
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
- "9000661"
- "2527"
ms.openlocfilehash: 0267286ca5967ee891e65343d49adf776f0322a6
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: bg-BG
ms.lasthandoff: 04/15/2021
ms.locfileid: "51816837"
---
# <a name="no-results-from-content-searchexports"></a><span data-ttu-id="02919-102">Няма резултати от търсене/експортиране на съдържание</span><span class="sxs-lookup"><span data-stu-id="02919-102">No results from Content Search/Exports</span></span>

<span data-ttu-id="02919-103">Проблеми с търсенето/експортирането на съдържание, които не връщат никакви данни, може да се дължат на определен филтър за защита на съответствието, който е бил настроен от конкретен администратор и не го съобщава на всички администратори.</span><span class="sxs-lookup"><span data-stu-id="02919-103">Issues with Content Search/Exports not returning any data may be due to certain Compliance Security Filter that was setup by a specific Admin and not communicating it to all Admins.</span></span>

<span data-ttu-id="02919-104">За да отстраните това, проверете дали има някакви филтри за защита на съответствието, които може да са причина за това:</span><span class="sxs-lookup"><span data-stu-id="02919-104">To resolve this, check to see if there are any Compliance Security Filters that may be causing this:</span></span>
1. <span data-ttu-id="02919-105">Свързване към центъра за защита и съответствие Powershell</span><span class="sxs-lookup"><span data-stu-id="02919-105">Connect to Security and Compliance Center Powershell</span></span>
2. <span data-ttu-id="02919-106">Изпълнете следните команди:</span><span class="sxs-lookup"><span data-stu-id="02919-106">Run the following commandlets:</span></span>
<br><span data-ttu-id="02919-107">$org = "yourdomain.com"</span><span class="sxs-lookup"><span data-stu-id="02919-107">$org = “yourdomain.com”</span></span>
<br><span data-ttu-id="02919-108">Get-ComplianceSecurityFilter -Organization $org</span><span class="sxs-lookup"><span data-stu-id="02919-108">Get-ComplianceSecurityFilter -Organization $org</span></span>