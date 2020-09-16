---
title: Подателят не получава имейли, изпратени до групата на Microsoft 365
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
ms.openlocfilehash: b8091305d55408f51cf369506acc7bfac59defb5
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: bg-BG
ms.lasthandoff: 09/14/2020
ms.locfileid: "47751304"
---
# <a name="sender-does-not-receive-email-sent-to-microsoft-365-group"></a>Подателят не получава имейли, изпратени до групата на Microsoft 365

По подразбиране подателят на имейл съобщение до група на Microsoft 365 не получава копие на съобщението в своята папка "Входящи", дори ако подателят е член на групата.

Използвайте тази команда на командата ЕКСО, за да разрешите на подателя да получи копие на всеки имейл, изпратен от групата на Microsoft 365:  

`Set-MailboxMessageConfiguration <MailboxName> -EchoGroupMessageBackToSubscribedSender $True`  

За да разрешите настройката за всички пощенски кутии наведнъж:

`Get-Mailbox -ResultSize Unlimited | ForEach {Set-MailboxMessageConfiguration -Identity $_.UserPrincipalName -EchoGroupMessageBackToSubscribedSender $true}` 

**Забележка** Промените в тази настройка отнемат до един час, за да влязат в сила.