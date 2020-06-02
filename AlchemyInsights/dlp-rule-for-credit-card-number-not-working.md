---
title: DLP правило за кредитна карта номер не работи
ms.author: deniseb
author: denisebmsft
manager: laurawi
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1270"
- "3200001"
ms.assetid: 30496c79-c8b4-4337-a46d-abed12864209
ms.openlocfilehash: e2e93bed44749b9017dc6ff919a151d46da7a3fc
ms.sourcegitcommit: bc7d6f4f3c9f7060d073f5130e1ec856e248d020
ms.translationtype: MT
ms.contentlocale: bg-BG
ms.lasthandoff: 06/02/2020
ms.locfileid: "44507395"
---
# <a name="dlp-issues-with-credit-card-numbers"></a>Проблеми с DLP с номера на кредитни карти

**Важно**: през тези безпрецедентни времена ние предприемаме стъпки, за да гарантираме, че услугите на SharePoint Online и OneDrive остават на пълно разположение – за повече информация посетете [Временни корекции на функции на SharePoint Online](https://aka.ms/ODSPAdjustments).

**Проблеми с DLP с номера на кредитни карти**

Имате проблеми с **предотвратяване на загуба на данни (DLP),** които не работят за съдържание, съдържащо номер на кредитна **карта,** когато използвате DLP чувствителен тип информация в O365? Ако е така, уверете се, че съдържанието съдържа необходимата информация, за да задействате правилата на DLP, когато се оценява. Например за **кредитна карта правила** конфигуриран с ниво на доверие от 85 %, се оценяват следното и трябва да бъдат открити за правилото да задейства:
  
- **[Формат:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#format-19)** 16 цифри, които могат да бъдат форматирани или неформатирани (ddddddddddddddddddddddddddddddddddddddddddddddddddddddddddddddddddddddddddddddddddddddddddddddddddddddddddddddd)

- **[Модел:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#pattern-19)** Много сложен и здрав модел, който открива карти от всички големи марки в света, включително Visa, MasterCard, Discover Card, JCB, American Express, карти за подаръчни подаръци, и закусвални карти.

- **[Контролна сума:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#checksum-19)** Да, сумата на Лун

- **[Определение:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#definition-19)** DLP политика е 85% уверени, че е открита този тип чувствителна информация, ако в близост до 300 знака:

  - Функцията Func_credit_card намира съдържание, което съответства на модела.

  - Едно от следните е вярно:

  - Намерена е ключова дума от Keyword_cc_verification.

  - Намерена е ключова дума от Keyword_cc_name

  - Функцията Func_expiration_date намери дата в правилния формат на датата.

  - Контролната сума преминава

    Например следната пример ще задейства DLP кредитна карта номер политика:

  - Виза: 4485 3647 3952 7352
  
  - Изтича на: 2/2009

За повече информация относно това, което е необходимо за да бъде открит **номер на кредитна карта** за вашето съдържание, вижте следния раздел в тази статия: Какво чувствителна информация видове изглежда за кредитна карта [#](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#credit-card-number)
  
С помощта на друг вграден тип поверителна информация вижте следната статия за информация за това какво е необходимо за други типове: [Какво се търси типовете информация за чувствителната информация](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions)
  