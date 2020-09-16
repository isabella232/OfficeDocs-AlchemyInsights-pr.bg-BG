---
title: Имате нужда от помощ за ограничения за изпращане на имейли?
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9002938"
- "5630"
ms.openlocfilehash: 66ff82afd7b44ef5fd4943bfc794c2fa35bbfa9e
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: bg-BG
ms.lasthandoff: 09/14/2020
ms.locfileid: "47702352"
---
# <a name="need-help-with-email-sending-limits"></a><span data-ttu-id="2def8-102">Имате нужда от помощ за ограничения за изпращане на имейли?</span><span class="sxs-lookup"><span data-stu-id="2def8-102">Need help with email sending limits?</span></span>

<span data-ttu-id="2def8-103">По-долу са наложените по **-долу ограничения за изпращане на проекти** в услугата.</span><span class="sxs-lookup"><span data-stu-id="2def8-103">Below is the **by-design sending limits** enforced in the service.</span></span> <span data-ttu-id="2def8-104">Повече информация за тези ограничения е документирана [тук](https://docs.microsoft.com/office365/servicedescriptions/exchange-online-service-description/exchange-online-limits#receiving-and-sending-limits).</span><span class="sxs-lookup"><span data-stu-id="2def8-104">More information on these limits is documented [here](https://docs.microsoft.com/office365/servicedescriptions/exchange-online-service-description/exchange-online-limits#receiving-and-sending-limits).</span></span>

- <span data-ttu-id="2def8-105">За да ограничите доставянето на незаявени групови съобщения, прилагаме **ограничения за процента на получателите за всички изходящи и вътрешни съобщения**.</span><span class="sxs-lookup"><span data-stu-id="2def8-105">To discourage the delivery of unsolicited bulk messages, we apply per-user **recipient rate limits to all outbound and internal messages**.</span></span> <span data-ttu-id="2def8-106">Във всички МСА това ограничение е **10 000 получатели на ден**.</span><span class="sxs-lookup"><span data-stu-id="2def8-106">Across all SKUs, this limit is **10,000 recipients per day**.</span></span>  <span data-ttu-id="2def8-107">Клиенти, които трябва да изпратят законна Групова търговска електронна поща (например бюлетини за клиенти), трябва да използват доставчици на трети страни, които са специализирани в тези услуги.</span><span class="sxs-lookup"><span data-stu-id="2def8-107">Customers who need to send legitimate bulk commercial email (for example, customer newsletters) should use third-party providers that specialize in these services.</span></span>
    - <span data-ttu-id="2def8-108">**Забележка**: след като ограничението за брой получатели бъде достигнато, не може да се изпращат съобщения от пощенската кутия, докато броят на получателите, на които са били изпратени съобщения в изминалите 24 часа, капки под ограничението.</span><span class="sxs-lookup"><span data-stu-id="2def8-108">**Note**: Once the recipient rate limit is reached, messages can't be sent from the mailbox until the number of recipients that were sent messages in the past 24 hours drops below the limit.</span></span> <span data-ttu-id="2def8-109">Потребителят няма да може да изпраща съобщения до този момент.</span><span class="sxs-lookup"><span data-stu-id="2def8-109">The user will not be able to send messages until that point.</span></span>
- <span data-ttu-id="2def8-110">Ограничение за размера на съобщенията от **30 съобщения в минута** се прилага във всички МСА.</span><span class="sxs-lookup"><span data-stu-id="2def8-110">Message rate limit of **30 messages per minute** is applied across all SKUs.</span></span> <span data-ttu-id="2def8-111">Това определя колко съобщения потребителят може да изпраща от своя акаунт за Exchange Online в определен период от време.</span><span class="sxs-lookup"><span data-stu-id="2def8-111">This determines how many messages a user can send from their Exchange Online account within a specified period.</span></span>
- <span data-ttu-id="2def8-112">**Максималният брой получатели, разрешени в полетата "до", "Як" и "СК** " за едно имейл съобщение, за всички ие е **1000 получатели**.</span><span class="sxs-lookup"><span data-stu-id="2def8-112">The **maximum number of recipients allowed in the To, Cc, and Bcc** fields for a single email message, across all SKUs, is **1000 recipients**.</span></span> <span data-ttu-id="2def8-113">За да персонализирате това ограничение, отидете [тук](https://techcommunity.microsoft.com/t5/exchange-team-blog/customizable-recipient-limits-in-office-365/ba-p/1183228).</span><span class="sxs-lookup"><span data-stu-id="2def8-113">To customize this limit, go [here](https://techcommunity.microsoft.com/t5/exchange-team-blog/customizable-recipient-limits-in-office-365/ba-p/1183228).</span></span>
