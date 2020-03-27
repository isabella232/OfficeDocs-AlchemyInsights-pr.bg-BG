---
title: DLP не работи според очакванията
ms.author: deniseb
author: denisebmsft
manager: laurawi
ms.date: 1/9/2019
ms.audience: ITPro
ms.topic: article
ms.prod: office-online-server
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1241"
- "3200001"
ms.assetid: f6fcf5ad-55a1-4f25-af27-1f7c1ce06409
ms.openlocfilehash: 574a8a43d8264e98c6af2bfeb1bb472475e6e334
ms.sourcegitcommit: d108a2da2f5dab05246e30b5108cca5173e09051
ms.translationtype: MT
ms.contentlocale: bg-BG
ms.lasthandoff: 03/26/2020
ms.locfileid: "42977427"
---
# <a name="dlp-not-working-as-expected"></a>DLP не работи според очакванията

**Важно**: По време на тези безпрецедентни времена, ние предприемаме стъпки, за да се гарантира, че SharePoint Online и OneDrive услуги остават високо достъпни – посетете [SharePoint Online временни функция корекции](https://aka.ms/ODSPAdjustments) за повече информация.

 **Настройване на DLP**

Имате проблеми с **предотвратяване на загуба на данни (DLP)** в Office 365 не работи според очакванията? Ако е така, уверете се, че **вашите DLP правила** е настроен правилно и че вашите данни съдържа това, което се търси **dlp правила,** когато се оценява.
  
DLP правилата ви позволяват да идентифицирате и защитавате поверителна информация във вашата организация. За да настроите DLP правила, използвайте информацията [тук](https://docs.microsoft.com/office365/securitycompliance/prevent-data-loss#set-up-dlp).
  
 **Какви dlp политики търсят**
  
Когато използвате **вградените поверителни типове информация** в центъра за защита и съответствие на Office 365, DLP правила търсят конкретни модели и елементи при откриване на тези типове.
  
- **Вградени типове поверителна информация**

    За информация относно вградените типове чувствителни и какво търси правилото на DLP при откриване на типа "Чувствителен", вижте: [Какво търсят типовете поверителна информация за](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for).

- **Типове поверителни по избор информация**

    Ако се опитвате да създадете потребителски поверителни типове информация, използвайте следната статия за информация как да създадете персонализиран тип на поверителна [информация: Създаване на потребителски поверителен тип информация](https://docs.microsoft.com/office365/securitycompliance/create-a-custom-sensitive-information-type).

**Проверка на DLP правила**

За да тествате данните си с вграден или персонализиран тип информация, използвайте опцията **Тип тест** под **Класификация** > **Sensitive видове информация**. За повече информация вижте [Тестване на персонализирани типове информация за поверителни информация](https://docs.microsoft.com/office365/securitycompliance/create-a-custom-sensitive-information-type#test-custom-sensitive-information-types-in-the-security--compliance-center).

 **Доклади**
  
- Получете аналитични данни за конфиденциални данни с [DLP отчети.](https://docs.microsoft.com/office365/securitycompliance/data-loss-prevention-policies#dlp-reports)

- Вижте конкретни подробности за събитието с [доклад за инцидент .](https://docs.microsoft.com/office365/securitycompliance/data-loss-prevention-policies#incident-reports)
