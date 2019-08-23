---
title: DLP правило за номер на кредитна карта не работи
ms.author: deniseb
author: denisebmsft
manager: laurawi
ms.date: 11/5/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1270"
- "3200001"
ms.assetid: 30496c79-c8b4-4337-a46d-abed12864209
ms.openlocfilehash: 875afb47175a78c22894720cb0db8222f6f41614
ms.sourcegitcommit: 1d98db8acb9959aba3b5e308a567ade6b62da56c
ms.translationtype: MT
ms.contentlocale: bg-BG
ms.lasthandoff: 08/22/2019
ms.locfileid: "36529944"
---
# <a name="dlp-issues-with-credit-card-numbers"></a>DLP проблеми с номера на кредитни карти

Имате ли проблеми с **Данни загуба предотвратяване (DLP)** не работи за съдържание, съдържаща **Номер на кредитна карта** , когато използвате тип DLP чувствителна информация в O365? Ако е така, се уверете, че вашето съдържание съдържа необходимата информация за задействане на DLP политика, когато той се оценява. Например за **кредитната ви карта** конфигуриран с ниво на доверие от 85 %, следното се оценяват и трябва да бъде открит за да задейства правилото:
  
- **[Формат:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#format-19)** 16 цифри, което може да бъде форматиран или неформатиран (dddddddddddddddd) и трябва да мине на Luhn теста.

- **[Модел:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#pattern-19)** Много сложни и стабилна шарка, която открива карти от всички основни марки по целия свят, включително Visa, MasterCard, Открийте карта, JCB, American Express, подарък и вечеря карти.

- **[Контролна сума:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#checksum-19)** Да, на Luhn шах

- **[Дефиниция:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#definition-19)** DLP политика е 85 % уверени, че е открил този вид чувствителна информация ако, в рамките на близост на 300 знака:

  - Функцията Func_credit_card открие съдържание, което съвпада с модела.

  - Един от следните е вярно:

  - Ключова дума от Keyword_cc_verification е намерен.

  - Ключова дума от Keyword_cc_name се намира

  - Функцията Func_expiration_date намира дата във формат на правилната дата.

  - Контролна преминава

    Например следните примерни ще предизвика DLP кредитна карта номер политика за:

  - Виза: 4485 3647 3952 7352
  
  - Изтича: 2/2009

За повече информация относно това, което се изисква за **Номер на кредитна карта** , за да бъдат открити за вашето съдържание, вижте следващия раздел в тази статия: [Какво чувствителна информация типове търси кредитна карта #](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#credit-card-number)
  
Използване на тип на различни вградени чувствителна информация, вижте следната статия за повече информация относно какво е необходимо за други типове: [Какво чувствителна информация типове търси](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for)
  