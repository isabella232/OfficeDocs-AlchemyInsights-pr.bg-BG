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
ms.openlocfilehash: 0b83a858975ffe1bb70f16a7452a13d57dff5340
ms.sourcegitcommit: b0d5b68366028abcf08610672d5bc9d3b25ac433
ms.translationtype: MT
ms.contentlocale: bg-BG
ms.lasthandoff: 03/24/2020
ms.locfileid: "42932510"
---
# <a name="dlp-issues-with-social-security-numbers"></a><span data-ttu-id="4ddd6-102">DLP проблеми с номера на социална сигурност</span><span class="sxs-lookup"><span data-stu-id="4ddd6-102">DLP issues with Social Security Numbers</span></span>

<span data-ttu-id="4ddd6-103">**Важно:** много sharePoint Online и OneDrive клиенти работят критични бизнес приложения срещу услугата, която се изпълнява във фонов режим.</span><span class="sxs-lookup"><span data-stu-id="4ddd6-103">**Important**: Many SharePoint Online and OneDrive customers run business-critical applications against the service that run in the background.</span></span> <span data-ttu-id="4ddd6-104">Те включват миграция на съдържанието, предотвратяване на загуба на данни (DLP) и архивиране на решения.</span><span class="sxs-lookup"><span data-stu-id="4ddd6-104">These include content migration, Data Loss Prevention (DLP), and backup solutions.</span></span> <span data-ttu-id="4ddd6-105">По време на тези безпрецедентни времена ние предприемаме стъпки, за да гарантираме, че SharePoint Online и OneDrive услуги остават високо достъпни и надеждни за вашите потребители, които зависят от услугата повече от всякога в отдалечени работни сценарии.</span><span class="sxs-lookup"><span data-stu-id="4ddd6-105">During these unprecedented times, we are taking steps to ensure that SharePoint Online and OneDrive services remain highly available and reliable for your users who depend on the service more than ever in remote work scenarios.</span></span>

<span data-ttu-id="4ddd6-106">В подкрепа на тази цел, ние сме внедрили по-строги ограничения за ограничаване на приложенията за фон (миграция, DLP и архивиране на решения) през делничните дни.</span><span class="sxs-lookup"><span data-stu-id="4ddd6-106">In support of this objective, we have implemented tighter throttling limits on background apps (migration, DLP and backup solutions) during weekday daytime hours.</span></span> <span data-ttu-id="4ddd6-107">Трябва да очаквате, че тези приложения ще постигнат много ограничена пропускателна информация по време на тези времена.</span><span class="sxs-lookup"><span data-stu-id="4ddd6-107">You should expect that these apps will achieve very limited throughput during these times.</span></span> <span data-ttu-id="4ddd6-108">Въпреки това, по време на вечерните и почивните часове за региона, услугата ще бъде готова да обработи значително по-голям обем заявки от приложения за фон.</span><span class="sxs-lookup"><span data-stu-id="4ddd6-108">However, during evening and weekend hours for the region, the service will be ready to process a significantly higher volume of requests from background apps.</span></span>

<span data-ttu-id="4ddd6-109">**Проблеми с dlp с SSN**</span><span class="sxs-lookup"><span data-stu-id="4ddd6-109">**DLP issues with SSNs**</span></span>

<span data-ttu-id="4ddd6-110">Имате проблеми с **предотвратяване на загуба на данни (DLP)** не работи за съдържание, съдържащо номер за социална сигурност **(SSN),** когато използвате поверителна информация тип в Office 365?</span><span class="sxs-lookup"><span data-stu-id="4ddd6-110">Are you having problems with **Data Loss Prevention (DLP)** not working for content containing a **Social Security Number (SSN)** when using a sensitive information type in Office 365?</span></span> <span data-ttu-id="4ddd6-111">Ако е така, уверете се, че съдържанието ви съдържа необходимата информация за това, което се търси dlp правилата.</span><span class="sxs-lookup"><span data-stu-id="4ddd6-111">If so, make sure your content contains the needed information for what the DLP policy is looking.</span></span> 
  
<span data-ttu-id="4ddd6-112">Например за SSN правила, конфигурирани с ниво на сигурност 85 %, се оценяват следното и трябва да бъдат открити за правилото за задействане:</span><span class="sxs-lookup"><span data-stu-id="4ddd6-112">For example, for an SSN policy configured with a confidence level of 85%, the following are evaluated and must be detected for the rule to trigger:</span></span>
  
