---
title: DLP правило за САЩ / Великобритания паспорт номер не работи
ms.author: cmcatee
author: cmcatee-MSFT
manager: mnirkhe
ms.date: 11/5/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.assetid: fc178b8b-943b-4346-a2bd-a75c6af6f80f
ms.openlocfilehash: 5722f7b6c9a2f905fed2ef4164787e020260edf7
ms.sourcegitcommit: 0ae6cbb8cf2836da98300767ed81b411d6551bee
ms.translationtype: MT
ms.contentlocale: bg-BG
ms.lasthandoff: 01/30/2019
ms.locfileid: "29656412"
---
<span data-ttu-id="d581d-p101">Имате ли проблеми с **Данни загуба предотвратяване (DLP)** не работи за съдържание, съдържащи **САЩ / Великобритания паспорт номер** при използване на тип DLP чувствителна информация в O365? Ако е така, уверете се, че вашето съдържание съдържа необходимата информация за какво е търсенето на DLP политика, когато той се оценява.</span><span class="sxs-lookup"><span data-stu-id="d581d-p101">Are you having problems with **Data Loss Prevention (DLP)** not working for content containing a **US/UK Passport Number** when using a DLP sensitive information type in O365? If so, make sure your content contains the needed information for what the DLP policy is looking for when it is evaluated.</span></span> 
  
<span data-ttu-id="d581d-104">Например, за **САЩ / Великобритания паспорт номер** политика, конфигуриран с ниво на доверие от 75 %, следните се оценяват и трябва да бъдат открити за да задейства правилото</span><span class="sxs-lookup"><span data-stu-id="d581d-104">For example, for a **US/UK Passport Number** policy configured with a confidence level of 75%, the following are evaluated and must be detected for the rule to trigger</span></span> 
  
- <span data-ttu-id="d581d-105">**[Формат:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#format-77)** Девет цифри</span><span class="sxs-lookup"><span data-stu-id="d581d-105">**[Format:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#format-77)** Nine digits</span></span> 
    
- <span data-ttu-id="d581d-106">**[Модел:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#pattern-77)** Девет поредни цифри</span><span class="sxs-lookup"><span data-stu-id="d581d-106">**[Pattern:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#pattern-77)** Nine consecutive digits</span></span> 
    
- <span data-ttu-id="d581d-107">**[Контролна сума:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#checksum-76)** Не, няма никакъв шах</span><span class="sxs-lookup"><span data-stu-id="d581d-107">**[Checksum:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#checksum-76)** No, there is no Checksum</span></span> 
    
- <span data-ttu-id="d581d-108">**[Дефиниция:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#definition-77)** DLP политика е 75 % уверени, че е открил този вид чувствителна информация ако, в рамките на близост на 300 знака:</span><span class="sxs-lookup"><span data-stu-id="d581d-108">**[Definition:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#definition-77)** A DLP policy is 75% confident that it's detected this type of sensitive information if, within a proximity of 300 characters:</span></span> 
    
  - <span data-ttu-id="d581d-109">Функцията Func_usa_uk_passport открие съдържание, което съвпада с модела.</span><span class="sxs-lookup"><span data-stu-id="d581d-109">The function Func_usa_uk_passport finds content that matches the pattern.</span></span>
    
  - <span data-ttu-id="d581d-110">Ключова дума от Keyword_passport е намерен.</span><span class="sxs-lookup"><span data-stu-id="d581d-110">A keyword from Keyword_passport is found.</span></span>
    
    <span data-ttu-id="d581d-111">Например, следните примерни ще спусък за **САЩ / Великобритания паспорт номер** политика: Паспорт САЩ номер 123456789</span><span class="sxs-lookup"><span data-stu-id="d581d-111">For example, the following sample would trigger for the **US/UK Passport Number** policy: U.S. Passport number 123456789</span></span> 
    
<span data-ttu-id="d581d-112">За повече информация за това, което се изисква за САЩ / Великобритания паспорт номер да бъде открито за съдържанието ви, вижте следващия раздел в тази статия: [Какво чувствителна информация типове поглед за САЩ / Великобритания паспорт номер](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#us--uk-passport-number)</span><span class="sxs-lookup"><span data-stu-id="d581d-112">For more information on what is required for a US/UK Passport Number to be detected for your content, see the following section in this article: [What the Sensitive Information Types look for US/UK Passport Number](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#us--uk-passport-number)</span></span>
  
<span data-ttu-id="d581d-113">Използване на тип на различни вградени чувствителна информация, вижте следната статия за повече информация относно какво е необходимо за други типове: [Какво чувствителна информация типове търси](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for)</span><span class="sxs-lookup"><span data-stu-id="d581d-113">Using a different built-in sensitive information type, see the following article for information on what is required for other types: [What the Sensitive Information Types look for](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for)</span></span>
  

