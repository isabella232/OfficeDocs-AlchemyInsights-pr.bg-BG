---
title: DLP правило за номер на банкова сметка в САЩ не работи
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
- "1287"
- "3200001"
ms.assetid: 80b40145-8376-4c3a-8d22-6efb9f9cb271
ms.openlocfilehash: eb399e4b23de32a757562833ed32d97daa6a1247
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: bg-BG
ms.lasthandoff: 09/14/2020
ms.locfileid: "47679285"
---
# <a name="dlp-issues-with-us-bank-account-numbers"></a>DLP проблеми с номерата на банковите сметки в САЩ

**Важно**: през тези безпрецедентни времена ние предприемаме стъпки, за да гарантираме, че услугите на SharePoint Online и OneDrive остават на пълно разположение – за повече информация посетете [Временни корекции на функции на SharePoint Online](https://aka.ms/ODSPAdjustments).

**DLP проблеми с номерата на банковите сметки в САЩ**

Имате ли проблеми с **предотвратяване на загуба на данни (DLP)** , които не работят за съдържание, съдържащо **номер на банкова сметка в САЩ** , когато се използва тип на DLP за чувствителна информация в O365? Ако е така, трябва да се уверите, че вашето съдържание съдържа необходимата информация за това, което се търси в DLP политиката, когато бъде изчислена.
  
Например за правилата за **номер на банкова сметка в САЩ** , конфигурирани с ниво на надеждност от 85%, следва да бъдат оценени следните неща и трябва да бъдат открити, за да се задейства правилото:
  
- **[Формат:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#format-77)** 8-17 цифри

- **[Шарка:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#pattern-77)** 8-17 последователни цифри.

- **[Контролна сума:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#checksum-76)** Не, няма шах

- **[Дефиниция:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions)** DLP правилата е 75% сигурни, че той е открил този тип поверителна информация, ако в близост до знаците на 300:

  - Регулярният израз Regex_usa_bank_account_number намира съдържание, което съответства на модела

  - Намерена е ключова дума от Keyword_usa_Bank_Account.

    Например примерът по-долу би активирал за правилата за **номер на банкова сметка на САЩ** : проверка на акаунт 78344011

За повече информация за това, което е необходимо, за да бъде открит **номерът на банкова сметка на САЩ** за вашето съдържание, вижте раздела по-долу в тази статия: [какви типове чувствителна информация търси в САЩ номер на банкова сметка](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#us-bank-account-number)
  
С помощта на различен вграден тип чувствителна информация вижте статията по-долу за информация относно това, което е необходимо за други типове: [какви типове чувствителна информация търсите](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions)
  