- <span data-ttu-id="4ddd6-113">**[Формат:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#format-80)** 9 цифри, които може да са във формат или неформатиран модел</span><span class="sxs-lookup"><span data-stu-id="4ddd6-113">**[Format:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#format-80)** 9 digits, which may be in a formatted or unformatted pattern</span></span>

- <span data-ttu-id="4ddd6-114">**[Модел:](https://msconnect.microsoft.com/https:/docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#pattern-80)** Четири функции търсят SSN в четири различни модела:</span><span class="sxs-lookup"><span data-stu-id="4ddd6-114">**[Pattern:](https://msconnect.microsoft.com/https:/docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#pattern-80)** Four functions look for SSNs in four different patterns:</span></span>

  - <span data-ttu-id="4ddd6-115">Func_ssn намира SSN със силно форматиране преди 2011 г., форматирани с тирета или интервали (ddd-dddddd ddddd ddddd ddddd dddddddddddddddddddddddddddddddddddddddd)</span><span class="sxs-lookup"><span data-stu-id="4ddd6-115">Func_ssn finds SSNs with pre-2011 strong formatting that are formatted with dashes or spaces (ddd-dd-dddd OR ddd dd dddd)</span></span>

  - <span data-ttu-id="4ddd6-116">Func_unformatted_ssn открива SSN с предварително 2011 силно форматиране, които са неформатирани като девет последователни цифри (ddddddddddddddddddddddddddddddddddddddddddddddddddd</span><span class="sxs-lookup"><span data-stu-id="4ddd6-116">Func_unformatted_ssn finds SSNs with pre-2011 strong formatting that are unformatted as nine consecutive digits (ddddddddd)</span></span>

  - <span data-ttu-id="4ddd6-117">Func_randomized_formatted_ssn намира след 2011 SSN, които са форматирани с тирета или интервали (ddd-dddddd или ddd ddd dddd dddd dddddd)</span><span class="sxs-lookup"><span data-stu-id="4ddd6-117">Func_randomized_formatted_ssn finds post-2011 SSNs that are formatted with dashes or spaces (ddd-dd-dddd OR ddd dd dddd)</span></span>

  - <span data-ttu-id="4ddd6-118">Func_randomized_unformatted_ssn намира след 2011 SSN, които са неформатирани като девет последователни цифри (ddddddddddd)</span><span class="sxs-lookup"><span data-stu-id="4ddd6-118">Func_randomized_unformatted_ssn finds post-2011 SSNs that are unformatted as nine consecutive digits (ddddddddd)</span></span>

- <span data-ttu-id="4ddd6-119">**[Контролна сума:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#checksum-79)** Не, няма чексума</span><span class="sxs-lookup"><span data-stu-id="4ddd6-119">**[Checksum:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#checksum-79)** No, there is no Checksum</span></span>

- <span data-ttu-id="4ddd6-120">**[Определение:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#definition-80)** DLP политика е 85% уверен, че е открит този тип чувствителна информация, ако в близост до 300 знака:</span><span class="sxs-lookup"><span data-stu-id="4ddd6-120">**[Definition:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#definition-80)** A DLP policy is 85% confident that it's detected this type of sensitive information if, within a proximity of 300 characters:</span></span>

  - <span data-ttu-id="4ddd6-121">[Функцията Func_ssn](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#pattern-80) намира съдържание, което съответства на шаблона.</span><span class="sxs-lookup"><span data-stu-id="4ddd6-121">The [function Func_ssn](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#pattern-80) finds content that matches the pattern.</span></span>

  - <span data-ttu-id="4ddd6-122">Намира се ключова дума от [Keyword_ssn.](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#keyword_ssn)</span><span class="sxs-lookup"><span data-stu-id="4ddd6-122">A keyword from [Keyword_ssn](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#keyword_ssn) is found.</span></span> <span data-ttu-id="4ddd6-123">Сред ключовите думи са: *Социална сигурност, Социална осигуровка#, Soc Sec, SSN.*</span><span class="sxs-lookup"><span data-stu-id="4ddd6-123">Examples of keywords includes:  *Social Security, Social Security#, Soc Sec ,SSN*  .</span></span> <span data-ttu-id="4ddd6-124">Например следната извадка ще предизвика за DLP SSN **политика: SSN: 489-36-8350**</span><span class="sxs-lookup"><span data-stu-id="4ddd6-124">For example, the following sample would trigger for the DLP SSN policy: **SSN: 489-36-8350**</span></span>
  
<span data-ttu-id="4ddd6-125">За повече информация за това какво се изисква за SSN да бъдат открити за вашето съдържание вижте следния раздел в тази статия: [Какви типове поверителна информация търси SSN](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#us-social-security-number-ssn)</span><span class="sxs-lookup"><span data-stu-id="4ddd6-125">For more information on what is required for SSNs to be detected for your content, see the following section in this article: [What the Sensitive Information Types look for SSNs](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#us-social-security-number-ssn)</span></span>
  
<span data-ttu-id="4ddd6-126">Използвайки друг вграден тип поверителна информация, вижте следната статия за информация за това какво се изисква за други типове: [Какво търсят типовете поверителна информация за](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for)</span><span class="sxs-lookup"><span data-stu-id="4ddd6-126">Using a different built-in sensitive information type, see the following article for information on what is required for other types: [What the Sensitive Information Types look for](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for)</span></span>
  