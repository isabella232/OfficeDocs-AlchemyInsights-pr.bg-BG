---
title: DLP правило за номер на паспорт САЩ/Великобритания не работи
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
- "1319"
- "3200001"
ms.assetid: fc178b8b-943b-4346-a2bd-a75c6af6f80f
ms.openlocfilehash: c6c7191f380f264113e2042f2869d9767922b2cc
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: bg-BG
ms.lasthandoff: 09/14/2020
ms.locfileid: "47679213"
---
# <a name="problems-with-dlp---usuk-passport-numbers"></a>Проблеми с номерата на паспорти със DLP/САЩ/Великобритания

**Важно**: през тези безпрецедентни времена ние предприемаме стъпки, за да гарантираме, че услугите на SharePoint Online и OneDrive остават на пълно разположение – за повече информация посетете [Временни корекции на функции на SharePoint Online](https://aka.ms/ODSPAdjustments).

**DLP проблеми с номерата за паспорти САЩ и Великобритания**

Имате ли проблеми с **предотвратяване на загуба на данни (DLP)** , които не работят за съдържание, съдържащо **номер в САЩ/UK Passport** , когато се използва тип DLP чувствителна информация в O365? Ако е така, трябва да се уверите, че вашето съдържание съдържа необходимата информация за това, което се търси в DLP политиката, когато бъде изчислена.
  
Например за правилата за **номер за паспорт САЩ/Обединеното кралство** , конфигурирани с ниво на надеждност от 75%, следва да бъдат оценени следните неща и трябва да бъдат открити, за да се активира правилото
  
- **[Формат:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#format-77)** Девет цифри

- **[Шарка:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#pattern-77)** Девет последователни цифри

- **[Контролна сума:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#checksum-76)** Не, няма шах

- **[Дефиниция:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#definition-77)** DLP правилата е 75% сигурни, че той е открил този тип поверителна информация, ако в близост до знаците на 300:

  - Функцията Func_usa_uk_passport намира съдържание, което съответства на шарката.

  - Намерена е ключова дума от Keyword_passport.

    Например примерът по-долу би предизвикал правила за **номер за паспорт за САЩ/Великобритания** : номер на САЩ за паспорт 123456789

За повече информация за това, което е необходимо за откриване на номер за паспорт САЩ/Великобритания за вашето съдържание, вижте раздела по-долу в тази статия: [какви типове чувствителна информация търси САЩ/номер на паспорт](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#us--uk-passport-number)
  
С помощта на различен вграден тип чувствителна информация вижте статията по-долу за информация относно това, което е необходимо за други типове: [какви типове чувствителна информация търсите](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions)
  