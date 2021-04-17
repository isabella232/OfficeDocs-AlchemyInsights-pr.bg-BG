---
title: Инструкции за скриване/показване на група от адресен списък
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
- "1200024"
- "3161"
ms.openlocfilehash: 4d55866700b9b8494f1f692cd3b865116b96a1bc
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: bg-BG
ms.lasthandoff: 04/15/2021
ms.locfileid: "51831867"
---
# <a name="hide-microsoft-365-group-from-address-list-gal"></a>Скриване на групата на Microsoft 365 от адресния списък (GAL)

За да скриете група на Microsoft 365 от адресни списъци (GAL) на клиенти на Exchange (например Outlook или OWA), използвайте следната команда в обвивката на EXO:

`Set-UnifiedGroup -Identity GroupName -HiddenFromAddressListsEnabled:$true`

За да скриете групата Microsoft 365 от видима за клиентите на Exchange, използвайте следната команда в обвивката на EXO:

`Set-unifiedGroup -Identity GroupName -HiddenFromExchangeClientsEnabled:$true
Check this article for detailed instructions`

