---
title: Грешка при изпращане на имейл, блокиран от SpamHaus
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "255"
- "3100003"
ms.assetid: fa98ab4a-92eb-45e9-8d57-ad10fb123042
ms.openlocfilehash: 8372032e19bd2ebaf3ba8cc8e87f19ef3e2edf1e607b1739a919f6dcc443cd97
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: bg-BG
ms.lasthandoff: 08/05/2021
ms.locfileid: "53946695"
---
# <a name="error-sending-email-client-host-blocked-using-spamhaus"></a>Грешка при изпращане на имейл: Хостът на клиента е блокиран с помощта на Spamhaus

IP адресът, който е изпратил съобщението, е в списък за блокиране, притежаван [от Spamhaus.](https://go.microsoft.com/fwlink/p/?linkid=123245) Причините за блокиране от Spamhaus включват компрометирани акаунти, компрометирани машини, споделящи публичен IP адрес, и правила за доставчик на интернет (ISP). Възможните корекции са:
  
- За блокирани входящи съобщения, където управлявате изходния имейл сървър, трябва да определите причината и да премахнете блока от уеб сайта на Spamhaus.

- За блокирани входящи съобщения, където IP адресът източник принадлежи на някой друг, собственикът на адреса трябва да премахне блока от уеб сайта на Spamhaus. Ако IP адресът е в списъка с блокирани правила (PBL), собственикът може да назначи друг статичен IP адрес или да премахне адреса от PBL.

- За блокирани изходящи съобщения от вашия домейн, свързани с Microsoft, можете да получите тази грешка, ако съобщенията се маршрутизирани чрез услуга на трета страна. Можете да използвате инструмент за търсене на WHOIS, за да намерите собственика на блокирания IP адрес.
