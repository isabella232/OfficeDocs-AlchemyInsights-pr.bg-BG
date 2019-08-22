---
title: Грешка при изпращане на имейл, блокирани от SpamHaus
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 2/23/2018
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "255"
- "3100003"
ms.assetid: fa98ab4a-92eb-45e9-8d57-ad10fb123042
ms.openlocfilehash: 39213f6f1b96c2bef9ea071f43c38766debf64d1
ms.sourcegitcommit: 1d98db8acb9959aba3b5e308a567ade6b62da56c
ms.translationtype: MT
ms.contentlocale: bg-BG
ms.lasthandoff: 08/22/2019
ms.locfileid: "36527121"
---
# <a name="error-sending-email-client-host-blocked-using-spamhaus"></a>Грешка при изпращане на имейл: клиент домакин блокирани използване Spamhaus

IP адреса, който е изпратил съобщението е в списък за блокиране, собственост на [Spamhaus](https://go.microsoft.com/fwlink/p/?linkid=123245). Причини за блокирано от Spamhaus включват компрометирана сметки, компрометирани машини споделяне публичен IP адрес, както и интернет доставчик (ISP) политики. Възможни корекции са:
  
- За блокираните входящите съобщения в Office 365, където можете да контролирате източник имейл сървър трябва да се определи причината и премахнете блок от сайта на Spamhaus.

- За блокираните входящите съобщения в Office 365, където изходният IP адрес принадлежи на някой друг собственика на адреса трябва да премахнете блок от сайта на Spamhaus. Ако IP адресът е в политиката блок списък (PBL), собственикът може да присвоите различни статичен IP адрес или премахнете адреса от PBL.

- За блокирани изходящи съобщения от вашия домейн на Office 365 можете да получавате тази грешка, ако съобщенията се насочват чрез 3-та страна услуга. Можете да използвате инструмента за търсене WHOIS да намерите собственика на блокираните IP адрес.
