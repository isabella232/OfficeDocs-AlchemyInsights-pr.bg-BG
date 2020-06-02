---
title: DLP правило за номер на банковата сметка в САЩ не работи
ms.author: deniseb
author: denisebmsft
manager: laurawi
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1287"
- "3200001"
ms.assetid: 80b40145-8376-4c3a-8d22-6efb9f9cb271
ms.openlocfilehash: b032a7c80e8b387114aeda95c4f6af7e57225517
ms.sourcegitcommit: bc7d6f4f3c9f7060d073f5130e1ec856e248d020
ms.translationtype: MT
ms.contentlocale: bg-BG
ms.lasthandoff: 06/02/2020
ms.locfileid: "44507323"
---
# <a name="dlp-issues-with-us-bank-account-numbers"></a>Проблеми с DLP с номера на банкови сметки в САЩ

**Важно**: през тези безпрецедентни времена ние предприемаме стъпки, за да гарантираме, че услугите на SharePoint Online и OneDrive остават на пълно разположение – за повече информация посетете [Временни корекции на функции на SharePoint Online](https://aka.ms/ODSPAdjustments).

**Проблеми с DLP с номера на банкови сметки в САЩ**

Имате проблеми с **предотвратяването на загуба на данни (DLP),** което не работи за съдържание, съдържащо номер на банкова сметка в **САЩ,** когато използвате DLP чувствителен тип информация в O365? Ако е така, уверете се, че съдържанието съдържа необходимата информация за това, което DLP се търси, когато се оценява.
  
Например за **сащ банка номер** правила конфигуриран с ниво на доверие 85%, се оценяват по-долу и трябва да бъдат открити за правилото да задейства:
  
- **[Формат:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#format-77)** 8-17 цифри

- **[Модел:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#pattern-77)** 8-17 последователни цифри.

- **[Контролна сума:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#checksum-76)** Не, няма контролна сума

- **[Определение:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions)** Правилата на DLP са 75% уверени, че е открита тази информация, ако в близост до 300 знака:

  - Регулярният израз Regex_usa_bank_account_number намира съдържание, което съответства на модела

  - Намерена е ключова дума от Keyword_usa_Bank_Account.

    Например следната извадка ще задейства за правилата за **номер на банкови сметки в САЩ:** Проверка на сметка 78344011

За повече информация относно това, което е необходимо за да бъде открит **номер на банковата сметка** в САЩ за вашето съдържание вижте следния раздел в тази статия: Какво чувствителна информация видове изглежда за номер на [банковата сметка в САЩ](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#us-bank-account-number)
  
С помощта на друг вграден тип поверителна информация вижте следната статия за информация за това какво е необходимо за други типове: [Какво се търси типовете информация за чувствителната информация](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions)
  