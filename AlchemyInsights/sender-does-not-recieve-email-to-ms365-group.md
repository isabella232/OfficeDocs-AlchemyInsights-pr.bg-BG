---
title: Подателят не получава имейли, изпратени до групата на Microsoft 365
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 08/20/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9003200"
ms.openlocfilehash: b3b438e17c35f18289d3e9c3ca89d16a6f2a065f
ms.sourcegitcommit: dcca0df53f9194f406cf3a5f6b046cb33a0a5b03
ms.translationtype: MT
ms.contentlocale: bg-BG
ms.lasthandoff: 08/21/2020
ms.locfileid: "46871608"
---
# <a name="sender-does-not-receive-email-sent-to-microsoft-365-group"></a><span data-ttu-id="899fe-102">Подателят не получава имейли, изпратени до групата на Microsoft 365</span><span class="sxs-lookup"><span data-stu-id="899fe-102">Sender does not receive email sent to Microsoft 365 group</span></span>

<span data-ttu-id="899fe-103">По подразбиране подателят на имейл съобщение до група на Microsoft 365 не получава копие на съобщението в своята папка "Входящи", дори ако подателят е член на групата.</span><span class="sxs-lookup"><span data-stu-id="899fe-103">By default, the sender of an email message to a Microsoft 365 group doesn't receive a copy of the message in their Inbox, even if the sender is a member of the group.</span></span>

<span data-ttu-id="899fe-104">Използвайте тази команда на командата ЕКСО, за да разрешите на подателя да получи копие на всеки имейл, изпратен от групата на Microsoft 365:</span><span class="sxs-lookup"><span data-stu-id="899fe-104">Use this EXO PowerShell command to allow the sender to receive a copy of each email they send to the Microsoft 365 group:</span></span>  

`Set-MailboxMessageConfiguration <MailboxName> -EchoGroupMessageBackToSubscribedSender $True`  

<span data-ttu-id="899fe-105">За да разрешите настройката за всички пощенски кутии наведнъж:</span><span class="sxs-lookup"><span data-stu-id="899fe-105">To enable the setting for all mailboxes at once:</span></span>

`Get-Mailbox -ResultSize Unlimited | ForEach {Set-MailboxMessageConfiguration -Identity $_.UserPrincipalName -EchoGroupMessageBackToSubscribedSender $true}` 

<span data-ttu-id="899fe-106">**Забележка** Промените в тази настройка отнемат до един час, за да влязат в сила.</span><span class="sxs-lookup"><span data-stu-id="899fe-106">**Note** Changes to this setting take up to an hour to take effect.</span></span>