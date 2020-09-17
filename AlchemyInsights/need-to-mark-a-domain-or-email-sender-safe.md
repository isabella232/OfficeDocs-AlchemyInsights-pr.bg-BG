---
title: Трябва да маркирате безопасен домейн или имейл подател?
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
- "9002921"
- "5673"
ms.openlocfilehash: 0ea089b95ad7de25e77017196fb2db895d4d0178
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: bg-BG
ms.lasthandoff: 09/15/2020
ms.locfileid: "47803234"
---
# <a name="need-to-mark-a-domain-or-email-sender-safe"></a>Трябва да маркирате безопасен домейн или имейл подател?

- Използването на **списъци с безопасни податели не се препоръчва** , тъй като отваря вашата организация за нежелана поща, фишинг и измамнически атаки.
- Ако обаче има бизнес изискване, **ви препоръчваме** да използвате правилата за **[пощенския поток](https://docs.microsoft.com/microsoft-365/security/office-365-security/create-safe-sender-lists-in-office-365?view=o365-worldwide#recommended-use-mail-flow-rules)** за това. Нашите указания гарантират удостоверяване на подателя (проверява дали изпращането на домейни не е фалшифицирано). **Забележка**: не препоръчваме управление на неверни положителни резултати с помощта на списъци с безопасни податели, тъй като изключенията за филтриране на нежелана поща могат да отворят вашата организация за атаки по защитата. Ако вашите потребители получават съобщения, които са неправилно маркирани като спам или нежелана поща, **[съобщете за съобщения и файлове на Microsoft](https://protection.office.com/reportsubmission)**.
- Безопасните податели в Outlook, списъка с разрешени податели или разрешените домейни в правила за нежелана поща **трябва да бъдат избегнати** , тъй като подателите заобикалят всички нежелани съобщения, пародия и защита на подателя и удостоверяването на изпращача (SPF, DKIM, DMARC). Този метод се използва най-добре само за временен тест.
