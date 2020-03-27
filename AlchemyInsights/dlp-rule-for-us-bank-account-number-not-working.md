---
title: DLP правило за сащ номер на парични средства не работи
ms.author: deniseb
author: denisebmsft
manager: laurawi
ms.date: 11/5/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1287"
- "3200001"
ms.assetid: 80b40145-8376-4c3a-8d22-6efb9f9cb271
ms.openlocfilehash: bb7d8ca91af73fa4ebed5992ec848128beb18830
ms.sourcegitcommit: d108a2da2f5dab05246e30b5108cca5173e09051
ms.translationtype: MT
ms.contentlocale: bg-BG
ms.lasthandoff: 03/26/2020
ms.locfileid: "42977151"
---
# <a name="dlp-issues-with-us-bank-account-numbers"></a>DLP проблеми с номера на банкови сметки в САЩ

**Важно**: По време на тези безпрецедентни времена, ние предприемаме стъпки, за да се гарантира, че SharePoint Online и OneDrive услуги остават високо достъпни – посетете [SharePoint Online временни функция корекции](https://aka.ms/ODSPAdjustments) за повече информация.

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
  