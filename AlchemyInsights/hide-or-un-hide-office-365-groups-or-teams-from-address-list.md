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
ms.openlocfilehash: 7e667e22cd81f38a1a2c1385bf42e5227cb641480f4b505110ee7349a13f13a1
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: bg-BG
ms.lasthandoff: 08/05/2021
ms.locfileid: "54088385"
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
