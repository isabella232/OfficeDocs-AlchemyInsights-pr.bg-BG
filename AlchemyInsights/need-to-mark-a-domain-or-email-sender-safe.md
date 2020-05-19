---
title: Трябва да маркирате домейн или имейл подател безопасно?
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9002921"
- "5673"
ms.openlocfilehash: 7dc1576fd61e87b319c7486c59ed125943b4d959
ms.sourcegitcommit: 43acdecef129bfffc8bbe8ebb08fdd581b238a03
ms.translationtype: MT
ms.contentlocale: bg-BG
ms.lasthandoff: 05/18/2020
ms.locfileid: "44281119"
---
# <a name="need-to-mark-a-domain-or-email-sender-safe"></a>Трябва да маркирате домейн или имейл подател безопасно?

- Не се препоръчва използването на **списъци с безопасни податели,** тъй като тя отваря вашата организация за нежелана, фиш и подправяне на атаки.
- Ако обаче има бизнес изискване, **препоръчваме да** използвате за това **[правилата за пощенски поток.](https://docs.microsoft.com/microsoft-365/security/office-365-security/create-safe-sender-lists-in-office-365?view=o365-worldwide#recommended-use-mail-flow-rules)** Нашите указания гарантират удостоверяване на изпращача (проверява изпращане на домейн не се подмества). **Забележка:** Не препоръчваме да управлявате фалшиви положителни резултати чрез списъци на безопасни податели, защото изключенията при филтрирането на нежелана информация могат да отворят организацията ви за атаки на защитата. Ако вашите потребители получават съобщения, неправилно маркирани като спам или нежелана поща, **[моля, изпратете съобщение до Microsoft](https://protection.office.com/reportsubmission)**.
- Безопасните податели в Outlook, разрешен списък с податели или разрешен списък с домейни в анти-спам политики **трябва да се избягва,** защото подателите заобикалят всички спам, измамни и фиш защита и удостоверяване на подателя (SPF, DKIM, DMARC). Този метод се използва най-добре само за временно тестване.
