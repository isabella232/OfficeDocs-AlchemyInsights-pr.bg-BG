---
title: DLP правило за SSN не работи
ms.author: deniseb
author: denisebmsft
manager: laurawi
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1242"
- "3200001"
ms.assetid: ac265ee6-c946-476e-9bf0-0ea0e8adc98a
ms.openlocfilehash: 35859bce89ef1ae9b6a9e706fc316b0ee6cd27d1
ms.sourcegitcommit: bc7d6f4f3c9f7060d073f5130e1ec856e248d020
ms.translationtype: MT
ms.contentlocale: bg-BG
ms.lasthandoff: 06/02/2020
ms.locfileid: "44507359"
---
# <a name="dlp-issues-with-social-security-numbers"></a><span data-ttu-id="aeba7-102">Проблеми с DLP с номера на социална осигуровка</span><span class="sxs-lookup"><span data-stu-id="aeba7-102">DLP issues with Social Security Numbers</span></span>

<span data-ttu-id="aeba7-103">**Важно**: през тези безпрецедентни времена ние предприемаме стъпки, за да гарантираме, че услугите на SharePoint Online и OneDrive остават на пълно разположение – за повече информация посетете [Временни корекции на функции на SharePoint Online](https://aka.ms/ODSPAdjustments).</span><span class="sxs-lookup"><span data-stu-id="aeba7-103">**Important**: During these unprecedented times, we are taking steps to ensure that SharePoint Online and OneDrive services remain highly available – Please visit [SharePoint Online Temporary Feature Adjustments](https://aka.ms/ODSPAdjustments) for more information.</span></span>

<span data-ttu-id="aeba7-104">**Проблеми с DLP с SSN**</span><span class="sxs-lookup"><span data-stu-id="aeba7-104">**DLP issues with SSNs**</span></span>

<span data-ttu-id="aeba7-105">Имате проблеми с **предотвратяване на загуба на данни (DLP)** не работи за съдържание, съдържащо **социално-осигурителен номер (SSN),** когато използвате чувствителен тип информация в Microsoft 365?</span><span class="sxs-lookup"><span data-stu-id="aeba7-105">Are you having problems with **Data Loss Prevention (DLP)** not working for content containing a **Social Security Number (SSN)** when using a sensitive information type in Microsoft 365?</span></span> <span data-ttu-id="aeba7-106">Ако е така, уверете се, че съдържанието съдържа необходимата информация за това, което се търси от правилата на DLP.</span><span class="sxs-lookup"><span data-stu-id="aeba7-106">If so, make sure your content contains the needed information for what the DLP policy is looking.</span></span> 
  
<span data-ttu-id="aeba7-107">Например за SSN правила конфигурирани с ниво на доверие 85%, се оценяват следното и трябва да бъдат открити за правило за задействане:</span><span class="sxs-lookup"><span data-stu-id="aeba7-107">For example, for an SSN policy configured with a confidence level of 85%, the following are evaluated and must be detected for the rule to trigger:</span></span>
  
- <span data-ttu-id="aeba7-108">**[Формат:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#format-80)** 9 цифри, които могат да бъдат във формат или неформатиран модел</span><span class="sxs-lookup"><span data-stu-id="aeba7-108">**[Format:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#format-80)** 9 digits, which may be in a formatted or unformatted pattern</span></span>

- <span data-ttu-id="aeba7-109">**[Модел:](https://msconnect.microsoft.com/https:/docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#pattern-80)** Четири функции търсят SSN в четири различни модела:</span><span class="sxs-lookup"><span data-stu-id="aeba7-109">**[Pattern:](https://msconnect.microsoft.com/https:/docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#pattern-80)** Four functions look for SSNs in four different patterns:</span></span>

  - <span data-ttu-id="aeba7-110">Func_ssn намира SSNs с форматиране преди 2011 г., които са форматирани с тирета или интервали (ddd-dddd ИЛИ DDD ddd dddd)</span><span class="sxs-lookup"><span data-stu-id="aeba7-110">Func_ssn finds SSNs with pre-2011 strong formatting that are formatted with dashes or spaces (ddd-dd-dddd OR ddd dd dddd)</span></span>

  - <span data-ttu-id="aeba7-111">Func_unformatted_ssn намира SSN с форматиране преди 2011 г., които не са форматирани като девет последователни цифри (ddddddddddddddd)</span><span class="sxs-lookup"><span data-stu-id="aeba7-111">Func_unformatted_ssn finds SSNs with pre-2011 strong formatting that are unformatted as nine consecutive digits (ddddddddd)</span></span>

  - <span data-ttu-id="aeba7-112">Func_randomized_formatted_ssn намира след 2011 SSNs, които са форматирани с тирета или интервали (ddd-dddd ИЛИ DDD DDD)</span><span class="sxs-lookup"><span data-stu-id="aeba7-112">Func_randomized_formatted_ssn finds post-2011 SSNs that are formatted with dashes or spaces (ddd-dd-dddd OR ddd dd dddd)</span></span>

  - <span data-ttu-id="aeba7-113">Func_randomized_unformatted_ssn намира след 2011 SSNs, които са неформатирани като девет последователни цифри (ddddddddddddddddd</span><span class="sxs-lookup"><span data-stu-id="aeba7-113">Func_randomized_unformatted_ssn finds post-2011 SSNs that are unformatted as nine consecutive digits (ddddddddd)</span></span>

- <span data-ttu-id="aeba7-114">**[Контролна сума:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#checksum-79)** Не, няма контролна сума</span><span class="sxs-lookup"><span data-stu-id="aeba7-114">**[Checksum:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#checksum-79)** No, there is no Checksum</span></span>

- <span data-ttu-id="aeba7-115">**[Определение:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#definition-80)** DLP политика е 85% уверени, че е открита този тип чувствителна информация, ако в близост до 300 знака:</span><span class="sxs-lookup"><span data-stu-id="aeba7-115">**[Definition:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#definition-80)** A DLP policy is 85% confident that it's detected this type of sensitive information if, within a proximity of 300 characters:</span></span>

  - <span data-ttu-id="aeba7-116">[Функцията Func_ssn](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#pattern-80) намира съдържание, което съответства на модела.</span><span class="sxs-lookup"><span data-stu-id="aeba7-116">The [function Func_ssn](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#pattern-80) finds content that matches the pattern.</span></span>

  - <span data-ttu-id="aeba7-117">Намерена е ключова дума от [Keyword_ssn.](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#keyword_ssn)</span><span class="sxs-lookup"><span data-stu-id="aeba7-117">A keyword from [Keyword_ssn](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#keyword_ssn) is found.</span></span> <span data-ttu-id="aeba7-118">Примерите за ключови думи включват: *Социална сигурност, Социална сигурност# Soc Sec, SSN.*</span><span class="sxs-lookup"><span data-stu-id="aeba7-118">Examples of keywords includes:  *Social Security, Social Security#, Soc Sec ,SSN*  .</span></span> <span data-ttu-id="aeba7-119">Например следната проба ще задейства DLP SSN политика: **SSN: 489-36-8350**</span><span class="sxs-lookup"><span data-stu-id="aeba7-119">For example, the following sample would trigger for the DLP SSN policy: **SSN: 489-36-8350**</span></span>
  
<span data-ttu-id="aeba7-120">За повече информация относно това, което е необходимо за SSN да бъдат открити за вашето съдържание вижте следния раздел в тази статия: [Какви типове информация за чувствителна изглежда за SSN](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#us-social-security-number-ssn)</span><span class="sxs-lookup"><span data-stu-id="aeba7-120">For more information on what is required for SSNs to be detected for your content, see the following section in this article: [What the Sensitive Information Types look for SSNs](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#us-social-security-number-ssn)</span></span>
  
<span data-ttu-id="aeba7-121">С помощта на друг вграден тип поверителна информация вижте следната статия за информация за това какво е необходимо за други типове: [Какво се търси типовете информация за чувствителната информация](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions)</span><span class="sxs-lookup"><span data-stu-id="aeba7-121">Using a different built-in sensitive information type, see the following article for information on what is required for other types: [What the Sensitive Information Types look for](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions)</span></span>
  