---
title: Търсене на съдържание няма резултати
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
- "9000661"
- "2527"
ms.openlocfilehash: 1e90c403556a317ff810971ccfa4a91694fb1171
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: bg-BG
ms.lasthandoff: 09/14/2020
ms.locfileid: "47680636"
---
# <a name="no-results-from-content-searchexports"></a><span data-ttu-id="d5025-102">Няма резултати от търсенето/експортиране на съдържание</span><span class="sxs-lookup"><span data-stu-id="d5025-102">No results from Content Search/Exports</span></span>

<span data-ttu-id="d5025-103">Проблемите при търсене/Експортиране на съдържание, които не връщат каквито и да е данни, може да се дължат на определен филтър за защита на съответствието, който е инсталирал от конкретен администратор и не го е информирал за всички администратори.</span><span class="sxs-lookup"><span data-stu-id="d5025-103">Issues with Content Search/Exports not returning any data may be due to certain Compliance Security Filter that was setup by a specific Admin and not communicating it to all Admins.</span></span>

<span data-ttu-id="d5025-104">За да отстраните това, проверете дали има филтри за защита за съответствие, които може да причиняват това:</span><span class="sxs-lookup"><span data-stu-id="d5025-104">To resolve this, check to see if there are any Compliance Security Filters that may be causing this:</span></span>
1. <span data-ttu-id="d5025-105">Свързване към центъра за сигурност и съответствие на PowerShell</span><span class="sxs-lookup"><span data-stu-id="d5025-105">Connect to Security and Compliance Center Powershell</span></span>
2. <span data-ttu-id="d5025-106">Изпълнете следните кратки команди:</span><span class="sxs-lookup"><span data-stu-id="d5025-106">Run the following commandlets:</span></span>
<br><span data-ttu-id="d5025-107">$org = "yourdomain.com"</span><span class="sxs-lookup"><span data-stu-id="d5025-107">$org = “yourdomain.com”</span></span>
<br><span data-ttu-id="d5025-108">Get-ComplianceSecurityFilter-$org за организация</span><span class="sxs-lookup"><span data-stu-id="d5025-108">Get-ComplianceSecurityFilter -Organization $org</span></span>