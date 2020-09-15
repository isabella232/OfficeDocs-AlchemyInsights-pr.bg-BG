---
title: DLP правило за социална ОСИГУРОВКА не работи
ms.author: deniseb
author: denisebmsft
manager: laurawi
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1242"
- "3200001"
ms.assetid: ac265ee6-c946-476e-9bf0-0ea0e8adc98a
ms.openlocfilehash: b221e66862ca01074f380fbb8433f8f9cac044cb
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: bg-BG
ms.lasthandoff: 09/14/2020
ms.locfileid: "47679358"
---
# <a name="dlp-issues-with-social-security-numbers"></a><span data-ttu-id="af494-102">DLP проблеми със социални осигуровки</span><span class="sxs-lookup"><span data-stu-id="af494-102">DLP issues with Social Security Numbers</span></span>

<span data-ttu-id="af494-103">**Важно**: през тези безпрецедентни времена ние предприемаме стъпки, за да гарантираме, че услугите на SharePoint Online и OneDrive остават на пълно разположение – за повече информация посетете [Временни корекции на функции на SharePoint Online](https://aka.ms/ODSPAdjustments).</span><span class="sxs-lookup"><span data-stu-id="af494-103">**Important**: During these unprecedented times, we are taking steps to ensure that SharePoint Online and OneDrive services remain highly available – Please visit [SharePoint Online Temporary Feature Adjustments](https://aka.ms/ODSPAdjustments) for more information.</span></span>

<span data-ttu-id="af494-104">**DLP проблеми с SSNs**</span><span class="sxs-lookup"><span data-stu-id="af494-104">**DLP issues with SSNs**</span></span>

<span data-ttu-id="af494-105">Имате ли проблеми при **предотвратяване на загуба на данни (DLP)** , които не работят за съдържание, съдържащо **номер на социална осигуровка (социална осигуровка)** , когато използвате чувствителна информация в Microsoft 365?</span><span class="sxs-lookup"><span data-stu-id="af494-105">Are you having problems with **Data Loss Prevention (DLP)** not working for content containing a **Social Security Number (SSN)** when using a sensitive information type in Microsoft 365?</span></span> <span data-ttu-id="af494-106">Ако е така, трябва да се уверите, че вашето съдържание съдържа нужната информация за това, което търси DLP политиката.</span><span class="sxs-lookup"><span data-stu-id="af494-106">If so, make sure your content contains the needed information for what the DLP policy is looking.</span></span> 
  
<span data-ttu-id="af494-107">Например за правилата на социална ОСИГУРОВКА, конфигурирани с ниво на надеждност от 85%, следва да бъдат оценени следните неща и трябва да бъдат открити, за да се задейства правилото:</span><span class="sxs-lookup"><span data-stu-id="af494-107">For example, for an SSN policy configured with a confidence level of 85%, the following are evaluated and must be detected for the rule to trigger:</span></span>
  
- <span data-ttu-id="af494-108">**[Формат:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#format-80)** 9 цифри, които може да са в форматиран или неформатиран модел</span><span class="sxs-lookup"><span data-stu-id="af494-108">**[Format:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#format-80)** 9 digits, which may be in a formatted or unformatted pattern</span></span>

- <span data-ttu-id="af494-109">**[Шарка:](https://msconnect.microsoft.com/https:/docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#pattern-80)** Четирите функции търсят SSNs в четири различни модела:</span><span class="sxs-lookup"><span data-stu-id="af494-109">**[Pattern:](https://msconnect.microsoft.com/https:/docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#pattern-80)** Four functions look for SSNs in four different patterns:</span></span>

  - <span data-ttu-id="af494-110">Func_ssn намира SSNs с предварително 2011 силно форматиране, което се форматира с тирета или интервали (ДДД-дд-Асен или ДДД дд Асен)</span><span class="sxs-lookup"><span data-stu-id="af494-110">Func_ssn finds SSNs with pre-2011 strong formatting that are formatted with dashes or spaces (ddd-dd-dddd OR ddd dd dddd)</span></span>

  - <span data-ttu-id="af494-111">Func_unformatted_ssn намира SSNs с предварително 2011 силно форматиране, което е неформатирано като девет последователни цифри (ddddddddd)</span><span class="sxs-lookup"><span data-stu-id="af494-111">Func_unformatted_ssn finds SSNs with pre-2011 strong formatting that are unformatted as nine consecutive digits (ddddddddd)</span></span>

  - <span data-ttu-id="af494-112">Func_randomized_formatted_ssn намира Post-2011 SSNs, които са форматирани с тирета или интервали (ДДД-дд-Асен или ДДД дд Асен)</span><span class="sxs-lookup"><span data-stu-id="af494-112">Func_randomized_formatted_ssn finds post-2011 SSNs that are formatted with dashes or spaces (ddd-dd-dddd OR ddd dd dddd)</span></span>

  - <span data-ttu-id="af494-113">Func_randomized_unformatted_ssn намира Post-2011 SSNs, които са неформатирани като девет последователни цифри (ddddddddd)</span><span class="sxs-lookup"><span data-stu-id="af494-113">Func_randomized_unformatted_ssn finds post-2011 SSNs that are unformatted as nine consecutive digits (ddddddddd)</span></span>

- <span data-ttu-id="af494-114">**[Контролна сума:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#checksum-79)** Не, няма шах</span><span class="sxs-lookup"><span data-stu-id="af494-114">**[Checksum:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#checksum-79)** No, there is no Checksum</span></span>

- <span data-ttu-id="af494-115">**[Дефиниция:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#definition-80)** DLP правилата е 85% сигурни, че той е открил този тип поверителна информация, ако в близост до знаците на 300:</span><span class="sxs-lookup"><span data-stu-id="af494-115">**[Definition:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#definition-80)** A DLP policy is 85% confident that it's detected this type of sensitive information if, within a proximity of 300 characters:</span></span>

  - <span data-ttu-id="af494-116">[Функцията Func_ssn](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#pattern-80) намира съдържание, което съответства на шарката.</span><span class="sxs-lookup"><span data-stu-id="af494-116">The [function Func_ssn](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#pattern-80) finds content that matches the pattern.</span></span>

  - <span data-ttu-id="af494-117">Намерена е ключова дума от [Keyword_ssn](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#keyword_ssn) .</span><span class="sxs-lookup"><span data-stu-id="af494-117">A keyword from [Keyword_ssn](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#keyword_ssn) is found.</span></span> <span data-ttu-id="af494-118">Примерите за ключови думи включват:  *социално осигуряване, социално осигуряване #, SoC сек, социална осигуровка*  .</span><span class="sxs-lookup"><span data-stu-id="af494-118">Examples of keywords includes:  *Social Security, Social Security#, Soc Sec ,SSN*  .</span></span> <span data-ttu-id="af494-119">Например примерът по-долу би активирал правилата за DLP социална ОСИГУРОВКА: **социална осигуровка: 489-36-8350**</span><span class="sxs-lookup"><span data-stu-id="af494-119">For example, the following sample would trigger for the DLP SSN policy: **SSN: 489-36-8350**</span></span>
  
<span data-ttu-id="af494-120">За повече информация за това, което е необходимо, за да бъде открит SSNs за вашето съдържание, вижте раздела по-долу в тази статия: [какви типове чувствителна информация търси SSNs](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#us-social-security-number-ssn)</span><span class="sxs-lookup"><span data-stu-id="af494-120">For more information on what is required for SSNs to be detected for your content, see the following section in this article: [What the Sensitive Information Types look for SSNs](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#us-social-security-number-ssn)</span></span>
  
<span data-ttu-id="af494-121">С помощта на различен вграден тип чувствителна информация вижте статията по-долу за информация относно това, което е необходимо за други типове: [какви типове чувствителна информация търсите](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions)</span><span class="sxs-lookup"><span data-stu-id="af494-121">Using a different built-in sensitive information type, see the following article for information on what is required for other types: [What the Sensitive Information Types look for](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions)</span></span>
  