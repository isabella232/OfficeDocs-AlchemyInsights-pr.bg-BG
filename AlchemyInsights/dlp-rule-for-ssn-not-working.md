---
title: DLP правилото за SSN не работи
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
- "1242"
- "3200001"
ms.assetid: ac265ee6-c946-476e-9bf0-0ea0e8adc98a
ms.openlocfilehash: 3f30998fb3bc4c5442e4e1541b87d88ecd7df6eef3a50e719fa5014eb86af39c
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: bg-BG
ms.lasthandoff: 08/05/2021
ms.locfileid: "54004971"
---
# <a name="dlp-issues-with-social-security-numbers"></a>Проблеми с DLP с номера на социална осигуровка

**Важно**: през тези безпрецедентни времена ние предприемаме стъпки, за да гарантираме, че услугите на SharePoint Online и OneDrive остават на пълно разположение – за повече информация посетете [Временни корекции на функции на SharePoint Online](https://aka.ms/ODSPAdjustments).

**DLP проблеми с SSN**

Имате проблеми с предотвратяването на загуба на данни **(DLP)** не работи за съдържание, съдържащо номер на социална осигуровка **(SSN),** когато използвате чувствителен тип информация в Microsoft 365? Ако е така, уверете се, че съдържанието ви съдържа необходимата информация за това, което търси DLP правилата. 
  
Например за SSN правила, конфигурирани с доверително ниво от 85%, се оценяват следните и трябва да бъдат открити, за да се задейства правилото:
  
- **[Формат:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#format-80)** 9 цифри, които може да са във форматиран или неформатиран модел

- **[Шарка:](https://msconnect.microsoft.com/https:/docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#pattern-80)** Четири функции потърсете SSN в четири различни модела:

  - Func_ssn намира SSN мрежи със силно форматиране преди 2011 г., форматирани с тирета или интервали (ddd-dd-dddd OR ddd ddd ddddd)

  - Func_unformatted_ssn намира SSN мрежи със силно форматиране преди 2011 г., които са неформатирани като девет последователни цифри (dddddddd)

  - Func_randomized_formatted_ssn намира SSN мрежи след 2011 г., които са форматирани с тирета или интервали (ddd-dd-dddd OR ddd ddd dddd)

  - Func_randomized_unformatted_ssn намира SSN мрежи след 2011 г., които са неформатирани като девет последователни цифри (dddddddd)

- **[Контролна карта:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#checksum-79)** Не, няма контролна карта

- **[Дефиниция:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#definition-80)** Правилата за DLP са 85% уверени, че са открити този тип поверителна информация, ако в близост до 300 знака:

  - Функцията [Func_ssn](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#pattern-80) намира съдържание, което отговаря на шарката.

  - Намира се ключова [дума от Keyword_ssn.](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#keyword_ssn) Примерите за ключови думи включват:  *Социално осигуряване, Социална осигуровка#, Soc Sec ,SSN*  . Например следната извадка ще задейства за правилата за DLP SSN: **SSN: 489-36-8350**
  
За повече информация какво е необходимо за откриване на SSN за вашето съдържание, вижте следващия раздел в тази статия: Какво търси типовете поверителна [информация за SSN](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#us-social-security-number-ssn)
  
Като използвате различен вграден тип поверителна информация, вижте следната статия за информация какво е необходимо за други типове: [Какво търси типовете поверителна информация](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions)
  