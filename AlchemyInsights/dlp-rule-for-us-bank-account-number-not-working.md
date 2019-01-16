---
title: DLP правило за нас банкова сметка номер не работи
ms.author: cmcatee
author: cmcatee-MSFT
manager: mnirkhe
ms.date: 11/5/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.assetid: 80b40145-8376-4c3a-8d22-6efb9f9cb271
ms.openlocfilehash: 6eae9146d33f5fc307085dbf931d57bdbb28b82e
ms.sourcegitcommit: d6ea5e9458a2b8ceaab3ac4bd483e1130b9a398a
ms.translationtype: MT
ms.contentlocale: bg-BG
ms.lasthandoff: 01/15/2019
ms.locfileid: "28276771"
---
<span data-ttu-id="e5f60-p101">Имате ли проблеми с **Данни загуба предотвратяване (DLP)** не работи за съдържание, съдържаща **Номер на банкова сметка на САЩ** , когато използвате тип DLP чувствителна информация в O365? Ако е така, уверете се, че вашето съдържание съдържа необходимата информация за какво е търсенето на DLP политика, когато той се оценява.</span><span class="sxs-lookup"><span data-stu-id="e5f60-p101">Are you having problems with **Data Loss Prevention (DLP)** not working for content containing a **US Bank Account Number** when using a DLP sensitive information type in O365? If so, make sure your content contains the needed information for what the DLP policy is looking for when it is evaluated.</span></span> 
  
<span data-ttu-id="e5f60-104">Например за политика на **САЩ банкова сметка номер** , конфигуриран с ниво на доверие от 85 %, следното се оценяват и трябва да бъде открит за да задейства правилото:</span><span class="sxs-lookup"><span data-stu-id="e5f60-104">For example, for a **US Bank Account Number** policy configured with a confidence level of 85%, the following are evaluated and must be detected for the rule to trigger:</span></span> 
  
- <span data-ttu-id="e5f60-105">**[Формат:](https://docs.microsoft.com/en-us/office365/securitycompliance/what-the-sensitive-information-types-look-for#format-77)** 8-17 цифри</span><span class="sxs-lookup"><span data-stu-id="e5f60-105">**[Format:](https://docs.microsoft.com/en-us/office365/securitycompliance/what-the-sensitive-information-types-look-for#format-77)** 8-17 digits</span></span> 
    
- <span data-ttu-id="e5f60-106">**[Модел:](https://docs.microsoft.com/en-us/office365/securitycompliance/what-the-sensitive-information-types-look-for#pattern-77)** 8-17 поредни цифри.</span><span class="sxs-lookup"><span data-stu-id="e5f60-106">**[Pattern:](https://docs.microsoft.com/en-us/office365/securitycompliance/what-the-sensitive-information-types-look-for#pattern-77)** 8-17 consecutive digits.</span></span> 
    
- <span data-ttu-id="e5f60-107">**[Контролна сума:](https://docs.microsoft.com/en-us/office365/securitycompliance/what-the-sensitive-information-types-look-for#checksum-76)** Не, няма никакъв шах</span><span class="sxs-lookup"><span data-stu-id="e5f60-107">**[Checksum:](https://docs.microsoft.com/en-us/office365/securitycompliance/what-the-sensitive-information-types-look-for#checksum-76)** No, there is no Checksum</span></span> 
    
- <span data-ttu-id="e5f60-108">**[Дефиниция:](https://docs.microsoft.com/en-us/office365/securitycompliance/what-the-sensitive-information-types-look-for)** DLP политика е 75 % уверени, че е открил този вид чувствителна информация ако, в рамките на близост на 300 знака:</span><span class="sxs-lookup"><span data-stu-id="e5f60-108">**[Definition:](https://docs.microsoft.com/en-us/office365/securitycompliance/what-the-sensitive-information-types-look-for)** A DLP policy is 75% confident that it's detected this type of sensitive information if, within a proximity of 300 characters:</span></span> 
    
  - <span data-ttu-id="e5f60-109">Регулярен израз Regex_usa_bank_account_number открие съдържание, което съвпада с модела</span><span class="sxs-lookup"><span data-stu-id="e5f60-109">The regular expression Regex_usa_bank_account_number finds content that matches the pattern</span></span>
    
  - <span data-ttu-id="e5f60-110">Ключова дума от Keyword_usa_Bank_Account е намерен.</span><span class="sxs-lookup"><span data-stu-id="e5f60-110">A keyword from Keyword_usa_Bank_Account is found.</span></span>
    
    <span data-ttu-id="e5f60-111">Например, следните примерни ще спусък за политиката на **САЩ банкова сметка номер** : разплащателна сметка 78344011</span><span class="sxs-lookup"><span data-stu-id="e5f60-111">For example, the following sample would trigger for the **US Bank Account Number** policy: Checking Account 78344011</span></span> 
    
<span data-ttu-id="e5f60-112">За повече информация относно това, което се изисква за **Номер на банкова сметка на САЩ** да бъдат открити за вашето съдържание, вижте следващия раздел в тази статия: [Какво чувствителна типове информация потърсете номер на банкова сметка на САЩ](https://docs.microsoft.com/en-us/office365/securitycompliance/what-the-sensitive-information-types-look-for#us-bank-account-number)</span><span class="sxs-lookup"><span data-stu-id="e5f60-112">For more information on what is required for a **US Bank Account Number** to be detected for your content, see the following section in this article: [What the Sensitive Information Types look for US Bank Account Number](https://docs.microsoft.com/en-us/office365/securitycompliance/what-the-sensitive-information-types-look-for#us-bank-account-number)</span></span>
  
<span data-ttu-id="e5f60-113">Използване на тип на различни вградени чувствителна информация, вижте следната статия за повече информация относно какво е необходимо за други типове: [Какво чувствителна информация типове търси](https://docs.microsoft.com/en-us/office365/securitycompliance/what-the-sensitive-information-types-look-for)</span><span class="sxs-lookup"><span data-stu-id="e5f60-113">Using a different built-in sensitive information type, see the following article for information on what is required for other types: [What the Sensitive Information Types look for](https://docs.microsoft.com/en-us/office365/securitycompliance/what-the-sensitive-information-types-look-for)</span></span>
  

