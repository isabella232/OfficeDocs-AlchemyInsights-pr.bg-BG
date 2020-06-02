---
title: DLP правило за номер на банковата сметка в САЩ не работи
ms.author: deniseb
author: denisebmsft
manager: laurawi
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1287"
- "3200001"
ms.assetid: 80b40145-8376-4c3a-8d22-6efb9f9cb271
ms.openlocfilehash: b032a7c80e8b387114aeda95c4f6af7e57225517
ms.sourcegitcommit: bc7d6f4f3c9f7060d073f5130e1ec856e248d020
ms.translationtype: MT
ms.contentlocale: bg-BG
ms.lasthandoff: 06/02/2020
ms.locfileid: "44507323"
---
# <a name="dlp-issues-with-us-bank-account-numbers"></a><span data-ttu-id="9cfd0-102">Проблеми с DLP с номера на банкови сметки в САЩ</span><span class="sxs-lookup"><span data-stu-id="9cfd0-102">DLP issues with US bank account numbers</span></span>

<span data-ttu-id="9cfd0-103">**Важно**: през тези безпрецедентни времена ние предприемаме стъпки, за да гарантираме, че услугите на SharePoint Online и OneDrive остават на пълно разположение – за повече информация посетете [Временни корекции на функции на SharePoint Online](https://aka.ms/ODSPAdjustments).</span><span class="sxs-lookup"><span data-stu-id="9cfd0-103">**Important**: During these unprecedented times, we are taking steps to ensure that SharePoint Online and OneDrive services remain highly available – Please visit [SharePoint Online Temporary Feature Adjustments](https://aka.ms/ODSPAdjustments) for more information.</span></span>

<span data-ttu-id="9cfd0-104">**Проблеми с DLP с номера на банкови сметки в САЩ**</span><span class="sxs-lookup"><span data-stu-id="9cfd0-104">**DLP issues with US bank account numbers**</span></span>

<span data-ttu-id="9cfd0-105">Имате проблеми с **предотвратяването на загуба на данни (DLP),** което не работи за съдържание, съдържащо номер на банкова сметка в **САЩ,** когато използвате DLP чувствителен тип информация в O365?</span><span class="sxs-lookup"><span data-stu-id="9cfd0-105">Are you having problems with **Data Loss Prevention (DLP)** not working for content containing a **US Bank Account Number** when using a DLP sensitive information type in O365?</span></span> <span data-ttu-id="9cfd0-106">Ако е така, уверете се, че съдържанието съдържа необходимата информация за това, което DLP се търси, когато се оценява.</span><span class="sxs-lookup"><span data-stu-id="9cfd0-106">If so, make sure your content contains the needed information for what the DLP policy is looking for when it is evaluated.</span></span>
  
<span data-ttu-id="9cfd0-107">Например за **сащ банка номер** правила конфигуриран с ниво на доверие 85%, се оценяват по-долу и трябва да бъдат открити за правилото да задейства:</span><span class="sxs-lookup"><span data-stu-id="9cfd0-107">For example, for a **US Bank Account Number** policy configured with a confidence level of 85%, the following are evaluated and must be detected for the rule to trigger:</span></span>
  
- <span data-ttu-id="9cfd0-108">**[Формат:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#format-77)** 8-17 цифри</span><span class="sxs-lookup"><span data-stu-id="9cfd0-108">**[Format:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#format-77)** 8-17 digits</span></span>

- <span data-ttu-id="9cfd0-109">**[Модел:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#pattern-77)** 8-17 последователни цифри.</span><span class="sxs-lookup"><span data-stu-id="9cfd0-109">**[Pattern:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#pattern-77)** 8-17 consecutive digits.</span></span>

- <span data-ttu-id="9cfd0-110">**[Контролна сума:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#checksum-76)** Не, няма контролна сума</span><span class="sxs-lookup"><span data-stu-id="9cfd0-110">**[Checksum:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#checksum-76)** No, there is no Checksum</span></span>

- <span data-ttu-id="9cfd0-111">**[Определение:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions)** Правилата на DLP са 75% уверени, че е открита тази информация, ако в близост до 300 знака:</span><span class="sxs-lookup"><span data-stu-id="9cfd0-111">**[Definition:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions)** A DLP policy is 75% confident that it's detected this type of sensitive information if, within a proximity of 300 characters:</span></span>

  - <span data-ttu-id="9cfd0-112">Регулярният израз Regex_usa_bank_account_number намира съдържание, което съответства на модела</span><span class="sxs-lookup"><span data-stu-id="9cfd0-112">The regular expression Regex_usa_bank_account_number finds content that matches the pattern</span></span>

  - <span data-ttu-id="9cfd0-113">Намерена е ключова дума от Keyword_usa_Bank_Account.</span><span class="sxs-lookup"><span data-stu-id="9cfd0-113">A keyword from Keyword_usa_Bank_Account is found.</span></span>

    <span data-ttu-id="9cfd0-114">Например следната извадка ще задейства за правилата за **номер на банкови сметки в САЩ:** Проверка на сметка 78344011</span><span class="sxs-lookup"><span data-stu-id="9cfd0-114">For example, the following sample would trigger for the **US Bank Account Number** policy: Checking Account 78344011</span></span>

<span data-ttu-id="9cfd0-115">За повече информация относно това, което е необходимо за да бъде открит **номер на банковата сметка** в САЩ за вашето съдържание вижте следния раздел в тази статия: Какво чувствителна информация видове изглежда за номер на [банковата сметка в САЩ](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#us-bank-account-number)</span><span class="sxs-lookup"><span data-stu-id="9cfd0-115">For more information on what is required for a **US Bank Account Number** to be detected for your content, see the following section in this article: [What the Sensitive Information Types look for US Bank Account Number](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#us-bank-account-number)</span></span>
  
<span data-ttu-id="9cfd0-116">С помощта на друг вграден тип поверителна информация вижте следната статия за информация за това какво е необходимо за други типове: [Какво се търси типовете информация за чувствителната информация](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions)</span><span class="sxs-lookup"><span data-stu-id="9cfd0-116">Using a different built-in sensitive information type, see the following article for information on what is required for other types: [What the Sensitive Information Types look for](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions)</span></span>
  