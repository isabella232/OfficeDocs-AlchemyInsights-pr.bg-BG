---
title: Имате нужда от помощ за ограниченията за изпращане на имейли?
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9002938"
- "5630"
ms.openlocfilehash: b5bdfbf818328c97ec93b3468aeedcbe88e03913
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: bg-BG
ms.lasthandoff: 04/15/2021
ms.locfileid: "51836268"
---
# <a name="need-help-with-email-sending-limits"></a><span data-ttu-id="8a40c-102">Имате нужда от помощ за ограниченията за изпращане на имейли?</span><span class="sxs-lookup"><span data-stu-id="8a40c-102">Need help with email sending limits?</span></span>

<span data-ttu-id="8a40c-103">**По-долу са наложени ограниченията за изпращане по** проект в услугата.</span><span class="sxs-lookup"><span data-stu-id="8a40c-103">Below is the **by-design sending limits** enforced in the service.</span></span> <span data-ttu-id="8a40c-104">Повече информация за тези ограничения е документирана [тук.](https://docs.microsoft.com/office365/servicedescriptions/exchange-online-service-description/exchange-online-limits#receiving-and-sending-limits)</span><span class="sxs-lookup"><span data-stu-id="8a40c-104">More information on these limits is documented [here](https://docs.microsoft.com/office365/servicedescriptions/exchange-online-service-description/exchange-online-limits#receiving-and-sending-limits).</span></span>

- <span data-ttu-id="8a40c-105">За да предотвратим доставянето на нежелани групови съобщения, прилагаме ограничения за ставката за всеки потребител за **всички изходящи и вътрешни съобщения.**</span><span class="sxs-lookup"><span data-stu-id="8a40c-105">To discourage the delivery of unsolicited bulk messages, we apply per-user **recipient rate limits to all outbound and internal messages**.</span></span> <span data-ttu-id="8a40c-106">За всички МКИ това ограничение е **10 000 получатели на ден.**</span><span class="sxs-lookup"><span data-stu-id="8a40c-106">Across all SKUs, this limit is **10,000 recipients per day**.</span></span>  <span data-ttu-id="8a40c-107">Клиентите, които трябва да изпращат легитимен групов търговски имейл (например клиентски бюлетини), трябва да използват доставчици на трети страни, които са специализирани в тези услуги.</span><span class="sxs-lookup"><span data-stu-id="8a40c-107">Customers who need to send legitimate bulk commercial email (for example, customer newsletters) should use third-party providers that specialize in these services.</span></span>
    - <span data-ttu-id="8a40c-108">**Забележка:** След като достигне ограничението за ставката на получателя, съобщенията не могат да се изпращат от пощенската кутия, докато броят на получателите, които са изпратени съобщения през последните 24 часа, не падне под ограничението.</span><span class="sxs-lookup"><span data-stu-id="8a40c-108">**Note**: Once the recipient rate limit is reached, messages can't be sent from the mailbox until the number of recipients that were sent messages in the past 24 hours drops below the limit.</span></span> <span data-ttu-id="8a40c-109">Потребителят няма да може да изпраща съобщения до този момент.</span><span class="sxs-lookup"><span data-stu-id="8a40c-109">The user will not be able to send messages until that point.</span></span>
- <span data-ttu-id="8a40c-110">Ограничението за скоростта на **съобщението от 30 съобщения в** минута се прилага за всички МКИ.</span><span class="sxs-lookup"><span data-stu-id="8a40c-110">Message rate limit of **30 messages per minute** is applied across all SKUs.</span></span> <span data-ttu-id="8a40c-111">Това определя колко съобщения може да изпраща потребителят от своя акаунт за Exchange Online в рамките на определен период от време.</span><span class="sxs-lookup"><span data-stu-id="8a40c-111">This determines how many messages a user can send from their Exchange Online account within a specified period.</span></span>
- <span data-ttu-id="8a40c-112">Максималният брой получатели, разрешени в полетата **До, Як** и Ск за едно имейл съобщение, във всички skUs, е **1000 получатели.**</span><span class="sxs-lookup"><span data-stu-id="8a40c-112">The **maximum number of recipients allowed in the To, Cc, and Bcc** fields for a single email message, across all SKUs, is **1000 recipients**.</span></span> <span data-ttu-id="8a40c-113">За да персонализирате това ограничение, [отидете тук](https://techcommunity.microsoft.com/t5/exchange-team-blog/customizable-recipient-limits-in-office-365/ba-p/1183228).</span><span class="sxs-lookup"><span data-stu-id="8a40c-113">To customize this limit, go [here](https://techcommunity.microsoft.com/t5/exchange-team-blog/customizable-recipient-limits-in-office-365/ba-p/1183228).</span></span>
