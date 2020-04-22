---
title: DLP правило за сащ номер на парични средства не работи
ms.author: deniseb
author: denisebmsft
manager: laurawi
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1287"
- "3200001"
ms.assetid: 80b40145-8376-4c3a-8d22-6efb9f9cb271
ms.openlocfilehash: 45aa50f6c3505468e902e58faf698205f93f9264
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: bg-BG
ms.lasthandoff: 04/22/2020
ms.locfileid: "43704028"
---
# <a name="dlp-issues-with-us-bank-account-numbers"></a>DLP проблеми с номера на банкови сметки в САЩ

**Важно**: през тези безпрецедентни времена ние предприемаме стъпки, за да гарантираме, че услугите на SharePoint Online и OneDrive остават на пълно разположение – за повече информация посетете [Временни корекции на функции на SharePoint Online](https://aka.ms/ODSPAdjustments).

**DLP проблеми с номера на банкови сметки в САЩ**

Имате проблеми с **предотвратяване на загуба на данни (DLP)** не работи за съдържание, съдържащо номер на банкова сметка в **САЩ** при използване на тип на чувствителна тайнствена ИНФОРМАЦИЯ DLP в O365? Ако е така, уверете се, че съдържанието ви съдържа необходимата информация за това, което се търси dlp правила, когато се оценява.
  
Например за политика на **парични тет,** конфигурирани с ниво на сигурност от 85%, се оценяват следното и трябва да бъдат открити за правилото да се задейства:
  
- **[Формат:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#format-77)** 8-17 цифри

- **[Модел:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#pattern-77)** 8-17 последователни цифри.

- **[Контролна сума:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#checksum-76)** Не, няма чексума

- **[Определение:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for)** DLP политика е 75% уверен, че е открит този тип чувствителна информация, ако в близост до 300 знака:

  - Регулярният израз Regex_usa_bank_account_number намира съдържание, което съответства на

  - Намира се ключова дума от Keyword_usa_Bank_Account.

    Например следните примерни ще предизвика за сащ **парични номера** политика: проверка на акаунт 78344011

За повече информация за това, какво е необходимо за да бъде открит **номер на банкова сметка** в САЩ за вашето съдържание, вижте раздела в тази статия: Какъв вид информация за [чувствителна тава търси за номер на банкова сметка в САЩ](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#us-bank-account-number)
  
Използвайки друг вграден тип поверителна информация, вижте следната статия за информация за това какво се изисква за други типове: [Какво търсят типовете поверителна информация за](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for)
  