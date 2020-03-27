---
title: DLP правило за САЩ/Великобритания номер на паспорт не работи
ms.author: deniseb
author: denisebmsft
manager: laurawi
ms.date: 11/5/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1319"
- "3200001"
ms.assetid: fc178b8b-943b-4346-a2bd-a75c6af6f80f
ms.openlocfilehash: 534e258c31a9a71c618765511487487c53f455b5
ms.sourcegitcommit: d108a2da2f5dab05246e30b5108cca5173e09051
ms.translationtype: MT
ms.contentlocale: bg-BG
ms.lasthandoff: 03/26/2020
ms.locfileid: "42977095"
---
# <a name="problems-with-dlp---usuk-passport-numbers"></a><span data-ttu-id="737be-102">Проблеми с DLP - САЩ /UK номера на паспорти</span><span class="sxs-lookup"><span data-stu-id="737be-102">Problems with DLP - US/UK passport numbers</span></span>

<span data-ttu-id="737be-103">**Важно**: По време на тези безпрецедентни времена, ние предприемаме стъпки, за да се гарантира, че SharePoint Online и OneDrive услуги остават високо достъпни – посетете [SharePoint Online временни функция корекции](https://aka.ms/ODSPAdjustments) за повече информация.</span><span class="sxs-lookup"><span data-stu-id="737be-103">**Important**: During these unprecedented times, we are taking steps to ensure that SharePoint Online and OneDrive services remain highly available – Please visit [SharePoint Online Temporary Feature Adjustments](https://aka.ms/ODSPAdjustments) for more information.</span></span>

<span data-ttu-id="737be-104">**DLP проблеми с американски/великобритания паспортни номера**</span><span class="sxs-lookup"><span data-stu-id="737be-104">**DLP issues with US/UK passport numbers**</span></span>

<span data-ttu-id="737be-105">Имате проблеми с **предотвратяване на загуба на данни (DLP)** не работи за съдържание, съдържащо номер на **американски/английски паспорт** при използване на тип на чувствителна тайнствена ИНФОРМАЦИЯ DLP в O365?</span><span class="sxs-lookup"><span data-stu-id="737be-105">Are you having problems with **Data Loss Prevention (DLP)** not working for content containing a **US/UK passport number** when using a DLP sensitive information type in O365?</span></span> <span data-ttu-id="737be-106">Ако е така, уверете се, че съдържанието ви съдържа необходимата информация за това, което се търси dlp правила, когато се оценява.</span><span class="sxs-lookup"><span data-stu-id="737be-106">If so, make sure your content contains the needed information for what the DLP policy is looking for when it is evaluated.</span></span>
  
<span data-ttu-id="737be-107">Например, за политика за **номер на паспорт сащ/Обединеното кралство,** конфигурирана с ниво на сигурност от 75%, се оценяват следните и трябва да бъдат открити, за да се задейства правилото</span><span class="sxs-lookup"><span data-stu-id="737be-107">For example, for a **US/UK passport number** policy configured with a confidence level of 75%, the following are evaluated and must be detected for the rule to trigger</span></span>
  
- <span data-ttu-id="737be-108">**[Формат на](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#format-77)** Девет цифри</span><span class="sxs-lookup"><span data-stu-id="737be-108">**[Format:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#format-77)** Nine digits</span></span>

- <span data-ttu-id="737be-109">**[Модел:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#pattern-77)** Девет последователни цифри</span><span class="sxs-lookup"><span data-stu-id="737be-109">**[Pattern:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#pattern-77)** Nine consecutive digits</span></span>

- <span data-ttu-id="737be-110">**[Контролна сума:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#checksum-76)** Не, няма чексума</span><span class="sxs-lookup"><span data-stu-id="737be-110">**[Checksum:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#checksum-76)** No, there is no Checksum</span></span>

- <span data-ttu-id="737be-111">**[Определение:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#definition-77)** DLP политика е 75% уверен, че е открит този тип чувствителна информация, ако в близост до 300 знака:</span><span class="sxs-lookup"><span data-stu-id="737be-111">**[Definition:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#definition-77)** A DLP policy is 75% confident that it's detected this type of sensitive information if, within a proximity of 300 characters:</span></span>

  - <span data-ttu-id="737be-112">Функцията Func_usa_uk_passport намира съдържание, което съответства на шаблона.</span><span class="sxs-lookup"><span data-stu-id="737be-112">The function Func_usa_uk_passport finds content that matches the pattern.</span></span>

  - <span data-ttu-id="737be-113">Намира се ключова дума от Keyword_passport.</span><span class="sxs-lookup"><span data-stu-id="737be-113">A keyword from Keyword_passport is found.</span></span>

    <span data-ttu-id="737be-114">Например следната извадка ще задейства за **САЩ/Великобритания паспорт номер** политика: Номер на паспорт а в САЩ 123456789</span><span class="sxs-lookup"><span data-stu-id="737be-114">For example, the following sample would trigger for the **US/UK passport number** policy: U.S. Passport number 123456789</span></span>

<span data-ttu-id="737be-115">За повече информация относно това, което е необходимо за да бъде открит номер на американски/британски паспорт за вашето съдържание, вижте раздела по-долу в тази статия: [Какви типове информация за сащ/Великобритания търсят за сащ/UK Passport Number](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#us--uk-passport-number)</span><span class="sxs-lookup"><span data-stu-id="737be-115">For more information on what is required for a US/UK Passport Number to be detected for your content, see the following section in this article: [What the Sensitive Information Types look for US/UK Passport Number](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#us--uk-passport-number)</span></span>
  
<span data-ttu-id="737be-116">Използвайки друг вграден тип поверителна информация, вижте следната статия за информация за това какво се изисква за други типове: [Какво търсят типовете поверителна информация за](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for)</span><span class="sxs-lookup"><span data-stu-id="737be-116">Using a different built-in sensitive information type, see the following article for information on what is required for other types: [What the Sensitive Information Types look for](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for)</span></span>
  