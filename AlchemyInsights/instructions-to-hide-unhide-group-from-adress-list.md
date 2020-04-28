---
title: Инструкции за скриване / скриване на група от адресния списък
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "1200024"
- "3161"
ms.openlocfilehash: 61ba34e6d554831da712a92401f26fabb02c26b7
ms.sourcegitcommit: 286000b588adef1bbbb28337a9d9e087ec783fa2
ms.translationtype: MT
ms.contentlocale: bg-BG
ms.lasthandoff: 04/27/2020
ms.locfileid: "43908333"
---
# <a name="hide-microsoft-365-group-from-address-list-gal"></a>Скрий microsoft 365 група от адресния списък (GAL)

За да скриете Microsoft 365 група от адресни списъци (GAL) на Exchange клиенти (като Outlook или OWA), използвайте следната команда в обвивката НА EXO:

`Set-UnifiedGroup -Identity GroupName -HiddenFromAddressListsEnabled:$true`

За да скриете microsoft 365 група от видими за клиенти на Exchange, използвайте следната команда в обвивката EXO:

`Set-unifiedGroup -Identity GroupName -HiddenFromExchangeClientsEnabled:$true
Check this article for detailed instructions`

