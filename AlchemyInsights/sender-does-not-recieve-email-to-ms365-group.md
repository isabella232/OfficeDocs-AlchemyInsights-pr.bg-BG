---
title: Подателят не получава имейл, изпратен до Microsoft 365 група
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 08/20/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9003200"
ms.openlocfilehash: 893b80567567590357a638370b8c8d58b87a98a51c68cfcc84629eda5ac71b44
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: bg-BG
ms.lasthandoff: 08/05/2021
ms.locfileid: "53958286"
---
# <a name="sender-does-not-receive-email-sent-to-microsoft-365-group"></a>Подателят не получава имейл, изпратен до Microsoft 365 група

По подразбиране подателят на имейл съобщение до група Microsoft 365 не получава копие на съобщението в своята папка "Входящи", дори ако подателят е член на групата.

Използвайте тази команда exo PowerShell, за да позволите на подателя да получава копие на всеки имейл, който изпраща на Microsoft 365 група:  

`Set-MailboxMessageConfiguration <MailboxName> -EchoGroupMessageBackToSubscribedSender $True`  

За да разрешите настройката за всички пощенски кутии наведнъж:

`Get-Mailbox -ResultSize Unlimited | ForEach {Set-MailboxMessageConfiguration -Identity $_.UserPrincipalName -EchoGroupMessageBackToSubscribedSender $true}` 

**Забележка** Промените в тази настройка отнемат до един час, за да влязат в сила.