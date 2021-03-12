---
title: Не можете да изпращате/получавате имейл до/от Office 365, тъй като е дезактивирано TLS 1,0 и TLS 1,1
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
ms.openlocfilehash: 9927112608ae58751e43c1bf0592fbd4a7cf1a0e
ms.sourcegitcommit: be246651064dfeacc866b2f69c0dbe4002a73f1c
ms.translationtype: MT
ms.contentlocale: bg-BG
ms.lasthandoff: 03/11/2021
ms.locfileid: "50743187"
---
# <a name="unable-to-sendreceive-email-tofrom-office-365-because-of-the-tls-10-and-tls-11-disablement"></a>Не можете да изпращате/получавате имейл до/от Office 365, тъй като е дезактивирано TLS 1,0 и TLS 1,1

Както е потвърдено от центъра за съобщения Post MC229914, TLS 1,0 и неодобрението на TLS 1,1 започва да прилага за крайни точки за пощенския поток за Exchange Online. Скоро Office 365 вече няма да приема TLS 1,0 и TLS 1,1 имейл връзки от външни източници. Освен това Exchange Online никога няма да използва TLS 1,0 или 1,1, за да изпраща изходящи имейли. Ако сте изправени пред проблеми поради TLS 1,0 или 1,1 за инвалидност, е възможно да се сблъскате с една от следните грешки:

- Подателят получава отскачане на NDR обратно-"421 4.4.2 връзката е спаднал поради SocketError"
- Грешка в визуализатора на опашката на локален сървър, който изпраща имейл до служител 365-"421 4.4.2 връзката е спаднал поради SocketError"
- Грешка при изпращане на [регистрационен файл на протокола](https://docs.microsoft.com/exchange/mail-flow/connectors/protocol-logging) за свързване на сървъра за изпращане на имейл до Office 365 – TLS неуспешно водене на преговори с грешка SocketError
- Грешка при изпращане или получаване на регистрационен файл на свързващия протокол – "451 5.7.3 трябва първо да издаде командата STARTTLS"

Ако имате някоя от горните грешки, се уверете, че сървърът, на който се изпращат или получават имейли, има активиран TLS 1,2, като отметнете следните ключове от системния регистър:

[HKEY_LOCAL_MACHINE\SYSTEM\CurrentControlSet\Control\SecurityProviders\SCHANNEL\Protocols\TLS 1,2] [HKEY_LOCAL_MACHINE\SYSTEM\CurrentControlSet\Control\SecurityProviders\SCHANNEL\Protocols\TLS 1.2 \ клиент] **"DisabledByDefault" = DWORD: 00000000 "активиран" = DWORD: 00000001** [HKEY_LOCAL_MACHINE\SYSTEM\CurrentControlSet\Control\SecurityProviders\SCHANNEL\Protocols\TLS 1.2 \ Server] **"DisabledByDefault" = DWORD: 00000000 "активиран" = DWORD: 00000001**

Ако направите промяна в горните ключове от системния регистър, за да разрешите TLS 1,2, рестартирайте сървъра, за да влязат в сила промените. Също така се уверете, че разполагате с най-новите актуализации за Windows и Exchange.

За повече информация вижте:

- [Ръководство за TLS за Exchange Server, част 1: подготовка за TLS 1,2 – общност на Microsoft Tech](https://techcommunity.microsoft.com/t5/exchange-team-blog/exchange-server-tls-guidance-part-1-getting-ready-for-tls-1-2/ba-p/607649)
- [Ориентиране на Exchange Server TLS част 2: разрешаване на TLS 1,2 и идентифициране на клиенти, които не го използват – общност на Microsoft Tech](https://techcommunity.microsoft.com/t5/exchange-team-blog/exchange-server-tls-guidance-part-2-enabling-tls-1-2-and/ba-p/607761)
- [Разберете сценариите за имейл, ако не могат да бъдат договорени версии на TLS с Exchange Online – общност на Microsoft Tech](https://techcommunity.microsoft.com/t5/exchange-team-blog/understanding-email-scenarios-if-tls-versions-cannot-be-agreed/ba-p/2065089)
