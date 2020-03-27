---
title: DLP правило за кредитна карта номер не работи
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
ms.openlocfilehash: 40a4a1668039b70455e09ee662359c05235645e8
ms.sourcegitcommit: d108a2da2f5dab05246e30b5108cca5173e09051
ms.translationtype: MT
ms.contentlocale: bg-BG
ms.lasthandoff: 03/26/2020
ms.locfileid: "42977187"
---
# <a name="dlp-issues-with-credit-card-numbers"></a>DLP проблеми с номера на кредитни карти

**Важно**: По време на тези безпрецедентни времена, ние предприемаме стъпки, за да се гарантира, че SharePoint Online и OneDrive услуги остават високо достъпни – посетете [SharePoint Online временни функция корекции](https://aka.ms/ODSPAdjustments) за повече информация.

**DLP проблеми с номера на кредитни карти**

Имате проблеми с **предотвратяване на загуба на данни (DLP)** не работи за съдържание, съдържащо номер на кредитна **карта,** когато използвате тип на чувствителна тайнствена СТОЙНОСТ в O365? Ако е така, уверете се, че съдържанието ви съдържа необходимата информация за задействане на правилата на DLP, когато се оценява. Например за правила за **кредитна карта,** конфигурирани с ниво на сигурност от 85%, се оценяват следните и трябва да бъдат открити, за да се задейства правилото:
  
- **[Формат:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#format-19)** 16 цифри, които могат да бъдат форматирани или неформатирани (dddddddddddddddddddddddddddddddddddddddddddddddddddddddddddddddddddddddddddddddddddddddddddddddddddddddddddd

- **[Модел:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#pattern-19)** Много сложен и здрав модел, който открива карти от всички основни марки в света, включително Visa, MasterCard, Discover Card, JCB, American Express, карти за подаръци и карти за закусва.

- **[Контролна сума:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#checksum-19)** Да, чексумата на Луен

- **[Определение:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#definition-19)** DLP политика е 85% уверен, че е открит този тип чувствителна информация, ако в близост до 300 знака:

  - Функцията Func_credit_card намира съдържание, което съответства на шаблона.

  - Едно от следните неща е вярно:

  - Намерена е ключова дума от Keyword_cc_verification.

  - Намерена е ключова дума от Keyword_cc_name

  - Функцията Func_expiration_date намира дата в правилния формат на датата.

  - Контролната сума

    Например следните примерни ще предизвика за DLP кредитна карта номер политика:

  - Виза: 4485 3647 3952 7352
  
  - Изтича на: 2/2009

За повече информация относно това, което е необходимо за да бъде открит **номер на кредитна карта** за вашето съдържание, вижте следния раздел в тази статия: Какви типове [поверителна информация търсят кредитна карта#](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#credit-card-number)
  
Използвайки друг вграден тип поверителна информация, вижте следната статия за информация за това какво се изисква за други типове: [Какво търсят типовете поверителна информация за](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for)
  