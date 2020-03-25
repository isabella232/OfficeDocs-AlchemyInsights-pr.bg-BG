---
title: DLP правило за SSN не работи
ms.author: deniseb
author: denisebmsft
manager: laurawi
ms.date: 11/5/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1242"
- "3200001"
ms.assetid: ac265ee6-c946-476e-9bf0-0ea0e8adc98a
ms.openlocfilehash: 0b83a858975ffe1bb70f16a7452a13d57dff5340
ms.sourcegitcommit: b0d5b68366028abcf08610672d5bc9d3b25ac433
ms.translationtype: MT
ms.contentlocale: bg-BG
ms.lasthandoff: 03/24/2020
ms.locfileid: "42932510"
---
# <a name="dlp-issues-with-social-security-numbers"></a>DLP проблеми с номера на социална сигурност

**Важно:** много sharePoint Online и OneDrive клиенти работят критични бизнес приложения срещу услугата, която се изпълнява във фонов режим. Те включват миграция на съдържанието, предотвратяване на загуба на данни (DLP) и архивиране на решения. По време на тези безпрецедентни времена ние предприемаме стъпки, за да гарантираме, че SharePoint Online и OneDrive услуги остават високо достъпни и надеждни за вашите потребители, които зависят от услугата повече от всякога в отдалечени работни сценарии.

В подкрепа на тази цел, ние сме внедрили по-строги ограничения за ограничаване на приложенията за фон (миграция, DLP и архивиране на решения) през делничните дни. Трябва да очаквате, че тези приложения ще постигнат много ограничена пропускателна информация по време на тези времена. Въпреки това, по време на вечерните и почивните часове за региона, услугата ще бъде готова да обработи значително по-голям обем заявки от приложения за фон.

**Проблеми с dlp с SSN**

Имате проблеми с **предотвратяване на загуба на данни (DLP)** не работи за съдържание, съдържащо номер за социална сигурност **(SSN),** когато използвате поверителна информация тип в Office 365? Ако е така, уверете се, че съдържанието ви съдържа необходимата информация за това, което се търси dlp правилата. 
  
Например за SSN правила, конфигурирани с ниво на сигурност 85 %, се оценяват следното и трябва да бъдат открити за правилото за задействане:
  
- **[Формат:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#format-80)** 9 цифри, които може да са във формат или неформатиран модел

- **[Модел:](https://msconnect.microsoft.com/https:/docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#pattern-80)** Четири функции търсят SSN в четири различни модела:

  - Func_ssn намира SSN със силно форматиране преди 2011 г., форматирани с тирета или интервали (ddd-dddddd ddddd ddddd ddddd dddddddddddddddddddddddddddddddddddddddd)

  - Func_unformatted_ssn открива SSN с предварително 2011 силно форматиране, които са неформатирани като девет последователни цифри (ddddddddddddddddddddddddddddddddddddddddddddddddddd

  - Func_randomized_formatted_ssn намира след 2011 SSN, които са форматирани с тирета или интервали (ddd-dddddd или ddd ddd dddd dddd dddddd)

  - Func_randomized_unformatted_ssn намира след 2011 SSN, които са неформатирани като девет последователни цифри (ddddddddddd)

- **[Контролна сума:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#checksum-79)** Не, няма чексума

- **[Определение:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#definition-80)** DLP политика е 85% уверен, че е открит този тип чувствителна информация, ако в близост до 300 знака:

  - [Функцията Func_ssn](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#pattern-80) намира съдържание, което съответства на шаблона.

  - Намира се ключова дума от [Keyword_ssn.](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#keyword_ssn) Сред ключовите думи са: *Социална сигурност, Социална осигуровка#, Soc Sec, SSN.* Например следната извадка ще предизвика за DLP SSN **политика: SSN: 489-36-8350**
  
За повече информация за това какво се изисква за SSN да бъдат открити за вашето съдържание вижте следния раздел в тази статия: [Какви типове поверителна информация търси SSN](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#us-social-security-number-ssn)
  
Използвайки друг вграден тип поверителна информация, вижте следната статия за информация за това какво се изисква за други типове: [Какво търсят типовете поверителна информация за](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for)
  