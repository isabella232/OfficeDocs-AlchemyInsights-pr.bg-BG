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
ms.openlocfilehash: 425f9ba488fd69b8c5ea29636bccccd995bf48fd
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: bg-BG
ms.lasthandoff: 04/15/2021
ms.locfileid: "51815235"
---
# <a name="did-your-users-receive-malicious-email"></a>Потребителите ви получили ли са злонамерен имейл?

- Сега можете да съобщите за злонамерения имейл на Microsoft с помощта на подавания [на администратори в центъра за & съответствие.](https://sip.protection.office.com/reportsubmission)

Съобщенията, които са подадени в [подавания от администратор,](https://sip.protection.office.com/reportsubmission) се сканират и в допълнителната информация се показват **следните** резултати:

- Ако е имало грешка в удостоверяването на имейла на подателя към момента на доставянето.
- Информация за всички посещения на правила, които може да са засегнали или заместили решението на съобщението.
- Текущи резултати от детонацията, за да видите дали URL адресите или файловете, съдържащи се в съобщението, са злонамерени или не.
- Обратна връзка от класьори

Ако е намерено заместване, повторното сканиране трябва да завърши след няколко минути. Ако не е имало проблем в удостоверяването на имейл или ако доставянето не е било засегнато от заместване, обратната връзка от завършващите може да отнеме до един ден.

Ако не сте съгласни с окончателната присъда за съобщение, URL адрес или файл (блокирано спрямо блокирано, не е блокирано), изпратете съобщението отново след един ден за повторно сканиране. Шансовете са високи, че решението ще се промени след изпращането на съобщението отново.

Междувременно можете да премахнете злонамерените имейли от потребителските входящи, като следвате инструкциите в [тази статия.](https://docs.microsoft.com/microsoft-365/compliance/search-for-and-delete-messages-in-your-organization)

- Клиентите с Microsoft Defender за Office 365 могат:
    - използване на [Threat Explorer за намиране и изтриване на подозрителни имейли](https://docs.microsoft.com/microsoft-365/security/office-365-security/investigate-malicious-email-that-was-delivered)
    - [използване на безопасни връзки за блокиране на достъпа](https://docs.microsoft.com/microsoft-365/security/office-365-security/atp-safe-links) до злонамерен URL адрес
    - проследяване на потребители, които са щракнали и са осъществявали достъп до злонамерени URL адреси: Преглед на URL адрес за фишинг и щракване върху [пресъдени данни](https://docs.microsoft.com/microsoft-365/security/office-365-security/threat-explorer)  &  [Get-UrlTrace](https://docs.microsoft.com/powershell/module/exchange/get-urltrace)
    - ръчно [стартиране на автоматизирано разследване](https://docs.microsoft.com/microsoft-365/security/office-365-security/automated-investigation-response-office)

Можете също да защитите от злонамерени файлове и URL адреси, като следвате инструкциите в [Защита от злонамерени URL адреси и файлове.](https://docs.microsoft.com/microsoft-365/security/office-365-security/protect-against-threats)