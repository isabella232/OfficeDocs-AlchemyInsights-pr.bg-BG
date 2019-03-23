---
title: Грешка при изпращане на имейл, блокирани от SpamHaus
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 2/23/2018
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: fa98ab4a-92eb-45e9-8d57-ad10fb123042
ms.openlocfilehash: 7d6ad2667613ae948a4abcefafe8d91cf89d2418
ms.sourcegitcommit: 03a156a9c9740521155a30775492c7dff0982588
ms.translationtype: MT
ms.contentlocale: bg-BG
ms.lasthandoff: 03/22/2019
ms.locfileid: "30761622"
---
# <a name="error-sending-email-client-host-blocked-using-spamhaus"></a><span data-ttu-id="cac70-102">Грешка при изпращане на имейл: клиент домакин блокирани използване Spamhaus</span><span class="sxs-lookup"><span data-stu-id="cac70-102">Error sending email: Client host blocked using Spamhaus</span></span>

<span data-ttu-id="cac70-103">IP адреса, който е изпратил съобщението е в списък за блокиране, собственост на [Spamhaus](https://go.microsoft.com/fwlink/p/?linkid=123245).</span><span class="sxs-lookup"><span data-stu-id="cac70-103">The IP address that sent the message is on a block list owned by [Spamhaus](https://go.microsoft.com/fwlink/p/?linkid=123245).</span></span> <span data-ttu-id="cac70-104">Причини за блокирано от Spamhaus включват компрометирана сметки, компрометирани машини споделяне публичен IP адрес, както и интернет доставчик (ISP) политики.</span><span class="sxs-lookup"><span data-stu-id="cac70-104">Reasons for being blocked by Spamhaus include compromised accounts, compromised machines sharing a public IP address, and Internet Service Provider (ISP) policies.</span></span> <span data-ttu-id="cac70-105">Възможни корекции са:</span><span class="sxs-lookup"><span data-stu-id="cac70-105">Possible fixes are:</span></span>
  
- <span data-ttu-id="cac70-106">За блокираните входящите съобщения в Office 365, където можете да контролирате източник имейл сървър трябва да се определи причината и премахнете блок от сайта на Spamhaus.</span><span class="sxs-lookup"><span data-stu-id="cac70-106">For blocked inbound messages to Office 365 where you control the source email server, you need to determine the cause and remove the block from the Spamhaus website.</span></span>
    
- <span data-ttu-id="cac70-107">За блокираните входящите съобщения в Office 365, където изходният IP адрес принадлежи на някой друг собственика на адреса трябва да премахнете блок от сайта на Spamhaus.</span><span class="sxs-lookup"><span data-stu-id="cac70-107">For blocked inbound messages to Office 365 where the source IP address belongs to someone else, the address owner needs to remove the block from the Spamhaus website.</span></span> <span data-ttu-id="cac70-108">Ако IP адресът е в политиката блок списък (PBL), собственикът може да присвоите различни статичен IP адрес или премахнете адреса от PBL.</span><span class="sxs-lookup"><span data-stu-id="cac70-108">If the IP address is on the Policy Block List (PBL), the owner can assign a different static IP address or remove the address from the PBL.</span></span>
    
- <span data-ttu-id="cac70-109">За блокирани изходящи съобщения от вашия домейн на Office 365 можете да получавате тази грешка, ако съобщенията се насочват чрез 3-та страна услуга.</span><span class="sxs-lookup"><span data-stu-id="cac70-109">For blocked outbound messages from your Office 365 domain, you can receive this error if the messages are routed through a 3rd party service.</span></span> <span data-ttu-id="cac70-110">Можете да използвате инструмента за търсене WHOIS да намерите собственика на блокираните IP адрес.</span><span class="sxs-lookup"><span data-stu-id="cac70-110">You can use a WHOIS lookup tool to find the blocked IP address owner.</span></span>
    

