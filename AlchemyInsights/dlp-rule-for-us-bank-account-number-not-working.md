---
title: DLP правило за номер на банкова сметка в САЩ не работи
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
- "1287"
- "3200001"
ms.assetid: 80b40145-8376-4c3a-8d22-6efb9f9cb271
ms.openlocfilehash: d19b2dcc29e23fab522159945496165338a117a47bfcfcadf0b93e4e5f14464f
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: bg-BG
ms.lasthandoff: 08/05/2021
ms.locfileid: "54005007"
---
# <a name="dlp-issues-with-us-bank-account-numbers"></a>Проблеми с DLP с номера на банкови сметки в САЩ

**Важно**: през тези безпрецедентни времена ние предприемаме стъпки, за да гарантираме, че услугите на SharePoint Online и OneDrive остават на пълно разположение – за повече информация посетете [Временни корекции на функции на SharePoint Online](https://aka.ms/ODSPAdjustments).

**Проблеми с DLP с номера на банкови сметки в САЩ**

Имате проблеми с предотвратяването на загуба на данни **(DLP)** не работи за съдържание, съдържащо номер на банкова сметка в САЩ, когато използвате тип информация за DLP поверителна информация в O365?  Ако е така, уверете се, че съдържанието ви съдържа необходимата информация за това, което търси DLP правилата, когато се оценява.
  
Например за правила  за номер на банкова сметка в САЩ, конфигурирани с доверително ниво от 85%, се оценяват следните и трябва да бъдат открити, за да се задейства правилото:
  
- **[Формат:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#format-77)** 8-17 цифри

- **[Шарка:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#pattern-77)** 8-17 последователни цифри.

- **[Контролна карта:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#checksum-76)** Не, няма контролна карта

- **[Дефиниция:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions)** Правилата за DLP са 75% уверени, че са открити този тип поверителна информация, ако в близост до 300 знака:

  - Обикновеният израз Regex_usa_bank_account_number намира съдържание, което отговаря на модела

  - Намерена е ключова дума Keyword_usa_Bank_Account за търсене.

    Например следната извадка ще се задейства за правилата за номер на банкова **сметка в** САЩ: Проверка на 78344011

За повече информация какво е  необходимо за откриване на номер на банкова сметка в САЩ за вашето съдържание, вижте следващия раздел в тази статия: Какво търси типовете поверителна информация [за номера на банкова](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#us-bank-account-number) сметка в САЩ
  
Като използвате различен вграден тип поверителна информация, вижте следната статия за информация какво е необходимо за други типове: [Какво търси типовете поверителна информация](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions)
  