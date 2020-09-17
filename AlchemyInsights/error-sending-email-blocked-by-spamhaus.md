---
title: Грешка при изпращане на имейл, блокиран от SpamHaus
ms.author: pebaum
author: pebaum
manager: mnirkhe
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
ms.openlocfilehash: a0c2f4be0b2d8ba6fd3dadbdf306e6ce623ad380
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: bg-BG
ms.lasthandoff: 09/15/2020
ms.locfileid: "47783756"
---
# <a name="error-sending-email-client-host-blocked-using-spamhaus"></a><span data-ttu-id="f0a91-102">Грешка при изпращане на имейл: хостът на клиента е блокиран чрез SpamHaus</span><span class="sxs-lookup"><span data-stu-id="f0a91-102">Error sending email: Client host blocked using Spamhaus</span></span>

<span data-ttu-id="f0a91-103">IP адресът, който е изпратил съобщението, е в списък на блокирани, собственост на [SpamHaus](https://go.microsoft.com/fwlink/p/?linkid=123245).</span><span class="sxs-lookup"><span data-stu-id="f0a91-103">The IP address that sent the message is on a block list owned by [Spamhaus](https://go.microsoft.com/fwlink/p/?linkid=123245).</span></span> <span data-ttu-id="f0a91-104">Причините за блокирането на SpamHaus включват компрометирани акаунти, компрометирани машини, споделящи публичен IP адрес и правила за интернет доставчик (ISP).</span><span class="sxs-lookup"><span data-stu-id="f0a91-104">Reasons for being blocked by Spamhaus include compromised accounts, compromised machines sharing a public IP address, and Internet Service Provider (ISP) policies.</span></span> <span data-ttu-id="f0a91-105">Възможните корекции са:</span><span class="sxs-lookup"><span data-stu-id="f0a91-105">Possible fixes are:</span></span>
  
- <span data-ttu-id="f0a91-106">За блокирани входящи съобщения, където можете да управлявате изходния имейл сървър, трябва да определите причината и да премахнете блока от уеб сайта на SpamHaus.</span><span class="sxs-lookup"><span data-stu-id="f0a91-106">For blocked inbound messages where you control the source email server, you need to determine the cause and remove the block from the Spamhaus website.</span></span>

- <span data-ttu-id="f0a91-107">За блокирани входящи съобщения, в които IP адресът източник принадлежи на някой друг, собственикът на адреса трябва да премахне блока от уеб сайта на SpamHaus.</span><span class="sxs-lookup"><span data-stu-id="f0a91-107">For blocked inbound messages where the source IP address belongs to someone else, the address owner needs to remove the block from the Spamhaus website.</span></span> <span data-ttu-id="f0a91-108">Ако IP адресът е в списъка с блокирани правила (PBL), собственикът може да назначи различен статичен IP адрес или да премахне адреса на PBL.</span><span class="sxs-lookup"><span data-stu-id="f0a91-108">If the IP address is on the Policy Block List (PBL), the owner can assign a different static IP address or remove the address from the PBL.</span></span>

- <span data-ttu-id="f0a91-109">За блокирани изходящи съобщения от вашия домейн, които са свързани с Microsoft, можете да получите тази грешка, ако съобщенията се маршрутизират чрез услуга на трети страни.</span><span class="sxs-lookup"><span data-stu-id="f0a91-109">For blocked outbound messages from your domain connected to Microsoft, you can receive this error if the messages are routed through a 3rd party service.</span></span> <span data-ttu-id="f0a91-110">Можете да използвате инструмент за търсене WHOIS, за да намерите блокирания собственик на IP адреси.</span><span class="sxs-lookup"><span data-stu-id="f0a91-110">You can use a WHOIS lookup tool to find the blocked IP address owner.</span></span>
