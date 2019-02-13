---
title: DLP правило за SSN не работи
ms.author: cmcatee
author: cmcatee-MSFT
manager: mnirkhe
ms.date: 11/5/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: ac265ee6-c946-476e-9bf0-0ea0e8adc98a
ms.openlocfilehash: d2d21fb5546d36990d69b76e3ceb72ce2edf3d80
ms.sourcegitcommit: dd43cc0a9470f98b8ef2a3787c823801d674c666
ms.translationtype: MT
ms.contentlocale: bg-BG
ms.lasthandoff: 02/12/2019
ms.locfileid: "29933469"
---
Имате ли проблеми с **Данни загуба предотвратяване (DLP)** не работи за съдържание, съдържащи **Социално-осигурителен номер (SSN)** , когато използвате тип поверителна информация в Office 365? Ако е така, се уверете, че вашето съдържание съдържа необходимата информация за това, което политиката на DLP търси. 
  
Например за SSN политика, конфигуриран с ниво на доверие от 85 %, по-долу се оценяват и трябва да бъде открит за да задейства правилото:
  
- **[Формат:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#format-80)** 9 цифри, които могат да бъдат в форматиран или неформатиран модел 
    
- **[Модел:](https://msconnect.microsoft.com/https:/docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#pattern-80)** Четири функции търсите SSNs в четири различни модели: 
    
  - Func_ssn намира SSNs с предварително-2011 силно форматиране, които са форматирани с тирета или помещения (ddd дд Асен или ddd dd дддд)
    
  - Func_unformatted_ssn намира SSNs с предварително-2011 силно форматиране, които са неформатирани като девет поредни цифри (ddddddddd)
    
  - Func_randomized_formatted_ssn намира пост-2011 SSNs, които са форматирани с тирета или помещения (ddd дд Асен или ddd dd дддд)
    
  - Func_randomized_unformatted_ssn намира пост-2011 SSNs, които са неформатирани като девет поредни цифри (ddddddddd)
    
- **[Контролна сума:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#checksum-79)** Не, няма никакъв шах 
    
- **[Дефиниция:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#definition-80)** DLP политика е 85 % уверени, че е открил този вид чувствителна информация ако, в рамките на близост на 300 знака: 
    
  - [Функцията Func_ssn](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#pattern-80) намира съдържание, което съвпада с модела. 
    
  - Ключова дума от [Keyword_ssn](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#keyword_ssn) е намерен. Примери за ключови думи включва: *социалното осигуряване, социално осигуряване #, Soc Sec, SSN* . Например, следните примерни ще предизвика на DLP SSN политика: **SSN: 489-36-8350**
    
За повече информация относно това, което се изисква за SSNs да бъдат открити за вашето съдържание, вижте следващия раздел в тази статия: [Какво чувствителна информация типове търси SSNs](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#us-social-security-number-ssn)
  
Използване на тип на различни вградени чувствителна информация, вижте следната статия за повече информация относно какво е необходимо за други типове: [Какво чувствителна информация типове търси](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for)
  

