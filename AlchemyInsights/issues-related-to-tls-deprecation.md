---
title: Не може да се изпрати/получи имейл до/от Office 365 поради TLS 1.0 и TLS 1.1 забраняване
ms.author: v-jmathew
author: v-jmathew
manager: scotv
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9005383"
- "9275"
ms.openlocfilehash: 508e48fd0e46557de075f4752da017ab8cc326923a965350140e598f7f7cf557
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: bg-BG
ms.lasthandoff: 08/05/2021
ms.locfileid: "54054895"
---
# <a name="unable-to-sendreceive-email-tofrom-office-365-because-of-the-tls-10-and-tls-11-disablement"></a>Не може да се изпрати/получи имейл до/от Office 365 поради TLS 1.0 и TLS 1.1 забраняване

Както е потвърдено от центъра за съобщения след MC229914, TLS 1,0 и TLS 1,1 отричаването започна да се извършва за крайни точки Exchange Online пощенския поток. Скоро Office 365 вече няма да приема TLS 1.0 и TLS 1.1 имейл връзки от външни източници. Освен това Exchange Online никога няма да използват TLS 1.0 или 1.1 за изпращане на изходящи имейли. Ако имате проблеми поради TLS 1.0 или 1.1 дезактивиране, може да изпитате една от следните грешки:

- Подателят връща отпадането на NDR – '421 4.4.2 Връзката е прекъсната поради SocketError
- Грешка в визуализатора на опашки на локалния сървър, който изпраща имейл до служител 365 – "421 4.4.2 Връзката е прекъсната поради SocketError"
- Грешка в регистрационния файл за [протокола за изпращане на](https://docs.microsoft.com/exchange/mail-flow/connectors/protocol-logging) конектори на сървъра, изпращащ имейл до Office 365- TLS договарянето е неуспешно с грешка SocketError
- Грешка в регистрационния файл на протокола за изпращане или получаване – '451 5.7.3 Първо трябва да издаде команда STARTTLS

Ако имате някоя от горните грешки, уверете се, че сървърът, който изпраща или получава имейл, има TLS 1.2 разрешен, като проверите следните ключове от системния регистър:

[HKEY_LOCAL_MACHINE\SYSTEM\CurrentControlSet\Control\SecurityProviders\SCHANNEL\Protocols\TLS 1,2] [HKEY_LOCAL_MACHINE\SYSTEM\CurrentControlSet\Control\SecurityProviders\SCHANNEL\Protocols\TLS 1,2\Client] **"DisabledByDefault"=dword:00000000 "Enabled"=dword:00000001** [HKEY_LOCAL_MACHINE\SYSTEM\CurrentControlSet\Control\SecurityProviders\SCHANNEL\Protocols\TLS 1,2\Server] **"DisabledByDefault"=dword:00000000 "Enabled"=dword:00000001**

Ако направите промяна в горните ключове на системния регистър, за да разрешите TLS 1.2, рестартирайте сървъра, за да влязат в сила промените. Също така се уверете, че имате инсталирани най-новите Windows и Exchange актуализации.

За повече информация вижте:

- [Exchange Server Насоки за TLS, част 1: Готови за TLS 1.2 – Техническа общност на Microsoft](https://techcommunity.microsoft.com/t5/exchange-team-blog/exchange-server-tls-guidance-part-1-getting-ready-for-tls-1-2/ba-p/607649)
- [Exchange Server TLS указания част 2: Разрешаване на TLS 1.2 и идентифициране на клиенти, които не го използват – техническа общност на Microsoft](https://techcommunity.microsoft.com/t5/exchange-team-blog/exchange-server-tls-guidance-part-2-enabling-tls-1-2-and/ba-p/607761)
- [Разбиране на сценариите за имейл, ако версиите на TLS не могат да бъдат съгласувани с Exchange Online – техническа общност на Microsoft](https://techcommunity.microsoft.com/t5/exchange-team-blog/understanding-email-scenarios-if-tls-versions-cannot-be-agreed/ba-p/2065089)
