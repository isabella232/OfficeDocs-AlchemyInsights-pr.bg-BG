---
title: Използване на DLP в транспортни правила
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9002635"
- "5153"
ms.openlocfilehash: 124b031e2e029b745c66a71f681f57134739eafe
ms.sourcegitcommit: 07725fcaf073f0ac145f98653b989afdb34c5ad0
ms.translationtype: HT
ms.contentlocale: bg-BG
ms.lasthandoff: 04/28/2020
ms.locfileid: "43915020"
---
# <a name="using-dlp-in-transport-rules"></a>Използване на DLP в транспортни правила

За да интегрирате защитата от загуба на данни (DLP) в съществуващ транспорт, използвайте условието "**Ако съобщението съдържа... Поверителна информация**"в настройката за транспортно правило.

**За повече подробности вижте:**

- Интегрирана информация за типовете поверителна информация в транспортните правила: [Интегриране на правилата за поверителна информация](https://docs.microsoft.com/exchange/security-and-compliance/data-loss-prevention/integrate-sensitive-information-rules).

Можете също да тествате правилото със или без проверка на правила, като използвате режим на проверка на правилото.  Трябва да изчакате 30 минути, след като сте създали правилото, преди да го тествате.

- Вижте [Тестване на пощенски поток/транспортни правила](https://docs.microsoft.com/exchange/security-and-compliance/mail-flow-rules/test-mail-flow-rules)

**Забележка**: Ако се опитвате да внедрите нова DLP политика с транспортни правила в EAC, вместо това използвайте [DLP правила в центъра за защита и съответствие](https://docs.microsoft.com/microsoft-365/compliance/data-loss-prevention-policies?view=o365-worldwide).
