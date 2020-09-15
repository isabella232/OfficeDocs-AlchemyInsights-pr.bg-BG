---
title: DLP правило за социална ОСИГУРОВКА не работи
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
ms.openlocfilehash: b221e66862ca01074f380fbb8433f8f9cac044cb
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: bg-BG
ms.lasthandoff: 09/14/2020
ms.locfileid: "47679358"
---
# <a name="dlp-issues-with-social-security-numbers"></a>DLP проблеми със социални осигуровки

**Важно**: през тези безпрецедентни времена ние предприемаме стъпки, за да гарантираме, че услугите на SharePoint Online и OneDrive остават на пълно разположение – за повече информация посетете [Временни корекции на функции на SharePoint Online](https://aka.ms/ODSPAdjustments).

**DLP проблеми с SSNs**

Имате ли проблеми при **предотвратяване на загуба на данни (DLP)** , които не работят за съдържание, съдържащо **номер на социална осигуровка (социална осигуровка)** , когато използвате чувствителна информация в Microsoft 365? Ако е така, трябва да се уверите, че вашето съдържание съдържа нужната информация за това, което търси DLP политиката. 
  
Например за правилата на социална ОСИГУРОВКА, конфигурирани с ниво на надеждност от 85%, следва да бъдат оценени следните неща и трябва да бъдат открити, за да се задейства правилото:
  
- **[Формат:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#format-80)** 9 цифри, които може да са в форматиран или неформатиран модел

- **[Шарка:](https://msconnect.microsoft.com/https:/docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#pattern-80)** Четирите функции търсят SSNs в четири различни модела:

  - Func_ssn намира SSNs с предварително 2011 силно форматиране, което се форматира с тирета или интервали (ДДД-дд-Асен или ДДД дд Асен)

  - Func_unformatted_ssn намира SSNs с предварително 2011 силно форматиране, което е неформатирано като девет последователни цифри (ddddddddd)

  - Func_randomized_formatted_ssn намира Post-2011 SSNs, които са форматирани с тирета или интервали (ДДД-дд-Асен или ДДД дд Асен)

  - Func_randomized_unformatted_ssn намира Post-2011 SSNs, които са неформатирани като девет последователни цифри (ddddddddd)

- **[Контролна сума:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#checksum-79)** Не, няма шах

- **[Дефиниция:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#definition-80)** DLP правилата е 85% сигурни, че той е открил този тип поверителна информация, ако в близост до знаците на 300:

  - [Функцията Func_ssn](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#pattern-80) намира съдържание, което съответства на шарката.

  - Намерена е ключова дума от [Keyword_ssn](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#keyword_ssn) . Примерите за ключови думи включват:  *социално осигуряване, социално осигуряване #, SoC сек, социална осигуровка*  . Например примерът по-долу би активирал правилата за DLP социална ОСИГУРОВКА: **социална осигуровка: 489-36-8350**
  
За повече информация за това, което е необходимо, за да бъде открит SSNs за вашето съдържание, вижте раздела по-долу в тази статия: [какви типове чувствителна информация търси SSNs](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#us-social-security-number-ssn)
  
С помощта на различен вграден тип чувствителна информация вижте статията по-долу за информация относно това, което е необходимо за други типове: [какви типове чувствителна информация търсите](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions)
  