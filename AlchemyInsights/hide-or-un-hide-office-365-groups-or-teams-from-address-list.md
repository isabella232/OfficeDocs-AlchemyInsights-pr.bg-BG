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
# <a name="hide-or-un-hide-office-365-groups-or-teams-from-address-list"></a>Скриване или скриване на Office 365 групи или екипи от адресния списък

Използвайте командата EXO PowerShell да скриете или ООН-скрий група/екипи на Office 365 от адресните списъци (GAL) на Exchange клиенти (Outlook, OWA):

`
    Set-UnifiedGroup -Identity GroupName -HiddenFromAddressListsEnabled:<$true> or <$false>
`

Използвайте командата EXO PowerShell да скриете или оон-скрий групата Office365 от Exchange клиенти (Outlook, OWA):

`
    Set-unifiedGroup -Identity GroupName -HiddenFromExchangeClientsEnabled:<$true> or <$false>
`

- За подробни инструкции вижте [Скриване на Office 365 групи от глобалния адрес и Exchange клиенти](https://docs.microsoft.com/schooldatasync/hide-office-365-groups-from-the-gal).
