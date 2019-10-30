---
title: Инструкции за скриване/скриване на група от адресен списък
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
ms.openlocfilehash: d0e0285701f1a5f308bdc682abaddf5cc2d34120
ms.sourcegitcommit: defe2c412567b596fa8c3ab52111bde712ebb314
ms.translationtype: MT
ms.contentlocale: bg-BG
ms.lasthandoff: 10/29/2019
ms.locfileid: "37768900"
---
# <a name="hide-office-365-group-from-address-list-gal"></a>Скриване на Office 365 група от адресен списък (GAL)

За да скриете Office 365 група от адресни списъци (GAL) на Exchange клиенти (като Outlook или OWA), използвайте следната команда в ЕКЗО обвивка:

`Set-UnifiedGroup -Identity GroupName -HiddenFromAddressListsEnabled:$true`

За да скриете Office 365 група от е видима за Exchange клиенти, използвайте следната команда в ЕКЗО обвивка:

`Set-unifiedGroup -Identity GroupName -HiddenFromExchangeClientsEnabled:$true
Check this article for detailed instructions`

