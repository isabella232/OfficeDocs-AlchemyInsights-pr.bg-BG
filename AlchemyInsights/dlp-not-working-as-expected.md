---
title: DLP не работи според очакванията
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
- "1241"
- "3200001"
ms.assetid: f6fcf5ad-55a1-4f25-af27-1f7c1ce06409
ms.openlocfilehash: e1049f160a9b92040095b6725fa5771218a0956d17f99ea8a6e9cc279e7c73f6
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: bg-BG
ms.lasthandoff: 08/05/2021
ms.locfileid: "54079691"
---
# <a name="dlp-not-working-as-expected"></a>DLP не работи според очакванията

**Важно**: през тези безпрецедентни времена ние предприемаме стъпки, за да гарантираме, че услугите на SharePoint Online и OneDrive остават на пълно разположение – за повече информация посетете [Временни корекции на функции на SharePoint Online](https://aka.ms/ODSPAdjustments).

 **Настройване на DLP**

Имате проблеми с предотвратяването **на загуба на данни (DLP)** в Office 365 не работи по очаквания начин? Ако е така, уверете се, че **вашите DLP** правила са настроени правилно и че вашите данни съдържат това, което **DLP** правилата търсят, когато се оценяват.
  
Правилата за DLP ви позволяват да идентифицирате и защитите поверителна информация във вашата организация. За да настроите DLP правила, използвайте информацията [тук](https://docs.microsoft.com/microsoft-365/compliance/create-a-dlp-policy-from-a-template).
  
 **Какво търси DLP правила**
  
Когато използвате **вградените типове поверителна информация** в центровете за защита и съответствие, правилата за DLP потърсете конкретни модели и елементи, когато откриват тези чувствителни типове.
  
- **Вградени типове поверителна информация**

    За информация за вградените типове поверителна информация и какво търси DLP правилата при откриване на типа "Чувствителна", [вижте:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions)Какво търси типовете поверителна информация .

- **Типове поверителна информация по избор**

    Ако се опитвате да създадете типове поверителна информация по избор, използвайте следната статия за информация как да създадете потребителски тип поверителна информация: [Създаване на тип поверителна информация по избор](https://docs.microsoft.com/microsoft-365/compliance/create-a-custom-sensitive-information-type).

**Тестване на DLP правила**

За да тествате данните си с вграден или  персонализиран тип поверителна информация, използвайте опцията Тип тест под **Типове поверителна информация**  >  **за класификации.** За повече информация вижте Тестване на [типове поверителна информация по избор.](https://docs.microsoft.com/microsoft-365/compliance/create-a-custom-sensitive-information-type#create-custom-sensitive-information-types-in-the-security--compliance-center)

 **Отчети**
  
- Получете информация за поверителни данни с [DLP отчети.](https://docs.microsoft.com/microsoft-365/compliance/data-loss-prevention-policies#dlp-reports)

- Вижте конкретни подробности за събитието с отчет [за инцидент.](https://docs.microsoft.com/microsoft-365/compliance/data-loss-prevention-policies#incident-reports)
