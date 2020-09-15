---
title: Инструкции за скриване и показване на групата от адресния списък
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "1200024"
- "3161"
ms.openlocfilehash: 1ad9ab294d46ca0fc88a454e3503ddcf80398896
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: bg-BG
ms.lasthandoff: 09/14/2020
ms.locfileid: "47662998"
---
# <a name="hide-microsoft-365-group-from-address-list-gal"></a><span data-ttu-id="bbda9-102">Скрий Microsoft 365 Group от адресния списък (GAL)</span><span class="sxs-lookup"><span data-stu-id="bbda9-102">Hide Microsoft 365 group from address list (GAL)</span></span>

<span data-ttu-id="bbda9-103">За да скриете група на Microsoft 365 от адресни списъци (GAL) на клиенти на Exchange (като например Outlook или OWA), използвайте следната команда в обвивката:</span><span class="sxs-lookup"><span data-stu-id="bbda9-103">To hide a Microsoft 365 group from address lists (GAL) of Exchange clients (such as Outlook or OWA), use the following command in EXO shell:</span></span>

`Set-UnifiedGroup -Identity GroupName -HiddenFromAddressListsEnabled:$true`

<span data-ttu-id="bbda9-104">За да скриете групата на Microsoft 365, която е видима за клиенти на Exchange, използвайте следната команда в обвивката на ЕКСО:</span><span class="sxs-lookup"><span data-stu-id="bbda9-104">To hide the Microsoft 365 group from being visible to Exchange clients, use the following command in EXO shell:</span></span>

`Set-unifiedGroup -Identity GroupName -HiddenFromExchangeClientsEnabled:$true
Check this article for detailed instructions`

