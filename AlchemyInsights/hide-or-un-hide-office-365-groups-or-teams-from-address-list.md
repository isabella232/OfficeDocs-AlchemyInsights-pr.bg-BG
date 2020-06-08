---
title: Скриване или скриване на Office 365 групи или екипи от адресния списък
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9002947"
- "5642"
ms.openlocfilehash: cb3c2819ff7203774511bd0e45633b59a02091ff
ms.sourcegitcommit: e3a1f96200bc58dc8a5b3597cc2600e71c4bd266
ms.translationtype: MT
ms.contentlocale: bg-BG
ms.lasthandoff: 05/14/2020
ms.locfileid: "44225325"
---
# <a name="hide-or-un-hide-office-365-groups-or-teams-from-address-list"></a><span data-ttu-id="4dc21-102">Скриване или скриване на Office 365 групи или екипи от адресния списък</span><span class="sxs-lookup"><span data-stu-id="4dc21-102">Hide or un-hide Office 365 groups or teams from address list</span></span>

<span data-ttu-id="4dc21-103">Използвайте командата EXO PowerShell да скриете или ООН-скрий група/екипи на Office 365 от адресните списъци (GAL) на Exchange клиенти (Outlook, OWA):</span><span class="sxs-lookup"><span data-stu-id="4dc21-103">Use the following EXO PowerShell command to hide or un-hide Office 365 group/teams from address lists (GAL) of Exchange clients (Outlook, OWA):</span></span>

`
    Set-UnifiedGroup -Identity GroupName -HiddenFromAddressListsEnabled:<$true> or <$false>
`

<span data-ttu-id="4dc21-104">Използвайте командата EXO PowerShell да скриете или оон-скрий групата Office365 от Exchange клиенти (Outlook, OWA):</span><span class="sxs-lookup"><span data-stu-id="4dc21-104">Use the following EXO PowerShell command to hide or un-hide the Office365 group/teams from Exchange clients (Outlook, OWA):</span></span>

`
    Set-unifiedGroup -Identity GroupName -HiddenFromExchangeClientsEnabled:<$true> or <$false>
`

- <span data-ttu-id="4dc21-105">За подробни инструкции вижте [Скриване на Office 365 групи от глобалния адрес и Exchange клиенти](https://docs.microsoft.com/schooldatasync/hide-office-365-groups-from-the-gal).</span><span class="sxs-lookup"><span data-stu-id="4dc21-105">For detailed instructions, see [Hide Office 365 Groups from the GAL and Exchange Clients](https://docs.microsoft.com/schooldatasync/hide-office-365-groups-from-the-gal).</span></span>
