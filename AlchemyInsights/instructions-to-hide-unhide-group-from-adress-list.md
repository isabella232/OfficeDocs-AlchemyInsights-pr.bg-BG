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
ms.openlocfilehash: af7085890d295cf0c41e11aaf18e404313413100cb8a1134bfac051d5fa26996
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: bg-BG
ms.lasthandoff: 08/05/2021
ms.locfileid: "53926234"
---
# <a name="hide-microsoft-365-group-from-address-list-gal"></a>Скриване Microsoft 365 група от адресен списък (GAL)

За да скриете Microsoft 365 от адресни списъци (GAL) на Exchange клиенти (например Outlook или OWA), използвайте следната команда в обвивката на EXO:

`Set-UnifiedGroup -Identity GroupName -HiddenFromAddressListsEnabled:$true`

За да скриете Microsoft 365 да бъде видима за Exchange клиенти, използвайте следната команда в обвивката на EXO:

`Set-unifiedGroup -Identity GroupName -HiddenFromExchangeClientsEnabled:$true
Check this article for detailed instructions`

