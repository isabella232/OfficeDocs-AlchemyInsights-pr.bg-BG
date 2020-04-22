---
title: Грешка при изпращане на имейл, блокиран от SpamHaus
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "255"
- "3100003"
ms.assetid: fa98ab4a-92eb-45e9-8d57-ad10fb123042
ms.openlocfilehash: 3ff4f7a155fe74f5b42a1bd43e67ef0a751d7fbd
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: bg-BG
ms.lasthandoff: 04/22/2020
ms.locfileid: "43714247"
---
# <a name="error-sending-email-client-host-blocked-using-spamhaus"></a><span data-ttu-id="61ab4-102">Грешка при изпращане на имейл: Клиент хост блокирани използване на Spamhaus</span><span class="sxs-lookup"><span data-stu-id="61ab4-102">Error sending email: Client host blocked using Spamhaus</span></span>

<span data-ttu-id="61ab4-103">IP адресът, който е изпратил съобщението, е в списък с блокирани собственост на [Spamhaus](https://go.microsoft.com/fwlink/p/?linkid=123245).</span><span class="sxs-lookup"><span data-stu-id="61ab4-103">The IP address that sent the message is on a block list owned by [Spamhaus](https://go.microsoft.com/fwlink/p/?linkid=123245).</span></span> <span data-ttu-id="61ab4-104">Причините за блокиране от Spamhaus включват компрометирани акаунти, компрометирани машини, които споделят публичен IP адрес и правила на интернет доставчик (ISP).</span><span class="sxs-lookup"><span data-stu-id="61ab4-104">Reasons for being blocked by Spamhaus include compromised accounts, compromised machines sharing a public IP address, and Internet Service Provider (ISP) policies.</span></span> <span data-ttu-id="61ab4-105">Възможните корекции са:</span><span class="sxs-lookup"><span data-stu-id="61ab4-105">Possible fixes are:</span></span>
  
- <span data-ttu-id="61ab4-106">За блокирани входящи съобщения, където можете да контролирате източник имейл сървър, трябва да определите причината и да премахнете блок от сайта на Спамхаус.</span><span class="sxs-lookup"><span data-stu-id="61ab4-106">For blocked inbound messages where you control the source email server, you need to determine the cause and remove the block from the Spamhaus website.</span></span>

- <span data-ttu-id="61ab4-107">Блокирани входящи съобщения, където източник IP адрес принадлежи на някой друг, собственикът на адреса трябва да премахне блок от сайта на спамхаус.</span><span class="sxs-lookup"><span data-stu-id="61ab4-107">For blocked inbound messages where the source IP address belongs to someone else, the address owner needs to remove the block from the Spamhaus website.</span></span> <span data-ttu-id="61ab4-108">Ако IP адресът е в списъка с правила блок (PBL), собственикът може да присвоите различен статичен IP адрес или премахнете адреса от PBL.</span><span class="sxs-lookup"><span data-stu-id="61ab4-108">If the IP address is on the Policy Block List (PBL), the owner can assign a different static IP address or remove the address from the PBL.</span></span>

- <span data-ttu-id="61ab4-109">За блокирани изходящи съобщения от домейна, свързан с Microsoft, можете да получите тази грешка, ако съобщенията са насочени през услуга на трета страна.</span><span class="sxs-lookup"><span data-stu-id="61ab4-109">For blocked outbound messages from your domain connected to Microsoft, you can receive this error if the messages are routed through a 3rd party service.</span></span> <span data-ttu-id="61ab4-110">Можете да използвате инструмент за търсене WHOIS да намерите блокиран ip адрес собственик.</span><span class="sxs-lookup"><span data-stu-id="61ab4-110">You can use a WHOIS lookup tool to find the blocked IP address owner.</span></span>
