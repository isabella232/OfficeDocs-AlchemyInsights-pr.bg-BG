---
title: DLP правило за САЩ / Великобритания паспорт номер не работи
ms.author: cmcatee
author: cmcatee-MSFT
manager: mnirkhe
ms.date: 11/5/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.assetid: fc178b8b-943b-4346-a2bd-a75c6af6f80f
ms.openlocfilehash: 716d1030d93ce006c36d7925fb132e974ae8feb4
ms.sourcegitcommit: e2864efcfb493b6e46b662b746661a61232bdba7
ms.translationtype: MT
ms.contentlocale: bg-BG
ms.lasthandoff: 01/24/2019
ms.locfileid: "29458328"
---
Имате ли проблеми с **Данни загуба предотвратяване (DLP)** не работи за съдържание, съдържащи **САЩ / Великобритания паспорт номер** при използване на тип DLP чувствителна информация в O365? Ако е така, уверете се, че вашето съдържание съдържа необходимата информация за какво е търсенето на DLP политика, когато той се оценява. 
  
Например, за **САЩ / Великобритания паспорт номер** политика, конфигуриран с ниво на доверие от 75 %, следните се оценяват и трябва да бъдат открити за да задейства правилото 
  
- **[Формат:](https://docs.microsoft.com/en-us/office365/securitycompliance/what-the-sensitive-information-types-look-for#format-77)** Девет цифри 
    
- **[Модел:](https://docs.microsoft.com/en-us/office365/securitycompliance/what-the-sensitive-information-types-look-for#pattern-77)** Девет поредни цифри 
    
- **[Контролна сума:](https://docs.microsoft.com/en-us/office365/securitycompliance/what-the-sensitive-information-types-look-for#checksum-76)** Не, няма никакъв шах 
    
- **[Дефиниция:](https://docs.microsoft.com/en-us/office365/securitycompliance/what-the-sensitive-information-types-look-for#definition-77)** DLP политика е 75 % уверени, че е открил този вид чувствителна информация ако, в рамките на близост на 300 знака: 
    
  - Функцията Func_usa_uk_passport открие съдържание, което съвпада с модела.
    
  - Ключова дума от Keyword_passport е намерен.
    
    Например, следните примерни ще спусък за **САЩ / Великобритания паспорт номер** политика: Паспорт САЩ номер 123456789 
    
За повече информация за това, което се изисква за САЩ / Великобритания паспорт номер да бъде открито за съдържанието ви, вижте следващия раздел в тази статия: [Какво чувствителна информация типове поглед за САЩ / Великобритания паспорт номер](https://docs.microsoft.com/en-us/office365/securitycompliance/what-the-sensitive-information-types-look-for#us--uk-passport-number)
  
Използване на тип на различни вградени чувствителна информация, вижте следната статия за повече информация относно какво е необходимо за други типове: [Какво чувствителна информация типове търси](https://docs.microsoft.com/en-us/office365/securitycompliance/what-the-sensitive-information-types-look-for)
  

