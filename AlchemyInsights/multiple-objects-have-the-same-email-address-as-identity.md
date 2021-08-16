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
ms.openlocfilehash: 5866d182cb2e97e37bc6df87e05fb6ef55bfed1d36f9daa95b7b8993a509e2dd
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: bg-BG
ms.lasthandoff: 08/05/2021
ms.locfileid: "54011901"
---
# <a name="multiple-objects-have-the-same-email-address-as-identity"></a>Множество обекти имат един и същ имейл адрес като самоличност

**Множество обекти**

Една от често срещаните причини за тази грешка не е в състояние да маршрути Outlook искане за уеб достъп правилно в присъствието на множество обекти, които имат един и същ имейл адрес като самоличност. За да намерите тези обекти, изпълнете следните команди:

· Get-Recipient <email address>

· Get-User <email address>

· Get-User <email address> -SoftDeletedUser

· Get-Contact <email address>

· Get-Mailbox <email address> -PublicFolder

· Get-Mailbox <email address> -IncludeSoftDeletedMailbox

· Get-Mailbox <email address> -InactiveMailboxOnly

За да отстраните проблема, премахнете няколко обекта с една и съща имейл самоличност и се уверете, че има един обект с конкретната имейл самоличност и че неговият тип получател е UserMailbox.

**Същият адрес се използва за пощенски кутии на бизнеса и потребителите**

Друга причина е, когато същият адрес се използва за пощенски кутии на бизнеса и потребителите. В този случай потребителят трябва да промени своя основен потребителски псевдоним, докато кафенето не поддържа този сценарий. Това е постоянна грешка, която не излиза без намеса.

За подробности вижте Промяна [на имейл адреса или телефонния номер за вашия акаунт в Microsoft](https://support.microsoft.com/help/11545/microsoft-account-rename-your-personal-account).