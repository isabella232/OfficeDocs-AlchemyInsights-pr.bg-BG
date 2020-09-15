---
title: DLP правило за номер на кредитна карта не работи
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
ms.openlocfilehash: d5dd6354e7a1bcbb7f2fb917952ddbee5077e88d
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: bg-BG
ms.lasthandoff: 09/14/2020
ms.locfileid: "47679430"
---
# <a name="dlp-issues-with-credit-card-numbers"></a>DLP въпроси с номера на кредитни карти

**Важно**: през тези безпрецедентни времена ние предприемаме стъпки, за да гарантираме, че услугите на SharePoint Online и OneDrive остават на пълно разположение – за повече информация посетете [Временни корекции на функции на SharePoint Online](https://aka.ms/ODSPAdjustments).

**DLP въпроси с номера на кредитни карти**

Имате ли проблеми с **предотвратяване на загуба на данни (DLP)** , които не работят за съдържание, съдържащо **номер на кредитна карта** , когато се използва тип на DLP чувствителна информация в O365? Ако е така, трябва да се уверите, че вашето съдържание съдържа нужната информация, за да се задейства DLP правилата, когато бъдат оценени. Например за **правилата за кредитна карта** , конфигурирани с ниво на надеждност от 85%, следва да бъдат оценени следните неща и трябва да бъдат открити, за да се задейства правилото:
  
- **[Формат:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#format-19)** 16 цифри, които могат да бъдат форматирани или неформатирани (dddddddddddddddd) и трябва да изминат теста Luhn.

- **[Шарка:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#pattern-19)** Много сложна и здрава шарка, която открива картите от всички основни марки по целия свят, включително Visa, MasterCard, Discover Card, JCB, American Express, ваучери за подарък и вечеря.

- **[Контролна сума:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#checksum-19)** Да, контролната сума за Luhn

- **[Дефиниция:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#definition-19)** DLP правилата е 85% сигурни, че той е открил този тип поверителна информация, ако в близост до знаците на 300:

  - Функцията Func_credit_card намира съдържание, което съответства на шарката.

  - Едно от следните е вярно:

  - Намерена е ключова дума от Keyword_cc_verification.

  - Намерена е ключова дума от Keyword_cc_name

  - Функцията Func_expiration_date намира дата в правилния формат за дата.

  - Контролните пропуски

    Например примерът по-долу би предизвикал правила за номер за DLP кредитна карта:

  - Виза: 4485 3647 3952 7352
  
  - Изтича: 2/2009

За повече информация за това, което е необходимо за откриване на **номер на кредитна карта** за вашето съдържание, вижте раздела по-долу в тази статия: [какви типове чувствителна информация търсите за кредитна карта #](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#credit-card-number)
  
С помощта на различен вграден тип чувствителна информация вижте статията по-долу за информация относно това, което е необходимо за други типове: [какви типове чувствителна информация търсите](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions)
  