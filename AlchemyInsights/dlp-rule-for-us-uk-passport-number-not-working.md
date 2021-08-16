---
title: Правило за DLP за номер на паспорт в САЩ/Обединеното кралство не работи
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
ms.openlocfilehash: 85e3ed7fdc221981de13ab6e2ada8adf2a3a80b40ff163981e047cc4a02a1514
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: bg-BG
ms.lasthandoff: 08/05/2021
ms.locfileid: "54004935"
---
# <a name="problems-with-dlp---usuk-passport-numbers"></a>Проблеми с DLP – номера на паспорти в САЩ/Обединеното кралство

**Важно**: през тези безпрецедентни времена ние предприемаме стъпки, за да гарантираме, че услугите на SharePoint Online и OneDrive остават на пълно разположение – за повече информация посетете [Временни корекции на функции на SharePoint Online](https://aka.ms/ODSPAdjustments).

**Проблеми с DLP с номера на паспорти в САЩ/Обединеното кралство**

Имате проблеми с предотвратяването на загуба на данни **(DLP)** не работи за съдържание, съдържащо номер на паспорт **в САЩ/Обединеното** кралство, когато използвате тип информация за DLP поверителна информация в O365? Ако е така, уверете се, че съдържанието ви съдържа необходимата информация за това, което търси DLP правилата, когато се оценява.
  
Например за правила за номер на паспорт **в САЩ/Обединеното** кралство, конфигурирани с доверително ниво от 75%, се оценяват и трябва да бъдат открити следните правила, за да може правилото да се задейства
  
- **[Формат:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#format-77)** Девет цифри

- **[Шарка:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#pattern-77)** Девет последователни цифри

- **[Контролна карта:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#checksum-76)** Не, няма контролна карта

- **[Дефиниция:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#definition-77)** Правилата за DLP са 75% уверени, че са открити този тип поверителна информация, ако в близост до 300 знака:

  - Функцията Func_usa_uk_passport намира съдържание, което отговаря на шарката.

  - Намерена е ключова дума Keyword_passport за търсене.

    Например следната извадка ще се задейства за правилата за номер на паспорт **в САЩ/Обединеното** кралство: номер на паспорт в САЩ 123456789

За повече информация какво е необходимо за откриване на номер на паспорт в САЩ/Обединеното кралство за вашето съдържание, вижте следващия раздел в тази статия: Какво изглеждат типовете поверителна информация за номер на паспорт в [САЩ/Обединеното кралство](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#us--uk-passport-number)
  
Като използвате различен вграден тип поверителна информация, вижте следната статия за информация какво е необходимо за други типове: [Какво търси типовете поверителна информация](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions)
  