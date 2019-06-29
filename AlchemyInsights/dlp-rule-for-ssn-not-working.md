---
title: DLP правило за SSN не работи
ms.author: deniseb
author: denisebmsft
manager: laurawi
ms.date: 11/5/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1242"
- "3200001"
ms.assetid: ac265ee6-c946-476e-9bf0-0ea0e8adc98a
ms.openlocfilehash: fffd355279b064b31c0a8bf60518b15ee1ed1848
ms.sourcegitcommit: 5fb7a4b28859690020efdea630d03e70cc0e6334
ms.translationtype: MT
ms.contentlocale: bg-BG
ms.lasthandoff: 06/28/2019
ms.locfileid: "35389422"
---
# <a name="dlp-issues-with-social-security-numbers"></a><span data-ttu-id="f8e39-102">DLP проблеми с номера на социални осигуровки</span><span class="sxs-lookup"><span data-stu-id="f8e39-102">DLP issues with Social Security Numbers</span></span>

<span data-ttu-id="f8e39-103">Имате ли проблеми с **Данни загуба предотвратяване (DLP)** не работи за съдържание, съдържащи **Социално-осигурителен номер (SSN)** , когато използвате тип поверителна информация в Office 365?</span><span class="sxs-lookup"><span data-stu-id="f8e39-103">Are you having problems with **Data Loss Prevention (DLP)** not working for content containing a **Social Security Number (SSN)** when using a sensitive information type in Office 365?</span></span> <span data-ttu-id="f8e39-104">Ако е така, се уверете, че вашето съдържание съдържа необходимата информация за това, което политиката на DLP търси.</span><span class="sxs-lookup"><span data-stu-id="f8e39-104">If so, make sure your content contains the needed information for what the DLP policy is looking.</span></span> 
  
<span data-ttu-id="f8e39-105">Например за SSN политика, конфигуриран с ниво на доверие от 85 %, по-долу се оценяват и трябва да бъде открит за да задейства правилото:</span><span class="sxs-lookup"><span data-stu-id="f8e39-105">For example, for an SSN policy configured with a confidence level of 85%, the following are evaluated and must be detected for the rule to trigger:</span></span>
  
- <span data-ttu-id="f8e39-106">**[Формат:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#format-80)** 9 цифри, които могат да бъдат в форматиран или неформатиран модел</span><span class="sxs-lookup"><span data-stu-id="f8e39-106">**[Format:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#format-80)** 9 digits, which may be in a formatted or unformatted pattern</span></span>

- <span data-ttu-id="f8e39-107">**[Модел:](https://msconnect.microsoft.com/https:/docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#pattern-80)** Четири функции търсите SSNs в четири различни модели:</span><span class="sxs-lookup"><span data-stu-id="f8e39-107">**[Pattern:](https://msconnect.microsoft.com/https:/docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#pattern-80)** Four functions look for SSNs in four different patterns:</span></span>

  - <span data-ttu-id="f8e39-108">Func_ssn намира SSNs с предварително-2011 силно форматиране, които са форматирани с тирета или помещения (ddd дд Асен или ddd dd дддд)</span><span class="sxs-lookup"><span data-stu-id="f8e39-108">Func_ssn finds SSNs with pre-2011 strong formatting that are formatted with dashes or spaces (ddd-dd-dddd OR ddd dd dddd)</span></span>

  - <span data-ttu-id="f8e39-109">Func_unformatted_ssn намира SSNs с предварително-2011 силно форматиране, които са неформатирани като девет поредни цифри (ddddddddd)</span><span class="sxs-lookup"><span data-stu-id="f8e39-109">Func_unformatted_ssn finds SSNs with pre-2011 strong formatting that are unformatted as nine consecutive digits (ddddddddd)</span></span>

  - <span data-ttu-id="f8e39-110">Func_randomized_formatted_ssn намира пост-2011 SSNs, които са форматирани с тирета или помещения (ddd дд Асен или ddd dd дддд)</span><span class="sxs-lookup"><span data-stu-id="f8e39-110">Func_randomized_formatted_ssn finds post-2011 SSNs that are formatted with dashes or spaces (ddd-dd-dddd OR ddd dd dddd)</span></span>

  - <span data-ttu-id="f8e39-111">Func_randomized_unformatted_ssn намира пост-2011 SSNs, които са неформатирани като девет поредни цифри (ddddddddd)</span><span class="sxs-lookup"><span data-stu-id="f8e39-111">Func_randomized_unformatted_ssn finds post-2011 SSNs that are unformatted as nine consecutive digits (ddddddddd)</span></span>

- <span data-ttu-id="f8e39-112">**[Контролна сума:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#checksum-79)** Не, няма никакъв шах</span><span class="sxs-lookup"><span data-stu-id="f8e39-112">**[Checksum:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#checksum-79)** No, there is no Checksum</span></span>

- <span data-ttu-id="f8e39-113">**[Дефиниция:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#definition-80)** DLP политика е 85 % уверени, че е открил този вид чувствителна информация ако, в рамките на близост на 300 знака:</span><span class="sxs-lookup"><span data-stu-id="f8e39-113">**[Definition:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#definition-80)** A DLP policy is 85% confident that it's detected this type of sensitive information if, within a proximity of 300 characters:</span></span>

  - <span data-ttu-id="f8e39-114">[Функцията Func_ssn](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#pattern-80) намира съдържание, което съвпада с модела.</span><span class="sxs-lookup"><span data-stu-id="f8e39-114">The [function Func_ssn](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#pattern-80) finds content that matches the pattern.</span></span>

  - <span data-ttu-id="f8e39-115">Ключова дума от [Keyword_ssn](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#keyword_ssn) е намерен.</span><span class="sxs-lookup"><span data-stu-id="f8e39-115">A keyword from [Keyword_ssn](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#keyword_ssn) is found.</span></span> <span data-ttu-id="f8e39-116">Примери за ключови думи включва: *социалното осигуряване, социално осигуряване #, Soc Sec, SSN* .</span><span class="sxs-lookup"><span data-stu-id="f8e39-116">Examples of keywords includes:  *Social Security, Social Security#, Soc Sec ,SSN*  .</span></span> <span data-ttu-id="f8e39-117">Например, следните примерни ще предизвика на DLP SSN политика: **SSN: 489-36-8350**</span><span class="sxs-lookup"><span data-stu-id="f8e39-117">For example, the following sample would trigger for the DLP SSN policy: **SSN: 489-36-8350**</span></span>
  
<span data-ttu-id="f8e39-118">За повече информация относно това, което се изисква за SSNs да бъдат открити за вашето съдържание, вижте следващия раздел в тази статия: [Какво чувствителна информация типове търси SSNs](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#us-social-security-number-ssn)</span><span class="sxs-lookup"><span data-stu-id="f8e39-118">For more information on what is required for SSNs to be detected for your content, see the following section in this article: [What the Sensitive Information Types look for SSNs](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#us-social-security-number-ssn)</span></span>
  
<span data-ttu-id="f8e39-119">Използване на тип на различни вградени чувствителна информация, вижте следната статия за повече информация относно какво е необходимо за други типове: [Какво чувствителна информация типове търси](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for)</span><span class="sxs-lookup"><span data-stu-id="f8e39-119">Using a different built-in sensitive information type, see the following article for information on what is required for other types: [What the Sensitive Information Types look for](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for)</span></span>
  