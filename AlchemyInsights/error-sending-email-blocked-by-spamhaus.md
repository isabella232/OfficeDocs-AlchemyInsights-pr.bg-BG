---
title: Грешка при изпращане на имейл, блокиран от SpamHaus
ms.author: pebaum
author: pebaum
manager: mnirkhe
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
ms.openlocfilehash: a0c2f4be0b2d8ba6fd3dadbdf306e6ce623ad380
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: bg-BG
ms.lasthandoff: 09/15/2020
ms.locfileid: "47783756"
---
# <a name="error-sending-email-client-host-blocked-using-spamhaus"></a>Грешка при изпращане на имейл: хостът на клиента е блокиран чрез SpamHaus

IP адресът, който е изпратил съобщението, е в списък на блокирани, собственост на [SpamHaus](https://go.microsoft.com/fwlink/p/?linkid=123245). Причините за блокирането на SpamHaus включват компрометирани акаунти, компрометирани машини, споделящи публичен IP адрес и правила за интернет доставчик (ISP). Възможните корекции са:
  
- За блокирани входящи съобщения, където можете да управлявате изходния имейл сървър, трябва да определите причината и да премахнете блока от уеб сайта на SpamHaus.

- За блокирани входящи съобщения, в които IP адресът източник принадлежи на някой друг, собственикът на адреса трябва да премахне блока от уеб сайта на SpamHaus. Ако IP адресът е в списъка с блокирани правила (PBL), собственикът може да назначи различен статичен IP адрес или да премахне адреса на PBL.

- За блокирани изходящи съобщения от вашия домейн, които са свързани с Microsoft, можете да получите тази грешка, ако съобщенията се маршрутизират чрез услуга на трети страни. Можете да използвате инструмент за търсене WHOIS, за да намерите блокирания собственик на IP адреси.
