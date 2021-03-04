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
ms.sourcegitcommit: f4ba304b92ed01e35273ecda67e9dc3ad9d475c1
ms.translationtype: MT
ms.contentlocale: bg-BG
ms.lasthandoff: 03/04/2021
ms.locfileid: "50429255"
---
# <a name="turn-on-mailbox-auditing"></a>Включване на проверката на пощенските кутии

За да включите проверката на пощенските кутии за отделен потребител или за цялата организация, изпълнете следните кратки команди от отдалечения PowerShell:

- **Отделен потребител**: Set-Mailbox самоличност "Яне Дау" – AuditEnabled $True
- **Организация**: Get-Mailbox-ResultSize Unlimited-Filter {RecipientTypeDetails-EQ "UserMailbox"} | Set-Mailbox-AuditEnabled $true

За да научите повече, вижте [управление на проверката на пощенските кутии](https://go.microsoft.com/fwlink/?linkid=2103668).