---
title: Потребителите ви получавали ли са злонамерени имейли
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
- "9002907"
- "5594"
- "3100017"
- "2578"
ms.openlocfilehash: 525af0b29ffa291ddf69f6f2d97f505e93342989
ms.sourcegitcommit: ab75f66355116e995b3cb5505465b31989339e28
ms.translationtype: MT
ms.contentlocale: bg-BG
ms.lasthandoff: 08/13/2021
ms.locfileid: "58326647"
---
# <a name="did-your-users-receive-malicious-email"></a>Потребителите ви получили ли са злонамерен имейл?

Сега можете да съобщите за злонамерения имейл на Microsoft [с помощта на "Подавания" Microsoft 365 Defender портала.](https://sip.security.microsoft.com/reportsubmission?viewid=admin)

Съобщенията, които са подадени в [подавания от](https://security.microsoft.com/reportsubmission?viewid=admin) администратор, се сканират и се показват следните резултати в подробното листовка:

- Ако е имало грешка в удостоверяването на имейла на подателя към момента на доставянето.
- Информация за всички посещения на правила, които може да са засегнали или заместили решението на съобщението.
- Текущи резултати от детонацията, за да видите дали URL адресите или файловете, съдържащи се в съобщението, са злонамерени или не.
- Обратна връзка от класьори

Ако е намерено заместване, повторното сканиране трябва да завърши след няколко минути. Ако няма проблем в удостоверяването на имейл или ако доставянето не е било засегнато от заместване, обратната връзка от завършващите може да отнеме до един ден.

Ако не сте съгласни с окончателната присъда за съобщение, URL адрес или файл (блокирано спрямо блокирано, не е блокирано), изпратете съобщението отново след ден за повторно сканиране. Шансовете са високи, че решението ще се промени след повторното изпращане на съобщението.

Междувременно можете да премахнете злонамерените имейли от потребителските входящи, като следвате инструкциите в [тази статия.](https://docs.microsoft.com/microsoft-365/compliance/search-for-and-delete-messages-in-your-organization)

- Клиентите с Microsoft Defender за Office 365 могат да:
  - Използване на [Threat Explorer за намиране и изтриване на подозрителни имейли](https://docs.microsoft.com/microsoft-365/security/office-365-security/investigate-malicious-email-that-was-delivered)
  - [Използване Сейф връзки за блокиране на достъпа](https://docs.microsoft.com/microsoft-365/security/office-365-security/safe-links) до злонамерен URL адрес
  - Проследяване на потребители, които са щракнали и са осъществявали достъп до злонамерени URL адреси: Преглед на URL адреса за фишинг и щракване върху [пресъдени данни](https://docs.microsoft.com/microsoft-365/security/office-365-security/threat-explorer)  &  [Get-UrlTrace](https://docs.microsoft.com/powershell/module/exchange/get-urltrace)
  - Ръчно [стартиране на автоматизирано разследване](https://docs.microsoft.com/microsoft-365/security/office-365-security/automated-investigation-response-office)

Можете също да защитите от злонамерени файлове и URL адреси, като следвате инструкциите в [Защита от злонамерени URL адреси и файлове.](https://docs.microsoft.com/microsoft-365/security/office-365-security/protect-against-threats)
