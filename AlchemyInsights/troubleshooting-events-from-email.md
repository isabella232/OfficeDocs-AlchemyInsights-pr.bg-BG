---
title: Отстраняване на неизправности при събития от имейл
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9000301"
- "5765"
ms.openlocfilehash: e27589b7f6730036040b948b6275cef072fd8235
ms.sourcegitcommit: dc149ab45fbc2c974b54fb81156d2bc1b07017bb
ms.translationtype: MT
ms.contentlocale: bg-BG
ms.lasthandoff: 06/02/2020
ms.locfileid: "44568907"
---
# <a name="troubleshooting-events-from-email"></a>Отстраняване на неизправности при събития от имейл

1. Проверете функцията е разрешена за пощенска кутия: **Get-EventsFromEmailConfiguration -самоличност <mailbox> **

2. След това погледнете "Събития от имейл" регистрационни файлове **експортиране-пощенска кутияDiagnosticLogs-Component <mailbox> TimeProfile**

3. В регистрационните файлове "Събития от имейл" намерете InternetMessageId, който отговаря на елемента в пощенската кутия.  

4. В TrustScore се определя дали елементът е добавен или не. Събитията ще бъдат добавени само ако доверителният талона = "Надежден".

TrustScore се определя от SPF, Dkim или Dmarc свойства, които са в заглавната част на съобщението.

За да видите тези свойства:

**Работен плот На Outlook**

- Отваряне на елемента
- Свойства на > файлове -> интернет заглавки

Или

**1000000000000**

- Навигирайте до елемента във входящата поща
- Търси PR_TRANSPORT_MESSAGE_HEADERS_W

Тези свойства се определят и записват по време на транспортиране и маршрутизиране. За по-нататъшно отстраняване на неизправности може да се наложи да проследите транспортната поддръжка за неизправностите в SPF, DKIM и.or DMARC.