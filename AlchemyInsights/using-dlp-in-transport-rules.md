---
title: Използване на DLP в транспортни правила
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
- "9002635"
- "5153"
ms.openlocfilehash: e512b36b34c5fc4931fb0f796790ee4b01c6443c
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: bg-BG
ms.lasthandoff: 04/15/2021
ms.locfileid: "51827205"
---
# <a name="using-dlp-in-transport-rules"></a><span data-ttu-id="b4ba9-102">Използване на DLP в транспортни правила</span><span class="sxs-lookup"><span data-stu-id="b4ba9-102">Using DLP in transport rules</span></span>

<span data-ttu-id="b4ba9-103">За да интегрирате защитата от загуба на данни (DLP) в съществуващ транспорт, използвайте условието "**Ако съобщението съдържа... Поверителна информация**"в настройката за транспортно правило.</span><span class="sxs-lookup"><span data-stu-id="b4ba9-103">To integrate Data Loss Prevention (DLP) into an existing transport, use the condition "**If the message contains...Sensitive Information**" in the Transport rule setting.</span></span>

<span data-ttu-id="b4ba9-104">**За повече подробности вижте:**</span><span class="sxs-lookup"><span data-stu-id="b4ba9-104">**For more details, see:**</span></span>

- <span data-ttu-id="b4ba9-105">Интегрирана информация за типовете поверителна информация в транспортните правила: [Интегриране на правилата за поверителна информация](https://docs.microsoft.com/exchange/security-and-compliance/data-loss-prevention/integrate-sensitive-information-rules).</span><span class="sxs-lookup"><span data-stu-id="b4ba9-105">Integrated DLP sensitive information types in transport rules: [Integrate Sensitive Information Rules](https://docs.microsoft.com/exchange/security-and-compliance/data-loss-prevention/integrate-sensitive-information-rules).</span></span>

<span data-ttu-id="b4ba9-106">Можете също да тествате правилото със или без проверка на правила, като използвате режим на проверка на правилото.</span><span class="sxs-lookup"><span data-stu-id="b4ba9-106">You can also test the rule with or without policy test using Test Mode on the rule.</span></span>  <span data-ttu-id="b4ba9-107">Трябва да изчакате 30 минути, след като сте създали правилото, преди да го тествате.</span><span class="sxs-lookup"><span data-stu-id="b4ba9-107">You should wait 30 mins after creating the rule before testing it.</span></span>

- <span data-ttu-id="b4ba9-108">Вижте [Тестване на пощенски поток/транспортни правила](https://docs.microsoft.com/exchange/security-and-compliance/mail-flow-rules/test-mail-flow-rules)</span><span class="sxs-lookup"><span data-stu-id="b4ba9-108">See [Test Mail Flow/Transport rules](https://docs.microsoft.com/exchange/security-and-compliance/mail-flow-rules/test-mail-flow-rules)</span></span>

<span data-ttu-id="b4ba9-109">**Забележка**: Ако се опитвате да внедрите нова DLP политика с транспортни правила в EAC, вместо това използвайте [DLP правила в центъра за защита и съответствие](https://docs.microsoft.com/microsoft-365/compliance/data-loss-prevention-policies?view=o365-worldwide).</span><span class="sxs-lookup"><span data-stu-id="b4ba9-109">**Note**: If you are trying to implement a new DLP policy with transport rules in the EAC, use [DLP Policies in the Security and Compliance center](https://docs.microsoft.com/microsoft-365/compliance/data-loss-prevention-policies?view=o365-worldwide) instead.</span></span>
