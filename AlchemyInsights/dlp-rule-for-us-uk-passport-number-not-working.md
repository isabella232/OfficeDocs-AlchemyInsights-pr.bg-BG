---
title: DLP правило за САЩ/Великобритания номер на паспорт не работи
ms.author: deniseb
author: denisebmsft
manager: laurawi
ms.date: 11/5/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1319"
- "3200001"
ms.assetid: fc178b8b-943b-4346-a2bd-a75c6af6f80f
ms.openlocfilehash: 534e258c31a9a71c618765511487487c53f455b5
ms.sourcegitcommit: d108a2da2f5dab05246e30b5108cca5173e09051
ms.translationtype: MT
ms.contentlocale: bg-BG
ms.lasthandoff: 03/26/2020
ms.locfileid: "42977095"
---
# <a name="problems-with-dlp---usuk-passport-numbers"></a>Проблеми с DLP - САЩ /UK номера на паспорти

**Важно**: По време на тези безпрецедентни времена, ние предприемаме стъпки, за да се гарантира, че SharePoint Online и OneDrive услуги остават високо достъпни – посетете [SharePoint Online временни функция корекции](https://aka.ms/ODSPAdjustments) за повече информация.

**DLP проблеми с американски/великобритания паспортни номера**

Имате проблеми с **предотвратяване на загуба на данни (DLP)** не работи за съдържание, съдържащо номер на **американски/английски паспорт** при използване на тип на чувствителна тайнствена ИНФОРМАЦИЯ DLP в O365? Ако е така, уверете се, че съдържанието ви съдържа необходимата информация за това, което се търси dlp правила, когато се оценява.
  
Например, за политика за **номер на паспорт сащ/Обединеното кралство,** конфигурирана с ниво на сигурност от 75%, се оценяват следните и трябва да бъдат открити, за да се задейства правилото
  
- **[Формат на](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#format-77)** Девет цифри

- **[Модел:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#pattern-77)** Девет последователни цифри

- **[Контролна сума:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#checksum-76)** Не, няма чексума

- **[Определение:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#definition-77)** DLP политика е 75% уверен, че е открит този тип чувствителна информация, ако в близост до 300 знака:

  - Функцията Func_usa_uk_passport намира съдържание, което съответства на шаблона.

  - Намира се ключова дума от Keyword_passport.

    Например следната извадка ще задейства за **САЩ/Великобритания паспорт номер** политика: Номер на паспорт а в САЩ 123456789

За повече информация относно това, което е необходимо за да бъде открит номер на американски/британски паспорт за вашето съдържание, вижте раздела по-долу в тази статия: [Какви типове информация за сащ/Великобритания търсят за сащ/UK Passport Number](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#us--uk-passport-number)
  
Използвайки друг вграден тип поверителна информация, вижте следната статия за информация за това какво се изисква за други типове: [Какво търсят типовете поверителна информация за](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for)
  