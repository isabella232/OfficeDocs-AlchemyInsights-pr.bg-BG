---
title: Правило за DLP за номер на кредитна карта не работи
ms.author: deniseb
author: denisebmsft
manager: laurawi
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1270"
- "3200001"
ms.assetid: 30496c79-c8b4-4337-a46d-abed12864209
ms.openlocfilehash: bd4f200233d5571fc7b01576038e7b3951a07716a7d5948005418d2896291ee5
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: bg-BG
ms.lasthandoff: 08/05/2021
ms.locfileid: "54005079"
---
# <a name="dlp-issues-with-credit-card-numbers"></a>Проблеми с DLP с номера на кредитни карти

**Важно**: през тези безпрецедентни времена ние предприемаме стъпки, за да гарантираме, че услугите на SharePoint Online и OneDrive остават на пълно разположение – за повече информация посетете [Временни корекции на функции на SharePoint Online](https://aka.ms/ODSPAdjustments).

**Проблеми с DLP с номера на кредитни карти**

Имате проблеми с предотвратяването на загуба на данни **(DLP)** не работи за съдържание, съдържащо номер на кредитна карта, когато използвате тип информация за DLP поверителна информация в O365?  Ако е така, уверете се, че съдържанието ви съдържа необходимата информация, за да задейства правилата за DLP, когато се оценява. Например за правила за **кредитна карта,** конфигурирани с доверително ниво от 85%, се оценяват следните и трябва да бъдат открити, за да задейства правилото:
  
- **[Формат:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#format-19)** 16 цифри, които могат да бъдат форматирани или неформатирани (dddddddddd) и трябва да преминат теста luhn.

- **[Шарка:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#pattern-19)** Много сложен и стабилен модел, който открива карти от всички основни марки по целия свят, включително Visa, MasterCard, Discover Card, JCB, American Express, ваучери за подарък и картички за вечеря.

- **[Контролна карта:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#checksum-19)** Да, контролната карта на Лун

- **[Дефиниция:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#definition-19)** Правилата за DLP са 85% уверени, че са открити този тип поверителна информация, ако в близост до 300 знака:

  - Функцията Func_credit_card намира съдържание, което отговаря на шарката.

  - Едно от следните неща е вярно:

  - Намерена е Keyword_cc_verification ключова дума от него.

  - Намерена е Keyword_cc_name ключова дума

  - Функцията Func_expiration_date намери дата в правилния формат за дата.

  - Контролната карта преминава

    Например следната извадка ще задейства правила за номер на DLP кредитна карта:

  - Визи: 4485 3647 3952 7352
  
  - Изтича на: 2.02.2009 г.

За повече информация какво е  необходимо за откриване на номер на кредитна карта за вашето съдържание, вижте следващия раздел в тази статия: Какво търси типовете поверителна информация [за кредитна карта#](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#credit-card-number)
  
Като използвате различен вграден тип поверителна информация, вижте следната статия за информация какво е необходимо за други типове: [Какво търси типовете поверителна информация](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions)
  