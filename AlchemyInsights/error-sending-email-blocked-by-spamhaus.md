---
title: Грешка при изпращане на имейл, блокиран от SpamHaus
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "255"
- "3100003"
ms.assetid: fa98ab4a-92eb-45e9-8d57-ad10fb123042
ms.openlocfilehash: 8b5ac1df0b6a07a475345235a8b4b555d6881147
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: bg-BG
ms.lasthandoff: 04/15/2021
ms.locfileid: "51813713"
---
# <a name="error-sending-email-client-host-blocked-using-spamhaus"></a><span data-ttu-id="0239f-102">Грешка при изпращане на имейл: Хостът на клиента е блокиран с помощта на Spamhaus</span><span class="sxs-lookup"><span data-stu-id="0239f-102">Error sending email: Client host blocked using Spamhaus</span></span>

<span data-ttu-id="0239f-103">IP адресът, който е изпратил съобщението, е в списък за блокиране, притежаван [от Spamhaus.](https://go.microsoft.com/fwlink/p/?linkid=123245)</span><span class="sxs-lookup"><span data-stu-id="0239f-103">The IP address that sent the message is on a block list owned by [Spamhaus](https://go.microsoft.com/fwlink/p/?linkid=123245).</span></span> <span data-ttu-id="0239f-104">Причините за блокиране от Spamhaus включват компрометирани акаунти, компрометирани машини, споделящи публичен IP адрес, и правила за доставчик на интернет (ISP).</span><span class="sxs-lookup"><span data-stu-id="0239f-104">Reasons for being blocked by Spamhaus include compromised accounts, compromised machines sharing a public IP address, and Internet Service Provider (ISP) policies.</span></span> <span data-ttu-id="0239f-105">Възможните корекции са:</span><span class="sxs-lookup"><span data-stu-id="0239f-105">Possible fixes are:</span></span>
  
- <span data-ttu-id="0239f-106">За блокирани входящи съобщения, където управлявате изходния имейл сървър, трябва да определите причината и да премахнете блока от уеб сайта на Spamhaus.</span><span class="sxs-lookup"><span data-stu-id="0239f-106">For blocked inbound messages where you control the source email server, you need to determine the cause and remove the block from the Spamhaus website.</span></span>

- <span data-ttu-id="0239f-107">За блокирани входящи съобщения, където IP адресът източник принадлежи на някой друг, собственикът на адреса трябва да премахне блока от уеб сайта на Spamhaus.</span><span class="sxs-lookup"><span data-stu-id="0239f-107">For blocked inbound messages where the source IP address belongs to someone else, the address owner needs to remove the block from the Spamhaus website.</span></span> <span data-ttu-id="0239f-108">Ако IP адресът е в списъка с блокирани правила (PBL), собственикът може да назначи друг статичен IP адрес или да премахне адреса от PBL.</span><span class="sxs-lookup"><span data-stu-id="0239f-108">If the IP address is on the Policy Block List (PBL), the owner can assign a different static IP address or remove the address from the PBL.</span></span>

- <span data-ttu-id="0239f-109">За блокирани изходящи съобщения от вашия домейн, свързани с Microsoft, можете да получите тази грешка, ако съобщенията се маршрутизирани чрез услуга на трета страна.</span><span class="sxs-lookup"><span data-stu-id="0239f-109">For blocked outbound messages from your domain connected to Microsoft, you can receive this error if the messages are routed through a 3rd party service.</span></span> <span data-ttu-id="0239f-110">Можете да използвате инструмент за търсене на WHOIS, за да намерите собственика на блокирания IP адрес.</span><span class="sxs-lookup"><span data-stu-id="0239f-110">You can use a WHOIS lookup tool to find the blocked IP address owner.</span></span>
