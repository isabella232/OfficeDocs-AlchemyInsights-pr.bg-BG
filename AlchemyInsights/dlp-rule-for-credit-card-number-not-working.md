---
title: DLP правило за номер на кредитна карта не работи
ms.author: cmcatee
author: cmcatee-MSFT
manager: mnirkhe
ms.date: 11/5/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.assetid: 30496c79-c8b4-4337-a46d-abed12864209
ms.openlocfilehash: a56f32b54e6cb32fa044d26d08868bac8c368de5
ms.sourcegitcommit: e2864efcfb493b6e46b662b746661a61232bdba7
ms.translationtype: MT
ms.contentlocale: bg-BG
ms.lasthandoff: 01/24/2019
ms.locfileid: "29458761"
---
<span data-ttu-id="61439-p101">Имате ли проблеми с **Данни загуба предотвратяване (DLP)** не работи за съдържание, съдържаща **Номер на кредитна карта** , когато използвате тип DLP чувствителна информация в O365? Ако е така, се уверете, че вашето съдържание съдържа необходимата информация за задействане на DLP политика, когато той се оценява. Например за **кредитната ви карта** конфигуриран с ниво на доверие от 85 %, следното се оценяват и трябва да бъде открит за да задейства правилото:</span><span class="sxs-lookup"><span data-stu-id="61439-p101">Are you having problems with **Data Loss Prevention (DLP)** not working for content containing a **Credit Card Number** when using a DLP sensitive information type in O365? If so, make sure your content contains the needed information to trigger the the DLP policy when it is evaluated. For example, for a **Credit Card policy** configured with a confidence level of 85%, the following are evaluated and must be detected for the rule to trigger:</span></span> 
  
- <span data-ttu-id="61439-105">**[Формат:](https://docs.microsoft.com/en-us/office365/securitycompliance/what-the-sensitive-information-types-look-for#format-19)** 16 цифри, което може да бъде форматиран или неформатиран (dddddddddddddddd) и трябва да мине на Luhn теста.</span><span class="sxs-lookup"><span data-stu-id="61439-105">**[Format:](https://docs.microsoft.com/en-us/office365/securitycompliance/what-the-sensitive-information-types-look-for#format-19)** 16 digits which can be formatted or unformatted (dddddddddddddddd) and must pass the Luhn test.</span></span> 
    
- <span data-ttu-id="61439-106">**[Модел:](https://docs.microsoft.com/en-us/office365/securitycompliance/what-the-sensitive-information-types-look-for#pattern-19)** Много сложни и стабилна шарка, която открива карти от всички основни марки по целия свят, включително Visa, Mastercard, Открийте карта, JCB, American Express, подарък и вечеря карти.</span><span class="sxs-lookup"><span data-stu-id="61439-106">**[Pattern:](https://docs.microsoft.com/en-us/office365/securitycompliance/what-the-sensitive-information-types-look-for#pattern-19)** Very complex and robust pattern that detects cards from all major brands worldwide, including Visa, MasterCard, Discover Card, JCB, American Express, gift cards, and diner cards.</span></span> 
    
- <span data-ttu-id="61439-107">**[Контролна сума:](https://docs.microsoft.com/en-us/office365/securitycompliance/what-the-sensitive-information-types-look-for#checksum-19)** Да, на Luhn шах</span><span class="sxs-lookup"><span data-stu-id="61439-107">**[Checksum:](https://docs.microsoft.com/en-us/office365/securitycompliance/what-the-sensitive-information-types-look-for#checksum-19)** Yes, the Luhn checksum</span></span> 
    
- <span data-ttu-id="61439-108">**[Дефиниция:](https://docs.microsoft.com/en-us/office365/securitycompliance/what-the-sensitive-information-types-look-for#definition-19)** DLP политика е 85 % уверени, че е открил този вид чувствителна информация ако, в рамките на близост на 300 знака:</span><span class="sxs-lookup"><span data-stu-id="61439-108">**[Definition:](https://docs.microsoft.com/en-us/office365/securitycompliance/what-the-sensitive-information-types-look-for#definition-19)** A DLP policy is 85% confident that it's detected this type of sensitive information if, within a proximity of 300 characters:</span></span> 
    
  - <span data-ttu-id="61439-109">Функцията Func_credit_card открие съдържание, което съвпада с модела.</span><span class="sxs-lookup"><span data-stu-id="61439-109">The function Func_credit_card finds content that matches the pattern.</span></span>
    
  - <span data-ttu-id="61439-110">Един от следните е вярно:</span><span class="sxs-lookup"><span data-stu-id="61439-110">One of the following is true:</span></span> 
    
  - <span data-ttu-id="61439-111">Ключова дума от Keyword_cc_verification е намерен.</span><span class="sxs-lookup"><span data-stu-id="61439-111">A keyword from Keyword_cc_verification is found.</span></span>
    
  - <span data-ttu-id="61439-112">Ключова дума от Keyword_cc_name се намира</span><span class="sxs-lookup"><span data-stu-id="61439-112">A keyword from Keyword_cc_name is found</span></span>
    
  - <span data-ttu-id="61439-113">Функцията Func_expiration_date намира дата във формат на правилната дата.</span><span class="sxs-lookup"><span data-stu-id="61439-113">The function Func_expiration_date finds a date in the right date format.</span></span>
    
  - <span data-ttu-id="61439-114">Контролна преминава</span><span class="sxs-lookup"><span data-stu-id="61439-114">The checksum passes</span></span>
    
    <span data-ttu-id="61439-115">Например следните примерни ще предизвика DLP кредитна карта номер политика за:</span><span class="sxs-lookup"><span data-stu-id="61439-115">For example, the following sample would trigger for a DLP Credit Card Number Policy:</span></span>
    
  - <span data-ttu-id="61439-116">Виза: 4485 3647 3952 7352</span><span class="sxs-lookup"><span data-stu-id="61439-116">Visa: 4485 3647 3952 7352</span></span> 
    
  - <span data-ttu-id="61439-117">Изтича: 2/2009</span><span class="sxs-lookup"><span data-stu-id="61439-117">Expires: 2/2009</span></span>
    
<span data-ttu-id="61439-118">За повече информация относно това, което се изисква за **Номер на кредитна карта** , за да бъдат открити за вашето съдържание, вижте следващия раздел в тази статия: [Какво чувствителна информация типове търси кредитна карта #](https://docs.microsoft.com/en-us/office365/securitycompliance/what-the-sensitive-information-types-look-for#credit-card-number)</span><span class="sxs-lookup"><span data-stu-id="61439-118">For more information on what is required for a **Credit Card Number** to be detected for your content, see the following section in this article: [What the Sensitive Information Types look for Credit Card#](https://docs.microsoft.com/en-us/office365/securitycompliance/what-the-sensitive-information-types-look-for#credit-card-number)</span></span>
  
<span data-ttu-id="61439-119">Използване на тип на различни вградени чувствителна информация, вижте следната статия за повече информация относно какво е необходимо за други типове: [Какво чувствителна информация типове търси](https://docs.microsoft.com/en-us/office365/securitycompliance/what-the-sensitive-information-types-look-for)</span><span class="sxs-lookup"><span data-stu-id="61439-119">Using a different built-in sensitive information type, see the following article for information on what is required for other types: [What the Sensitive Information Types look for](https://docs.microsoft.com/en-us/office365/securitycompliance/what-the-sensitive-information-types-look-for)</span></span>
  

