---
title: Множество обекти имат един и същ имейл адрес като самоличност
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/27/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "1834"
- "9000247"
ms.openlocfilehash: 05fb43133bc68b71ccdbab44d28679a1f659e762
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: bg-BG
ms.lasthandoff: 09/14/2020
ms.locfileid: "47724604"
---
# <a name="multiple-objects-have-the-same-email-address-as-identity"></a>Множество обекти имат един и същ имейл адрес като самоличност

**Множество обекти**

Една от често срещаните причини за тази грешка не е в състояние да маршрутизира правилно заявка на Outlook Web Access в наличност на множество обекти, които имат един и същ имейл адрес като самоличност. За да намерите тези обекти, изпълнете следните команди:

· Получаване на получателя <email address>

· Get-User <email address>

· Get-User <email address> -SoftDeletedUser

· Свържете се с нас <email address>

· Получаване на пощенска кутия <email address> – PublicFolder

· Получаване на пощенска кутия <email address> – IncludeSoftDeletedMailbox

· Получаване на пощенска кутия <email address> – InactiveMailboxOnly

За да отстраните проблема, премахнете множество обекти с една и съща самоличност на имейл и се уверете, че има един обект с конкретната самоличност за имейл и че неговият тип получател е UserMailbox.

**Един и същ адрес се използва за пощенските кутии за фирми и потребители**

Друга причина е, когато един и същ адрес се използва за пощенски кутии за фирми и потребители. В този случай потребителят трябва да промени своя първичен псевдоним за потребител, докато Cafe не подкрепи този сценарий. Това е постоянна грешка, която не изчезва без интервенция.

За подробности вижте [Промяна на имейл адреса или телефонния номер за вашия акаунт в Microsoft](https://support.microsoft.com/help/11545/microsoft-account-rename-your-personal-account).