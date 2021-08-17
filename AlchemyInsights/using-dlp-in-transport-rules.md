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
ms.openlocfilehash: ebc0fb718eb0572e849c5d780977deaee480a00c2825c18a12e4d2212342f17a
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: bg-BG
ms.lasthandoff: 08/05/2021
ms.locfileid: "54084083"
---
# <a name="using-dlp-in-transport-rules"></a>Използване на DLP в транспортни правила

За да интегрирате защитата от загуба на данни (DLP) в съществуващ транспорт, използвайте условието "**Ако съобщението съдържа... Поверителна информация**"в настройката за транспортно правило.

**За повече подробности вижте:**

- Интегрирана информация за типовете поверителна информация в транспортните правила: [Интегриране на правилата за поверителна информация](https://docs.microsoft.com/exchange/security-and-compliance/data-loss-prevention/integrate-sensitive-information-rules).

Можете също да тествате правилото със или без проверка на правила, като използвате режим на проверка на правилото.  Трябва да изчакате 30 минути, след като сте създали правилото, преди да го тествате.

- Вижте [Тестване на пощенски поток/транспортни правила](https://docs.microsoft.com/exchange/security-and-compliance/mail-flow-rules/test-mail-flow-rules)

**Забележка**: Ако се опитвате да внедрите нова DLP политика с транспортни правила в EAC, вместо това използвайте [DLP правила в центъра за защита и съответствие](https://docs.microsoft.com/microsoft-365/compliance/data-loss-prevention-policies?view=o365-worldwide).
