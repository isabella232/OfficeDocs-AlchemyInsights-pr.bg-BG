---
title: Няма резултати от търсене на съдържание
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000661"
- "2527"
ms.openlocfilehash: 09cdbc3cb0465e0e0bc08872c49e283081ad3e92
ms.sourcegitcommit: 1d98db8acb9959aba3b5e308a567ade6b62da56c
ms.translationtype: MT
ms.contentlocale: bg-BG
ms.lasthandoff: 08/22/2019
ms.locfileid: "36516768"
---
# <a name="no-results-from-content-searchexports"></a><span data-ttu-id="04412-102">Няма резултати от съдържание търсене/износ</span><span class="sxs-lookup"><span data-stu-id="04412-102">No results from Content Search/Exports</span></span>

<span data-ttu-id="04412-103">Проблеми със съдържание търсене/износ не връща никакви данни може да се дължи филтър за защита някои съответствието, който е настройка от един определен администратор и не се свързва към всички администратори.</span><span class="sxs-lookup"><span data-stu-id="04412-103">Issues with Content Search/Exports not returning any data may be due to certain Compliance Security Filter that was setup by a specific Admin and not communicating it to all Admins.</span></span>

<span data-ttu-id="04412-104">За да разрешите този проблем, проверете да видите дали има някакви съответствие защитни филтри, които могат да се причинява това:</span><span class="sxs-lookup"><span data-stu-id="04412-104">To resolve this, check to see if there are any Compliance Security Filters that may be causing this:</span></span>
1. <span data-ttu-id="04412-105">Свързване към сигурността и съответствието център Powershell</span><span class="sxs-lookup"><span data-stu-id="04412-105">Connect to Security and Compliance Center Powershell</span></span>
2. <span data-ttu-id="04412-106">Изпълнете следните кратки команди:</span><span class="sxs-lookup"><span data-stu-id="04412-106">Run the following commandlets:</span></span>
<br><span data-ttu-id="04412-107">$org = "yourdomain.com"</span><span class="sxs-lookup"><span data-stu-id="04412-107">$org = “yourdomain.com”</span></span>
<br><span data-ttu-id="04412-108">Get-ComplianceSecurityFilter-организация $org</span><span class="sxs-lookup"><span data-stu-id="04412-108">Get-ComplianceSecurityFilter -Organization $org</span></span>