---
title: Грешка при изпращане на имейл, блокирани от SpamHaus
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 2/23/2018
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom: Adm_O365
ms.assetid: fa98ab4a-92eb-45e9-8d57-ad10fb123042
ms.openlocfilehash: a16c998d2f289ea2da52454819f6677c405381a1
ms.sourcegitcommit: e2864efcfb493b6e46b662b746661a61232bdba7
ms.translationtype: MT
ms.contentlocale: bg-BG
ms.lasthandoff: 01/24/2019
ms.locfileid: "29458033"
---
# <a name="error-sending-email-client-host-blocked-using-spamhaus"></a>Грешка при изпращане на имейл: клиент домакин блокирани използване Spamhaus

IP адреса, който е изпратил съобщението е в списък за блокиране, собственост на [Spamhaus](https://go.microsoft.com/fwlink/p/?linkid=123245). Причини за блокирано от Spamhaus включват компрометирана сметки, компрометирани машини споделяне публичен IP адрес, както и интернет доставчик (ISP) политики. Възможни корекции са:
  
- За блокираните входящите съобщения в Office 365, където можете да контролирате източник имейл сървър трябва да се определи причината и премахнете блок от сайта на Spamhaus.
    
- За блокираните входящите съобщения в Office 365, където изходният IP адрес принадлежи на някой друг собственика на адреса трябва да премахнете блок от сайта на Spamhaus. Ако IP адресът е в политиката блок списък (PBL), собственикът може да присвоите различни статичен IP адрес или премахнете адреса от PBL.
    
- За блокирани изходящи съобщения от вашия домейн на Office 365 можете да получавате тази грешка, ако съобщенията се насочват чрез 3-та страна услуга. Можете да използвате инструмента за търсене WHOIS да намерите собственика на блокираните IP адрес.
    

