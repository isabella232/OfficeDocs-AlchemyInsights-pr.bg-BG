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
ms.openlocfilehash: 4ec0df9d4954a8c65f0c34188d285dd8cf44a4f2
ms.sourcegitcommit: d108a2da2f5dab05246e30b5108cca5173e09051
ms.translationtype: MT
ms.contentlocale: bg-BG
ms.lasthandoff: 03/26/2020
ms.locfileid: "42977295"
---
# <a name="dlp-issues-with-social-security-numbers"></a><span data-ttu-id="49014-102">DLP проблеми с номера на социална сигурност</span><span class="sxs-lookup"><span data-stu-id="49014-102">DLP issues with Social Security Numbers</span></span>

<span data-ttu-id="49014-103">**Важно**: По време на тези безпрецедентни времена, ние предприемаме стъпки, за да се гарантира, че SharePoint Online и OneDrive услуги остават високо достъпни – посетете [SharePoint Online временни функция корекции](https://aka.ms/ODSPAdjustments) за повече информация.</span><span class="sxs-lookup"><span data-stu-id="49014-103">**Important**: During these unprecedented times, we are taking steps to ensure that SharePoint Online and OneDrive services remain highly available – Please visit [SharePoint Online Temporary Feature Adjustments](https://aka.ms/ODSPAdjustments) for more information.</span></span>

<span data-ttu-id="49014-104">**Проблеми с dlp с SSN**</span><span class="sxs-lookup"><span data-stu-id="49014-104">**DLP issues with SSNs**</span></span>

<span data-ttu-id="49014-105">Имате проблеми с **предотвратяване на загуба на данни (DLP)** не работи за съдържание, съдържащо номер за социална сигурност **(SSN),** когато използвате поверителна информация тип в Office 365?</span><span class="sxs-lookup"><span data-stu-id="49014-105">Are you having problems with **Data Loss Prevention (DLP)** not working for content containing a **Social Security Number (SSN)** when using a sensitive information type in Office 365?</span></span> <span data-ttu-id="49014-106">Ако е така, уверете се, че съдържанието ви съдържа необходимата информация за това, което се търси dlp правилата.</span><span class="sxs-lookup"><span data-stu-id="49014-106">If so, make sure your content contains the needed information for what the DLP policy is looking.</span></span> 
  
<span data-ttu-id="49014-107">Например за SSN правила, конфигурирани с ниво на сигурност 85 %, се оценяват следното и трябва да бъдат открити за правилото за задействане:</span><span class="sxs-lookup"><span data-stu-id="49014-107">For example, for an SSN policy configured with a confidence level of 85%, the following are evaluated and must be detected for the rule to trigger:</span></span>
  
- <span data-ttu-id="49014-108">**[Формат:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#format-80)** 9 цифри, които може да са във формат или неформатиран модел</span><span class="sxs-lookup"><span data-stu-id="49014-108">**[Format:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#format-80)** 9 digits, which may be in a formatted or unformatted pattern</span></span>

- <span data-ttu-id="49014-109">**[Модел:](https://msconnect.microsoft.com/https:/docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#pattern-80)** Четири функции търсят SSN в четири различни модела:</span><span class="sxs-lookup"><span data-stu-id="49014-109">**[Pattern:](https://msconnect.microsoft.com/https:/docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#pattern-80)** Four functions look for SSNs in four different patterns:</span></span>

  - <span data-ttu-id="49014-110">Func_ssn намира SSN със силно форматиране преди 2011 г., форматирани с тирета или интервали (ddd-dddddd ddddd ddddd ddddd dddddddddddddddddddddddddddddddddddddddd)</span><span class="sxs-lookup"><span data-stu-id="49014-110">Func_ssn finds SSNs with pre-2011 strong formatting that are formatted with dashes or spaces (ddd-dd-dddd OR ddd dd dddd)</span></span>

  - <span data-ttu-id="49014-111">Func_unformatted_ssn открива SSN с предварително 2011 силно форматиране, които са неформатирани като девет последователни цифри (ddddddddddddddddddddddddddddddddddddddddddddddddddd</span><span class="sxs-lookup"><span data-stu-id="49014-111">Func_unformatted_ssn finds SSNs with pre-2011 strong formatting that are unformatted as nine consecutive digits (ddddddddd)</span></span>

  - <span data-ttu-id="49014-112">Func_randomized_formatted_ssn намира след 2011 SSN, които са форматирани с тирета или интервали (ddd-dddddd или ddd ddd dddd dddd dddddd)</span><span class="sxs-lookup"><span data-stu-id="49014-112">Func_randomized_formatted_ssn finds post-2011 SSNs that are formatted with dashes or spaces (ddd-dd-dddd OR ddd dd dddd)</span></span>

  - <span data-ttu-id="49014-113">Func_randomized_unformatted_ssn намира след 2011 SSN, които са неформатирани като девет последователни цифри (ddddddddddd)</span><span class="sxs-lookup"><span data-stu-id="49014-113">Func_randomized_unformatted_ssn finds post-2011 SSNs that are unformatted as nine consecutive digits (ddddddddd)</span></span>

- <span data-ttu-id="49014-114">**[Контролна сума:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#checksum-79)** Не, няма чексума</span><span class="sxs-lookup"><span data-stu-id="49014-114">**[Checksum:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#checksum-79)** No, there is no Checksum</span></span>

- <span data-ttu-id="49014-115">**[Определение:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#definition-80)** DLP политика е 85% уверен, че е открит този тип чувствителна информация, ако в близост до 300 знака:</span><span class="sxs-lookup"><span data-stu-id="49014-115">**[Definition:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#definition-80)** A DLP policy is 85% confident that it's detected this type of sensitive information if, within a proximity of 300 characters:</span></span>

  - <span data-ttu-id="49014-116">[Функцията Func_ssn](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#pattern-80) намира съдържание, което съответства на шаблона.</span><span class="sxs-lookup"><span data-stu-id="49014-116">The [function Func_ssn](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#pattern-80) finds content that matches the pattern.</span></span>

  - <span data-ttu-id="49014-117">Намира се ключова дума от [Keyword_ssn.](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#keyword_ssn)</span><span class="sxs-lookup"><span data-stu-id="49014-117">A keyword from [Keyword_ssn](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#keyword_ssn) is found.</span></span> <span data-ttu-id="49014-118">Сред ключовите думи са: *Социална сигурност, Социална осигуровка#, Soc Sec, SSN.*</span><span class="sxs-lookup"><span data-stu-id="49014-118">Examples of keywords includes:  *Social Security, Social Security#, Soc Sec ,SSN*  .</span></span> <span data-ttu-id="49014-119">Например следната извадка ще предизвика за DLP SSN **политика: SSN: 489-36-8350**</span><span class="sxs-lookup"><span data-stu-id="49014-119">For example, the following sample would trigger for the DLP SSN policy: **SSN: 489-36-8350**</span></span>
  
<span data-ttu-id="49014-120">За повече информация за това какво се изисква за SSN да бъдат открити за вашето съдържание вижте следния раздел в тази статия: [Какви типове поверителна информация търси SSN](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#us-social-security-number-ssn)</span><span class="sxs-lookup"><span data-stu-id="49014-120">For more information on what is required for SSNs to be detected for your content, see the following section in this article: [What the Sensitive Information Types look for SSNs](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#us-social-security-number-ssn)</span></span>
  
<span data-ttu-id="49014-121">Използвайки друг вграден тип поверителна информация, вижте следната статия за информация за това какво се изисква за други типове: [Какво търсят типовете поверителна информация за](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for)</span><span class="sxs-lookup"><span data-stu-id="49014-121">Using a different built-in sensitive information type, see the following article for information on what is required for other types: [What the Sensitive Information Types look for](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for)</span></span>
  