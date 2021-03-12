---
title: DLP не работи по очаквания начин
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
ms.openlocfilehash: 0f07e64c95675a4f6a0aeb6df110fe4e6a21d72f
ms.sourcegitcommit: 0eb4f9bde53395b5fd4b5cd4ffc56ca96db91298
ms.translationtype: MT
ms.contentlocale: bg-BG
ms.lasthandoff: 03/10/2021
ms.locfileid: "50707799"
---
# <a name="dlp-not-working-as-expected"></a>DLP не работи по очаквания начин

**Важно**: през тези безпрецедентни времена ние предприемаме стъпки, за да гарантираме, че услугите на SharePoint Online и OneDrive остават на пълно разположение – за повече информация посетете [Временни корекции на функции на SharePoint Online](https://aka.ms/ODSPAdjustments).

 **Настройване на DLP**

Имате ли проблеми с **предотвратяване на загуба на данни (DLP)** в Office 365 не работи, както се очаква? Ако е така, уверете се, че вашата **DLP политика** е настроена правилно и че вашите данни съдържат това, което се намира в **DLP политиката** , когато тя се изчислява.
  
DLP правила ви позволява да идентифицирате и защитавате поверителната информация във вашата организация. За да настроите DLP правила, използвайте информацията [тук](https://docs.microsoft.com/microsoft-365/compliance/create-a-dlp-policy-from-a-template).
  
 **Какви правила за DLP търсят**
  
Когато използвате **вградените типове деликатни данни** в центъра за защита и съответствие, DLP правилата търсят определени модели и елементи, когато откриват тези типове чувствителни.
  
- **Вградени типове деликатни данни**

    За информация относно вградените типове чувствителни и за това какво търси DLP политика при откриването на типа чувствителна, вижте: [какви типове чувствителна информация търсите](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions).

- **Типове чувствителна информация по избор**

    Ако се опитвате да създадете типове чувствителна информация по избор, използвайте следната статия за информация как да създадете персонализиран тип чувствителна информация: [Създаване на персонализиран тип данни по избор](https://docs.microsoft.com/microsoft-365/compliance/create-a-custom-sensitive-information-type).

**Тестване на DLP правила**

За да тествате вашите данни с помощта на вграден или персонализиран тип информация, използвайте опцията **тип** на теста **под**  >  **типове чувствителна информация**. За повече информация вижте [проверка на типовете чувствителна информация по избор](https://docs.microsoft.com/microsoft-365/compliance/create-a-custom-sensitive-information-type#create-custom-sensitive-information-types-in-the-security--compliance-center).

 **Отчети**
  
- Получете данни за чувствителна информация с [DLP отчети.](https://docs.microsoft.com/microsoft-365/compliance/data-loss-prevention-policies#dlp-reports)

- Вижте конкретни подробности за събитието със съобщение за [инцидент](https://docs.microsoft.com/microsoft-365/compliance/data-loss-prevention-policies#incident-reports).
