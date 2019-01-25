---
title: DLP правило за SSN не работи
ms.author: cmcatee
author: cmcatee-MSFT
manager: mnirkhe
ms.date: 11/5/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.assetid: ac265ee6-c946-476e-9bf0-0ea0e8adc98a
ms.openlocfilehash: b92d122b774d97cd2e44cc0880dc5001065b57cc
ms.sourcegitcommit: e2864efcfb493b6e46b662b746661a61232bdba7
ms.translationtype: MT
ms.contentlocale: bg-BG
ms.lasthandoff: 01/24/2019
ms.locfileid: "29458798"
---
<span data-ttu-id="2969f-p101">Имате ли проблеми с **Данни загуба предотвратяване (DLP)** не работи за съдържание, съдържащи **Социално-осигурителен номер (SSN)** , когато използвате тип поверителна информация в Office 365? Ако е така, се уверете, че вашето съдържание съдържа необходимата информация за това, което политиката на DLP търси.</span><span class="sxs-lookup"><span data-stu-id="2969f-p101">Are you having problems with **Data Loss Prevention (DLP)** not working for content containing a **Social Security Number (SSN)** when using a sensitive information type in Office 365? If so, make sure your content contains the needed information for what the DLP policy is looking.</span></span> 
  
<span data-ttu-id="2969f-104">Например за SSN политика, конфигуриран с ниво на доверие от 85 %, по-долу се оценяват и трябва да бъде открит за да задейства правилото:</span><span class="sxs-lookup"><span data-stu-id="2969f-104">For example, for an SSN policy configured with a confidence level of 85%, the following are evaluated and must be detected for the rule to trigger:</span></span>
  
