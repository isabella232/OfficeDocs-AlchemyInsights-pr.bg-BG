---
title: Трябва да маркирате домейн или имейл подател в безопасност?
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
- "9002921"
- "5673"
ms.openlocfilehash: a1c4c4d2fadaf75eda9b5b322aca35c32dfee8ea
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: bg-BG
ms.lasthandoff: 04/15/2021
ms.locfileid: "51792121"
---
# <a name="need-to-mark-a-domain-or-email-sender-safe"></a>Трябва да маркирате домейн или имейл подател в безопасност?

- Използването на **списъци с безопасни податели не** се препоръчва, тъй като отваря вашата организация за нежелана поща, фишинг и измамни атаки.
- Ако обаче има бизнес изискване, ви препоръчваме да използвате **правила** за **[пощенски поток](https://docs.microsoft.com/microsoft-365/security/office-365-security/create-safe-sender-lists-in-office-365?view=o365-worldwide#recommended-use-mail-flow-rules)** за това. Нашите указания гарантират удостоверяване на подателя (проверява, че домейнът за изпращане не се подпрагва). **Забележка:** Не препоръчваме да управлявате грешни положителни резултати с помощта на списъци с безопасни податели, тъй като изключенията от филтрирането на нежелана поща могат да отворят вашата организация за атаки на защитата. Ако вашите потребители получават съобщения, неправилно маркирани като нежелана поща или нежелана поща, **[докладвайте за съобщения и файлове на Microsoft](https://protection.office.com/reportsubmission)**.
- Безопасните податели в Outlook, списъка с разрешени податели или разрешените домейни в правилата за нежелана поща трябва да се избягват, защото подателите заобикалят всички нежелана поща, подлост и фиш защита и удостоверяване на подателя (SPF, DKIM, DMARC).  Този метод се използва най-добре само за временно тестване.
