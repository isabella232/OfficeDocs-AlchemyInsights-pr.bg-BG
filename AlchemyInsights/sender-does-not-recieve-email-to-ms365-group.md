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
# <a name="sender-does-not-receive-email-sent-to-microsoft-365-group"></a><span data-ttu-id="bcdab-102">Подателят не получава имейли, изпратени до групата на Microsoft 365</span><span class="sxs-lookup"><span data-stu-id="bcdab-102">Sender does not receive email sent to Microsoft 365 group</span></span>

<span data-ttu-id="bcdab-103">По подразбиране подателят на имейл съобщение до група на Microsoft 365 не получава копие на съобщението в своята папка "Входящи", дори ако подателят е член на групата.</span><span class="sxs-lookup"><span data-stu-id="bcdab-103">By default, the sender of an email message to a Microsoft 365 group doesn't receive a copy of the message in their Inbox, even if the sender is a member of the group.</span></span>

<span data-ttu-id="bcdab-104">Използвайте тази команда на командата ЕКСО, за да разрешите на подателя да получи копие на всеки имейл, изпратен от групата на Microsoft 365:</span><span class="sxs-lookup"><span data-stu-id="bcdab-104">Use this EXO PowerShell command to allow the sender to receive a copy of each email they send to the Microsoft 365 group:</span></span>  

`Set-MailboxMessageConfiguration <MailboxName> -EchoGroupMessageBackToSubscribedSender $True`  

<span data-ttu-id="bcdab-105">За да разрешите настройката за всички пощенски кутии наведнъж:</span><span class="sxs-lookup"><span data-stu-id="bcdab-105">To enable the setting for all mailboxes at once:</span></span>

`Get-Mailbox -ResultSize Unlimited | ForEach {Set-MailboxMessageConfiguration -Identity $_.UserPrincipalName -EchoGroupMessageBackToSubscribedSender $true}` 

<span data-ttu-id="bcdab-106">**Забележка** Промените в тази настройка отнемат до един час, за да влязат в сила.</span><span class="sxs-lookup"><span data-stu-id="bcdab-106">**Note** Changes to this setting take up to an hour to take effect.</span></span>