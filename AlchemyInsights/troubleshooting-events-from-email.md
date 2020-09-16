---
title: Отстраняване на неизправности при събития от имейл
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
- "9000301"
- "5765"
ms.openlocfilehash: 9efd969e3e639c2679b0768c4a0fd045916b00d1
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: bg-BG
ms.lasthandoff: 09/14/2020
ms.locfileid: "47658723"
---
# <a name="troubleshooting-events-from-email"></a>Отстраняване на неизправности при събития от имейл

1. Проверете дали тази функция е разрешена за пощенската кутия: **get <mailbox> -EventsFromEmailConfiguration-самоличност**

2. След това погледнете "събития от имейл" регистрационни файлове за **експортиране – MailboxDiagnosticLogs <mailbox> – Component TimeProfile**

3. В регистрите "събития от имейл" Намерете свойството InternetMessageId, което съответства на елемента в пощенската кутия.  

4. Свойството TrustScore определя дали елементът е добавен, или не. Събития ще бъдат добавени само ако TrustScore = "доверен".

Свойството TrustScore се определя чрез SPF, DKIM или dMarc свойства, които са в заглавката на съобщението.

За да видите тези свойства:

**Настолна версия на Outlook**

- Отваряне на елемента
- Свойства на > на файл – > интернет заглавки

или

**MFCMapi**

- Придвижете се до елемента в папката "Входящи"
- Потърсете PR_TRANSPORT_MESSAGE_HEADERS_W

Тези свойства се определят и записват по време на транспорта и маршрутизирането. За по-нататъшно отстраняване на неизправности може да се наложи да се придържате към поддръжката на транспорта за неуспехите в SPF, DKIM и. or DMARC.