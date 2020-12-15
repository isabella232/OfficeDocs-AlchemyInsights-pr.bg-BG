---
title: Няма върнати резултати по време на търсене/Експортиране на съдържание
ms.author: v-jmathew
author: v-jmathew
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3200003"
- "7463"
ms.openlocfilehash: db025cd1278471a3c54d55409d9a9418095778a7
ms.sourcegitcommit: 9c64886a9e1a9b0ff356b28a5c1482ecc148d7ef
ms.translationtype: MT
ms.contentlocale: bg-BG
ms.lasthandoff: 12/14/2020
ms.locfileid: "49677190"
---
# <a name="no-results-returned-during-content-searchexport"></a><span data-ttu-id="781e1-102">Няма върнати резултати по време на търсене/Експортиране на съдържание</span><span class="sxs-lookup"><span data-stu-id="781e1-102">No results returned during Content Search/Export</span></span>

<span data-ttu-id="781e1-103">Ако имате проблеми със следните сценарии за откриване на електронни данни:</span><span class="sxs-lookup"><span data-stu-id="781e1-103">If you are experiencing issues with the following eDiscovery scenarios:</span></span>

- <span data-ttu-id="781e1-104">Търсене на съдържание/експортиране връща данни или неочаквани данни</span><span class="sxs-lookup"><span data-stu-id="781e1-104">Content Search/Export returns no data or unexpected data</span></span>
- <span data-ttu-id="781e1-105">Търсенето на откриване на електронни данни или експортирането е неуспешно</span><span class="sxs-lookup"><span data-stu-id="781e1-105">eDiscovery Search or Export fails</span></span>

<span data-ttu-id="781e1-106">Това може да се дължи на определени филтри за защита на съответствието, които са били настроени от определен администратор и не са били съобщени на всички администратори.</span><span class="sxs-lookup"><span data-stu-id="781e1-106">This may be caused due to certain Compliance Security Filters that were setup by a specific Admin and not been communicated to all Admins.</span></span>

<span data-ttu-id="781e1-107">За да отстраните този проблем, прегледайте дали има някои филтри за защита, които може да предизвикат следните проблеми:</span><span class="sxs-lookup"><span data-stu-id="781e1-107">To resolve this, check if there are any Compliance Security Filters that may be causing these issues:</span></span>

1. <span data-ttu-id="781e1-108">Свързване към центъра за сигурност и съответствие на PowerShell</span><span class="sxs-lookup"><span data-stu-id="781e1-108">Connect to Security and Compliance Center Powershell</span></span>
2. <span data-ttu-id="781e1-109">Изпълнете следните кратки команди:</span><span class="sxs-lookup"><span data-stu-id="781e1-109">Run the following commandlets:</span></span>

    `$org = “yourdomain.com”`

    `Get-ComplianceSecurityFilter -Organization $org`

<span data-ttu-id="781e1-110">За допълнителна информация относно филтрите за защита на съответствието вижте [филтриране на разрешения за търсене на съдържание](https://docs.microsoft.com/microsoft-365/compliance/permissions-filtering-for-content-search)</span><span class="sxs-lookup"><span data-stu-id="781e1-110">For additional information on Compliance Security Filters, see [Permissions Filtering for Content Search](https://docs.microsoft.com/microsoft-365/compliance/permissions-filtering-for-content-search)</span></span>
