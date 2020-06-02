---
title: DLP правило за SSN не работи
ms.author: deniseb
author: denisebmsft
manager: laurawi
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1242"
- "3200001"
ms.assetid: ac265ee6-c946-476e-9bf0-0ea0e8adc98a
ms.openlocfilehash: 35859bce89ef1ae9b6a9e706fc316b0ee6cd27d1
ms.sourcegitcommit: bc7d6f4f3c9f7060d073f5130e1ec856e248d020
ms.translationtype: MT
ms.contentlocale: bg-BG
ms.lasthandoff: 06/02/2020
ms.locfileid: "44507359"
---
# <a name="dlp-issues-with-social-security-numbers"></a>Проблеми с DLP с номера на социална осигуровка

**Важно**: през тези безпрецедентни времена ние предприемаме стъпки, за да гарантираме, че услугите на SharePoint Online и OneDrive остават на пълно разположение – за повече информация посетете [Временни корекции на функции на SharePoint Online](https://aka.ms/ODSPAdjustments).

**Проблеми с DLP с SSN**

Имате проблеми с **предотвратяване на загуба на данни (DLP)** не работи за съдържание, съдържащо **социално-осигурителен номер (SSN),** когато използвате чувствителен тип информация в Microsoft 365? Ако е така, уверете се, че съдържанието съдържа необходимата информация за това, което се търси от правилата на DLP. 
  
Например за SSN правила конфигурирани с ниво на доверие 85%, се оценяват следното и трябва да бъдат открити за правило за задействане:
  
- **[Формат:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#format-80)** 9 цифри, които могат да бъдат във формат или неформатиран модел

- **[Модел:](https://msconnect.microsoft.com/https:/docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#pattern-80)** Четири функции търсят SSN в четири различни модела:

  - Func_ssn намира SSNs с форматиране преди 2011 г., които са форматирани с тирета или интервали (ddd-dddd ИЛИ DDD ddd dddd)

  - Func_unformatted_ssn намира SSN с форматиране преди 2011 г., които не са форматирани като девет последователни цифри (ddddddddddddddd)

  - Func_randomized_formatted_ssn намира след 2011 SSNs, които са форматирани с тирета или интервали (ddd-dddd ИЛИ DDD DDD)

  - Func_randomized_unformatted_ssn намира след 2011 SSNs, които са неформатирани като девет последователни цифри (ddddddddddddddddd

- **[Контролна сума:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#checksum-79)** Не, няма контролна сума

- **[Определение:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#definition-80)** DLP политика е 85% уверени, че е открита този тип чувствителна информация, ако в близост до 300 знака:

  - [Функцията Func_ssn](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#pattern-80) намира съдържание, което съответства на модела.

  - Намерена е ключова дума от [Keyword_ssn.](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#keyword_ssn) Примерите за ключови думи включват: *Социална сигурност, Социална сигурност# Soc Sec, SSN.* Например следната проба ще задейства DLP SSN политика: **SSN: 489-36-8350**
  
За повече информация относно това, което е необходимо за SSN да бъдат открити за вашето съдържание вижте следния раздел в тази статия: [Какви типове информация за чувствителна изглежда за SSN](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#us-social-security-number-ssn)
  
С помощта на друг вграден тип поверителна информация вижте следната статия за информация за това какво е необходимо за други типове: [Какво се търси типовете информация за чувствителната информация](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions)
  