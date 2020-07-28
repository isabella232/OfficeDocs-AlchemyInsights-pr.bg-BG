---
title: Множество обекти имат същия имейл адрес като идентичност
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/27/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "1834"
- "9000247"
ms.openlocfilehash: cc932aa7ecbd1e338c409a7a6525e2c4e673b232
ms.sourcegitcommit: b10cea11b4975354b91193327b58aa4740d34833
ms.translationtype: MT
ms.contentlocale: bg-BG
ms.lasthandoff: 07/28/2020
ms.locfileid: "45438735"
---
# <a name="multiple-objects-have-the-same-email-address-as-identity"></a>Множество обекти имат същия имейл адрес като идентичност

**Множество обекти**

Една от най-честите причини за тази грешка е да не можете да маршрутите outlook Web Access заявка правилно в присъствието на множество обекти, които имат същия имейл адрес като самоличност. За да намерите тези обекти, изпълнете следните команди:

· Получаване на получател<email address>

· Потребител за получаване<email address>

· Потребител <email address> - Софтуерен Потребител

· Контакт с вас<email address>

· Get-пощенска кутия <email address> publicFolder

· Пощенска кутия <email address> -IncludeSoftИзтрешенmailbox

· Пощенска кутия <email address> - неактивни само

За да разрешите проблема, премахнете няколко обекта с една и съща самоличност на имейл и се уверете, че има един обект с конкретен имейл самоличността и че типа на получателя е UserMailbox.

**Същият адрес се използва за пощенски кутии за фирми и потребители**

Друга причина е, когато се използва същия адрес за бизнес и потребителски пощенски кутии. В този случай потребителят трябва да промените основния потребителски псевдоним, докато кафе поддържа този сценарий. Това е постоянна грешка, която не изчезва без намеса.

За подробности вижте [Промяна на имейл адреса или телефонния номер за вашия акаунт в Microsoft](https://support.microsoft.com/help/11545/microsoft-account-rename-your-personal-account).