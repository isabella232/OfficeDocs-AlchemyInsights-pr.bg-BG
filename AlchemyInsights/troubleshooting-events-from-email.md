---
title: Отстраняване на неизправности със събития от имейл
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
- "9000301"
- "5765"
ms.openlocfilehash: b6a8b2a1174f04a1e0ed0fdee9a954bb3bf108038f0804353d84755e490f5f47
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: bg-BG
ms.lasthandoff: 08/05/2021
ms.locfileid: "54105341"
---
# <a name="troubleshooting-events-from-email"></a>Отстраняване на неизправности със събития от имейл

1. Проверка на функцията е разрешена за пощенската кутия: **Get-EventsFromEmailConfiguration -Identity <mailbox>**

2. След това погледнете регистрационните файлове "Събития от имейл" **Експортиране-MailboxDiagnosticLogs <mailbox> -Component TimeProfile**

3. В регистрационните файлове "Събития от имейл" намерете InternetMessageId, който отговаря на елемента в пощенската кутия.  

4. TrustScore определя дали елементът е добавен или не. Събития ще се добавят само ако TrustScore = "Trusted".

TrustScore се определя от свойствата SPF, Dkim или Dmarc, които са в заглавката на съобщението.

За да видите тези свойства:

**Настолни Outlook**

- Отваряне на елемента
- Свойства на > –> интернет заглавки

или

**MFCMapi**

- Навигиране до елемента в папката "Входящи"
- Потърсете PR_TRANSPORT_MESSAGE_HEADERS_W

Тези свойства се определят и записват по време на транспорт и маршрутизиране. За по-нататъшно отстраняване на неизправности може да се наложи да следвате транспортната поддръжка за неизправностите в SPF, DKIM и.or DMARC.