- <span data-ttu-id="2969f-105">**[Формат:](https://docs.microsoft.com/en-us/office365/securitycompliance/what-the-sensitive-information-types-look-for#format-80)** 9 цифри, които могат да бъдат в форматиран или неформатиран модел</span><span class="sxs-lookup"><span data-stu-id="2969f-105">**[Format:](https://docs.microsoft.com/en-us/office365/securitycompliance/what-the-sensitive-information-types-look-for#format-80)** 9 digits, which may be in a formatted or unformatted pattern</span></span> 
    
- <span data-ttu-id="2969f-106">**[Модел:](https://msconnect.microsoft.com/https:/docs.microsoft.com/en-us/office365/securitycompliance/what-the-sensitive-information-types-look-for#pattern-80)** Четири функции търсите SSNs в четири различни модели:</span><span class="sxs-lookup"><span data-stu-id="2969f-106">**[Pattern:](https://msconnect.microsoft.com/https:/docs.microsoft.com/en-us/office365/securitycompliance/what-the-sensitive-information-types-look-for#pattern-80)** Four functions look for SSNs in four different patterns:</span></span> 
    
  - <span data-ttu-id="2969f-107">Func_ssn намира SSNs с предварително-2011 силно форматиране, които са форматирани с тирета или помещения (ddd дд Асен или ddd dd дддд)</span><span class="sxs-lookup"><span data-stu-id="2969f-107">Func_ssn finds SSNs with pre-2011 strong formatting that are formatted with dashes or spaces (ddd-dd-dddd OR ddd dd dddd)</span></span>
    
  - <span data-ttu-id="2969f-108">Func_unformatted_ssn намира SSNs с предварително-2011 силно форматиране, които са неформатирани като девет поредни цифри (ddddddddd)</span><span class="sxs-lookup"><span data-stu-id="2969f-108">Func_unformatted_ssn finds SSNs with pre-2011 strong formatting that are unformatted as nine consecutive digits (ddddddddd)</span></span>
    
  - <span data-ttu-id="2969f-109">Func_randomized_formatted_ssn намира пост-2011 SSNs, които са форматирани с тирета или помещения (ddd дд Асен или ddd dd дддд)</span><span class="sxs-lookup"><span data-stu-id="2969f-109">Func_randomized_formatted_ssn finds post-2011 SSNs that are formatted with dashes or spaces (ddd-dd-dddd OR ddd dd dddd)</span></span>
    
  - <span data-ttu-id="2969f-110">Func_randomized_unformatted_ssn намира пост-2011 SSNs, които са неформатирани като девет поредни цифри (ddddddddd)</span><span class="sxs-lookup"><span data-stu-id="2969f-110">Func_randomized_unformatted_ssn finds post-2011 SSNs that are unformatted as nine consecutive digits (ddddddddd)</span></span>
    
- <span data-ttu-id="2969f-111">**[Контролна сума:](https://docs.microsoft.com/en-us/office365/securitycompliance/what-the-sensitive-information-types-look-for#checksum-79)** Не, няма никакъв шах</span><span class="sxs-lookup"><span data-stu-id="2969f-111">**[Checksum:](https://docs.microsoft.com/en-us/office365/securitycompliance/what-the-sensitive-information-types-look-for#checksum-79)** No, there is no Checksum</span></span> 
    
- <span data-ttu-id="2969f-112">**[Дефиниция:](https://docs.microsoft.com/en-us/office365/securitycompliance/what-the-sensitive-information-types-look-for#definition-80)** DLP политика е 85 % уверени, че е открил този вид чувствителна информация ако, в рамките на близост на 300 знака:</span><span class="sxs-lookup"><span data-stu-id="2969f-112">**[Definition:](https://docs.microsoft.com/en-us/office365/securitycompliance/what-the-sensitive-information-types-look-for#definition-80)** A DLP policy is 85% confident that it's detected this type of sensitive information if, within a proximity of 300 characters:</span></span> 
    
  - <span data-ttu-id="2969f-113">[Функцията Func_ssn](https://docs.microsoft.com/en-us/office365/securitycompliance/what-the-sensitive-information-types-look-for#pattern-80) намира съдържание, което съвпада с модела.</span><span class="sxs-lookup"><span data-stu-id="2969f-113">The [function Func_ssn](https://docs.microsoft.com/en-us/office365/securitycompliance/what-the-sensitive-information-types-look-for#pattern-80) finds content that matches the pattern.</span></span> 
    
  - <span data-ttu-id="2969f-p102">Ключова дума от [Keyword_ssn](https://docs.microsoft.com/en-us/office365/securitycompliance/what-the-sensitive-information-types-look-for#keyword_ssn) е намерен. Примери за ключови думи включва: *социалното осигуряване, социално осигуряване #, Soc Sec, SSN* . Например, следните примерни ще предизвика на DLP SSN политика: **SSN: 489-36-8350**</span><span class="sxs-lookup"><span data-stu-id="2969f-p102">A keyword from [Keyword_ssn](https://docs.microsoft.com/en-us/office365/securitycompliance/what-the-sensitive-information-types-look-for#keyword_ssn) is found. Examples of keywords includes:  *Social Security, Social Security#, Soc Sec ,SSN*  . For example, the following sample would trigger for the DLP SSN policy: **SSN: 489-36-8350**</span></span>
    
<span data-ttu-id="2969f-117">За повече информация относно това, което се изисква за SSNs да бъдат открити за вашето съдържание, вижте следващия раздел в тази статия: [Какво чувствителна информация типове търси SSNs](https://docs.microsoft.com/en-us/office365/securitycompliance/what-the-sensitive-information-types-look-for#us-social-security-number-ssn)</span><span class="sxs-lookup"><span data-stu-id="2969f-117">For more information on what is required for SSNs to be detected for your content, see the following section in this article: [What the Sensitive Information Types look for SSNs](https://docs.microsoft.com/en-us/office365/securitycompliance/what-the-sensitive-information-types-look-for#us-social-security-number-ssn)</span></span>
  
<span data-ttu-id="2969f-118">Използване на тип на различни вградени чувствителна информация, вижте следната статия за повече информация относно какво е необходимо за други типове: [Какво чувствителна информация типове търси](https://docs.microsoft.com/en-us/office365/securitycompliance/what-the-sensitive-information-types-look-for)</span><span class="sxs-lookup"><span data-stu-id="2969f-118">Using a different built-in sensitive information type, see the following article for information on what is required for other types: [What the Sensitive Information Types look for](https://docs.microsoft.com/en-us/office365/securitycompliance/what-the-sensitive-information-types-look-for)</span></span>
  

