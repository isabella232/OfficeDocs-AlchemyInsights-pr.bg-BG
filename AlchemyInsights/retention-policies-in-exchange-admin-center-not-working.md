---
title: Правила за съхранение в Exchange за администриране не работят
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "308"
- "3100007"
ms.assetid: a48fd5fd-4af7-4d5f-b617-b0f9334ccaa7
ms.openlocfilehash: 6652ad5fc1691e1d5a4293d81f3a649f23ec38f18c8ed9fe06665628a901d13e
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: bg-BG
ms.lasthandoff: 08/05/2021
ms.locfileid: "54074921"
---
# <a name="retention-policies-in-exchange-admin-center"></a>Правила за съхранение в Exchange за администриране

Ако искате да изпълняваме автоматизирани проверки за настройките, споменати по-долу, изберете бутона назад < – в горната част на тази страница и след това въведете имейл адреса на потребителя, който има проблеми с правилата за съхранение.

Ако имате проблеми с правилата за съхранение в центъра за администриране на Exchange, които не се отнасят за пощенски кутии или елементи, които не се преместват в архивната пощенска кутия, проверете следното:

**Главни причини:**

- **Помощникът за управлявани** папки не е обработил пощенската кутия на потребителя. Помощникът за управлявани папки се опитва да обработи всяка пощенска кутия във вашата организация, базирана на облака, веднъж на всеки седем дни.

  **Решение:** Изпълнете помощника за управлявани папки.

- **ЗадържанеТо е** разрешено **в** пощенската кутия. Ако пощенската кутия е поставена в задържанеHold, правилата за съхранение в пощенската кутия няма да бъдат обработвани през това време.

  **Решение:** Проверете състоянието на настройката за задържане на задържането и актуализирайте, ако е необходимо. За подробности вижте Задържане [на пощенската кутия.](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/mailbox-retention-hold)
 
**Забележка:** Ако пощенската кутия е по-малка от 10 МБ, помощникът за управлявани папки няма да обработи автоматично пощенската кутия.
 
За повече информация относно правилата за съхранение в центъра Exchange за администриране вижте:

- [Етикети за съхранение и правила за съхранение](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/retention-tags-and-policies)

- [Прилагане на правила за съхранение към пощенски кутии или](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/apply-retention-policy) Добавяне или премахване на етикети за [съхранение](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/add-or-remove-retention-tags)

- [Как да идентифицирате типа задържане, поставено в пощенска кутия](https://docs.microsoft.com/microsoft-365/compliance/identify-a-hold-on-an-exchange-online-mailbox)
