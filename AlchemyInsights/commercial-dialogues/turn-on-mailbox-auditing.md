---
title: Включване на проверката на пощенските кутии
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 02/26/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3100005"
- "7327"
ms.openlocfilehash: aa0ff925ae891d28e31394ec66eb17c2d9710008
ms.sourcegitcommit: 251e2e82571fb3bb1fbe3dbf7bfca30e004b3373
ms.translationtype: MT
ms.contentlocale: bg-BG
ms.lasthandoff: 03/05/2021
ms.locfileid: "50481039"
---
# <a name="turn-on-mailbox-auditing"></a><span data-ttu-id="0e732-102">Включване на проверката на пощенските кутии</span><span class="sxs-lookup"><span data-stu-id="0e732-102">Turn on mailbox auditing</span></span>

<span data-ttu-id="0e732-103">За да включите проверката на пощенските кутии за отделен потребител или за цялата организация, изпълнете следните кратки команди от отдалечения PowerShell:</span><span class="sxs-lookup"><span data-stu-id="0e732-103">To turn on mailbox auditing for a single user or an entire organization, run the following cmdlets from Remote PowerShell:</span></span>

- <span data-ttu-id="0e732-104">**Отделен потребител**: Set-Mailbox самоличност "Яне Дау" – AuditEnabled $True</span><span class="sxs-lookup"><span data-stu-id="0e732-104">**Single user**: Set-Mailbox -Identity "Jane Dow" -AuditEnabled $true</span></span>
- <span data-ttu-id="0e732-105">**Организация**: Get-Mailbox-ResultSize Unlimited-Filter {RecipientTypeDetails-EQ "UserMailbox"} | Set-Mailbox-AuditEnabled $true</span><span class="sxs-lookup"><span data-stu-id="0e732-105">**Organization**: Get-Mailbox -ResultSize Unlimited -Filter {RecipientTypeDetails -eq "UserMailbox"} | Set-Mailbox -AuditEnabled $true</span></span>

<span data-ttu-id="0e732-106">За да научите повече, вижте [управление на проверката на пощенските кутии](https://go.microsoft.com/fwlink/?linkid=2103668).</span><span class="sxs-lookup"><span data-stu-id="0e732-106">To learn more, see [Manage mailbox auditing](https://go.microsoft.com/fwlink/?linkid=2103668).</span></span>