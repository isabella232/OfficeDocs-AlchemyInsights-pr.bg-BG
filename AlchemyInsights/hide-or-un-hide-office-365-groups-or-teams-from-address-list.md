---
title: Скриване или показване на групи или екипи на Office 365 от адресен списък
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9002947"
- "5642"
ms.openlocfilehash: 12e221c69775f3dfeed1781b70d3061e1ca0ac3b
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: bg-BG
ms.lasthandoff: 04/15/2021
ms.locfileid: "51811445"
---
# <a name="hide-or-un-hide-office-365-groups-or-teams-from-address-list"></a>Скриване или показване на групи или екипи на Office 365 от адресен списък

Използвайте следната команда на EXO PowerShell, за да скриете или покажете група/екипи на Office 365 от адресни списъци (GAL) на клиенти на Exchange (Outlook, OWA):

`
    Set-UnifiedGroup -Identity GroupName -HiddenFromAddressListsEnabled:<$true> or <$false>
`

Използвайте следната команда на EXO PowerShell, за да скриете или покажете група/екипи на Office 365 от клиенти на Exchange (Outlook, OWA):

`
    Set-unifiedGroup -Identity GroupName -HiddenFromExchangeClientsEnabled:<$true> or <$false>
`

- За подробни инструкции вж. [Скриване на групите на Office 365 от GAL и клиенти на Exchange](https://docs.microsoft.com/schooldatasync/hide-office-365-groups-from-the-gal).
