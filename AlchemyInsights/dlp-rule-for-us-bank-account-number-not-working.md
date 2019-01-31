---
title: DLP правило за нас банкова сметка номер не работи
ms.author: cmcatee
author: cmcatee-MSFT
manager: mnirkhe
ms.date: 11/5/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.assetid: 80b40145-8376-4c3a-8d22-6efb9f9cb271
ms.openlocfilehash: 9fd5d4736c5209f85e235dc6a0846f65f1b5f624
ms.sourcegitcommit: 0ae6cbb8cf2836da98300767ed81b411d6551bee
ms.translationtype: MT
ms.contentlocale: bg-BG
ms.lasthandoff: 01/30/2019
ms.locfileid: "29656988"
---
Имате ли проблеми с **Данни загуба предотвратяване (DLP)** не работи за съдържание, съдържаща **Номер на банкова сметка на САЩ** , когато използвате тип DLP чувствителна информация в O365? Ако е така, уверете се, че вашето съдържание съдържа необходимата информация за какво е търсенето на DLP политика, когато той се оценява. 
  
Например за политика на **САЩ банкова сметка номер** , конфигуриран с ниво на доверие от 85 %, следното се оценяват и трябва да бъде открит за да задейства правилото: 
  
- **[Формат:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#format-77)** 8-17 цифри 
    
- **[Модел:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#pattern-77)** 8-17 поредни цифри. 
    
- **[Контролна сума:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#checksum-76)** Не, няма никакъв шах 
    
- **[Дефиниция:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for)** DLP политика е 75 % уверени, че е открил този вид чувствителна информация ако, в рамките на близост на 300 знака: 
    
  - Регулярен израз Regex_usa_bank_account_number открие съдържание, което съвпада с модела
    
  - Ключова дума от Keyword_usa_Bank_Account е намерен.
    
    Например, следните примерни ще спусък за политиката на **САЩ банкова сметка номер** : разплащателна сметка 78344011 
    
За повече информация относно това, което се изисква за **Номер на банкова сметка на САЩ** да бъдат открити за вашето съдържание, вижте следващия раздел в тази статия: [Какво чувствителна типове информация потърсете номер на банкова сметка на САЩ](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#us-bank-account-number)
  
Използване на тип на различни вградени чувствителна информация, вижте следната статия за повече информация относно какво е необходимо за други типове: [Какво чувствителна информация типове търси](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for)
  

