---
title: DLP правило за САЩ / Великобритания паспорт номер не работи
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
ms.openlocfilehash: 0567e9521507bcc192b187d0e5a8a0658332ff99
ms.sourcegitcommit: 5fb7a4b28859690020efdea630d03e70cc0e6334
ms.translationtype: MT
ms.contentlocale: bg-BG
ms.lasthandoff: 06/28/2019
ms.locfileid: "35389530"
---
# <a name="problems-with-dlp---usuk-passport-numbers"></a>Проблеми с DLP - САЩ / Великобритания паспорта номера

Имате ли проблеми с **Данни загуба предотвратяване (DLP)** не работи за съдържание, съдържащи **САЩ / Великобритания паспорт номер** при използване на тип DLP чувствителна информация в O365? Ако е така, уверете се, че вашето съдържание съдържа необходимата информация за какво е търсенето на DLP политика, когато той се оценява.
  
Например, за **САЩ / Великобритания паспорт номер** политика, конфигуриран с ниво на доверие от 75 %, следните се оценяват и трябва да бъдат открити за да задейства правилото
  
- **[Формат:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#format-77)** Девет цифри

- **[Модел:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#pattern-77)** Девет поредни цифри

- **[Контролна сума:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#checksum-76)** Не, няма никакъв шах

- **[Дефиниция:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#definition-77)** DLP политика е 75 % уверени, че е открил този вид чувствителна информация ако, в рамките на близост на 300 знака:

  - Функцията Func_usa_uk_passport открие съдържание, което съвпада с модела.

  - Ключова дума от Keyword_passport е намерен.

    Например, следните примерни ще спусък за **САЩ / Великобритания паспорт номер** политика: Паспорт САЩ номер 123456789

За повече информация за това, което се изисква за САЩ / Великобритания паспорт номер да бъде открито за съдържанието ви, вижте следващия раздел в тази статия: [Какво чувствителна информация типове поглед за САЩ / Великобритания паспорт номер](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#us--uk-passport-number)
  
Използване на тип на различни вградени чувствителна информация, вижте следната статия за повече информация относно какво е необходимо за други типове: [Какво чувствителна информация типове търси](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for)
  