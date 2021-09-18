---
title: DLP може да се нуждае от тип по избор
ms.author: pebaum
author: pebaum
manager: laurawi
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1647"
- "3200001"
ms.assetid: ''
ms.openlocfilehash: c0996e0cc923c13b7de3752ac6534026e8627c51
ms.sourcegitcommit: dcd1c76ced1a0cec27f4cf8d383593760c198424
ms.translationtype: MT
ms.contentlocale: bg-BG
ms.lasthandoff: 09/18/2021
ms.locfileid: "59446680"
---
# <a name="dlp-might-need-a-custom-type"></a>DLP може да се нуждае от тип по избор

**Важно**: през тези безпрецедентни времена ние предприемаме стъпки, за да гарантираме, че услугите на SharePoint Online и OneDrive остават на пълно разположение – за повече информация посетете [Временни корекции на функции на SharePoint Online](https://aka.ms/ODSPAdjustments).

**DLP може да изисква тип информация по избор**

С правилата за защита от загуба на данни (DLP) можете да идентифицирате и защитите поверителни данни във вашата организация. В някои случаи може да се наложи да създадете свой собствен тип поверителна информация по избор, за да защитите данните на вашата организация. За повече информация вижте [Научете повече за типовете поверителна информация и](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-learn-about) дефинициите [на обекта тип поверителна информация.](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions)

За повече информация как да създадете типове и правила за поверителна информация по избор, вижте: 

**Персонализиране на вграден чувствителен тип информация**

Ако вграденият тип поверителна информация отговаря на вашите нужди само с няколко ощипвания, вижте Персонализиране на вграден [тип поверителна информация](https://docs.microsoft.com/microsoft-365/compliance/customize-a-built-in-sensitive-information-type). Можете например да добавяте или премахвате ключови думи или да добавяте или премахвате поддържащи доказателства, като например дата или адрес.

**Създаване на тип поверителна информация по избор**

Но ако трябва да идентифицирате и защитите напълно различен тип поверителна информация, можете да създадете потребителски тип поверителна информация в Център за съответствие на Microsoft 365. За повече информация вижте Първи [стъпки в типовете поверителна информация по избор.](https://docs.microsoft.com/microsoft-365/compliance/customize-a-built-in-sensitive-information-type)

**Създаване на тип поверителна информация по избор в центъра за & съответствие на PowerShell**

И накрая, ако потребителският интерфейс не предоставя всички необходими опции, можете да създадете потребителски тип поверителна информация в центъра за & съответствие PowerShell. Като започнете с XML файл, можете да използвате всяка налична опция. За повече информация вижте Създаване на [тип поверителна информация по избор с помощта на PowerShell](https://docs.microsoft.com/microsoft-365/compliance/create-a-custom-sensitive-information-type-in-scc-powershell).

За да тествате първо правилата [](https://docs.microsoft.com/microsoft-365/compliance/dlp-learn-about-dlp#implement-policy-in-test-mode) си в тестов режим, вижте Прилагане на правила в режим на тестване и Създаване, тестване и [настройване на DLP правила.](https://docs.microsoft.com/microsoft-365/compliance/create-test-tune-dlp-policy) 