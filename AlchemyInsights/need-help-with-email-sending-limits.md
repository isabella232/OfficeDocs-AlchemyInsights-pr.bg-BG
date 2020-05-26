---
title: Нуждаете се от помощ с ограниченията за изпращане на имейли?
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9002938"
- "5630"
ms.openlocfilehash: 7f563df313c869d18c3e4240d271c649a74914af
ms.sourcegitcommit: 88d2918aa51f4ba10771527380c3e0db0f5a9147
ms.translationtype: MT
ms.contentlocale: bg-BG
ms.lasthandoff: 05/20/2020
ms.locfileid: "44357327"
---
# <a name="need-help-with-email-sending-limits"></a><span data-ttu-id="a2c42-102">Нуждаете се от помощ с ограниченията за изпращане на имейли?</span><span class="sxs-lookup"><span data-stu-id="a2c42-102">Need help with email sending limits?</span></span>

<span data-ttu-id="a2c42-103">По-долу са **лимитите** за изпращане на проекта, наложени в услугата.</span><span class="sxs-lookup"><span data-stu-id="a2c42-103">Below is the **by-design sending limits** enforced in the service.</span></span> <span data-ttu-id="a2c42-104">Повече информация за тези ограничения е документирана [тук](https://docs.microsoft.com/office365/servicedescriptions/exchange-online-service-description/exchange-online-limits#receiving-and-sending-limits).</span><span class="sxs-lookup"><span data-stu-id="a2c42-104">More information on these limits is documented [here](https://docs.microsoft.com/office365/servicedescriptions/exchange-online-service-description/exchange-online-limits#receiving-and-sending-limits).</span></span>

- <span data-ttu-id="a2c42-105">За да се предотврати предоставянето на нежелани масови съобщения, ние прилагаме ограничения за процента на **получателите на всички изходящи и вътрешни съобщения.**</span><span class="sxs-lookup"><span data-stu-id="a2c42-105">To discourage the delivery of unsolicited bulk messages, we apply per-user **recipient rate limits to all outbound and internal messages**.</span></span> <span data-ttu-id="a2c42-106">За всички Sku този лимит е **10 000 получатели на ден.**</span><span class="sxs-lookup"><span data-stu-id="a2c42-106">Across all SKUs, this limit is **10,000 recipients per day**.</span></span>  <span data-ttu-id="a2c42-107">Клиентите, които трябва да изпращат наедро търговски имейл (например клиентски бюлетини) трябва да използват доставчици на трети страни, които са специализирани в тези услуги.</span><span class="sxs-lookup"><span data-stu-id="a2c42-107">Customers who need to send legitimate bulk commercial email (for example, customer newsletters) should use third-party providers that specialize in these services.</span></span>
    - <span data-ttu-id="a2c42-108">**Забележка:** След като се достигне ограничението на скоростта на получателя, съобщенията не могат да бъдат изпратени от пощенската кутия, докато броят на получателите, изпратени съобщения в последните 24 часа не падне под ограничението.</span><span class="sxs-lookup"><span data-stu-id="a2c42-108">**Note**: Once the recipient rate limit is reached, messages can't be sent from the mailbox until the number of recipients that were sent messages in the past 24 hours drops below the limit.</span></span> <span data-ttu-id="a2c42-109">Потребителят няма да може да изпраща съобщения до тази точка.</span><span class="sxs-lookup"><span data-stu-id="a2c42-109">The user will not be able to send messages until that point.</span></span>
- <span data-ttu-id="a2c42-110">Ограничението за скорост на съобщенията от **30 съобщения в минута** се прилага за всички sku.</span><span class="sxs-lookup"><span data-stu-id="a2c42-110">Message rate limit of **30 messages per minute** is applied across all SKUs.</span></span> <span data-ttu-id="a2c42-111">Това определя колко съобщения потребителят може да изпрати от своя акаунт в Exchange Online в определен период.</span><span class="sxs-lookup"><span data-stu-id="a2c42-111">This determines how many messages a user can send from their Exchange Online account within a specified period.</span></span>
- <span data-ttu-id="a2c42-112">**Максималният брой получатели, позволен в полетата До, Як и Ск** за едно имейл съобщение, във всички SKUs, е **1000 получатели.**</span><span class="sxs-lookup"><span data-stu-id="a2c42-112">The **maximum number of recipients allowed in the To, Cc, and Bcc** fields for a single email message, across all SKUs, is **1000 recipients**.</span></span> <span data-ttu-id="a2c42-113">За да персонализирате този лимит, отидете [тук](https://techcommunity.microsoft.com/t5/exchange-team-blog/customizable-recipient-limits-in-office-365/ba-p/1183228).</span><span class="sxs-lookup"><span data-stu-id="a2c42-113">To customize this limit, go [here](https://techcommunity.microsoft.com/t5/exchange-team-blog/customizable-recipient-limits-in-office-365/ba-p/1183228).</span></span>
