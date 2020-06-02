---
title: DLP правило за US/UK паспорт номер не работи
ms.author: deniseb
author: denisebmsft
manager: laurawi
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1319"
- "3200001"
ms.assetid: fc178b8b-943b-4346-a2bd-a75c6af6f80f
ms.openlocfilehash: 3d3b7dc2d9510376bc9eef6ec69b87ad7c681b05
ms.sourcegitcommit: bc7d6f4f3c9f7060d073f5130e1ec856e248d020
ms.translationtype: MT
ms.contentlocale: bg-BG
ms.lasthandoff: 06/02/2020
ms.locfileid: "44507287"
---
# <a name="problems-with-dlp---usuk-passport-numbers"></a><span data-ttu-id="c6aff-102">Проблеми с DLP - US/UK паспортни номера</span><span class="sxs-lookup"><span data-stu-id="c6aff-102">Problems with DLP - US/UK passport numbers</span></span>

<span data-ttu-id="c6aff-103">**Важно**: през тези безпрецедентни времена ние предприемаме стъпки, за да гарантираме, че услугите на SharePoint Online и OneDrive остават на пълно разположение – за повече информация посетете [Временни корекции на функции на SharePoint Online](https://aka.ms/ODSPAdjustments).</span><span class="sxs-lookup"><span data-stu-id="c6aff-103">**Important**: During these unprecedented times, we are taking steps to ensure that SharePoint Online and OneDrive services remain highly available – Please visit [SharePoint Online Temporary Feature Adjustments](https://aka.ms/ODSPAdjustments) for more information.</span></span>

<span data-ttu-id="c6aff-104">**Проблеми с DLP с американски/британски паспортни номера**</span><span class="sxs-lookup"><span data-stu-id="c6aff-104">**DLP issues with US/UK passport numbers**</span></span>

<span data-ttu-id="c6aff-105">Имате проблеми с **предотвратяването на загуба на данни (DLP),** което не работи за съдържание, съдържащо номер на паспорт в **САЩ/Великобритания,** когато използвате тип чувствителна информация за DLP в O365?</span><span class="sxs-lookup"><span data-stu-id="c6aff-105">Are you having problems with **Data Loss Prevention (DLP)** not working for content containing a **US/UK passport number** when using a DLP sensitive information type in O365?</span></span> <span data-ttu-id="c6aff-106">Ако е така, уверете се, че съдържанието съдържа необходимата информация за това, което DLP се търси, когато се оценява.</span><span class="sxs-lookup"><span data-stu-id="c6aff-106">If so, make sure your content contains the needed information for what the DLP policy is looking for when it is evaluated.</span></span>
  
<span data-ttu-id="c6aff-107">Например за правилата за номер на паспорт в **САЩ/Великобритания,** конфигурирани с ниво на достоверност от 75%, се оценяват следните и трябва да бъдат открити, за да се задейства правилото</span><span class="sxs-lookup"><span data-stu-id="c6aff-107">For example, for a **US/UK passport number** policy configured with a confidence level of 75%, the following are evaluated and must be detected for the rule to trigger</span></span>
  
- <span data-ttu-id="c6aff-108">**[Формат:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#format-77)** Девет цифри</span><span class="sxs-lookup"><span data-stu-id="c6aff-108">**[Format:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#format-77)** Nine digits</span></span>

- <span data-ttu-id="c6aff-109">**[Модел:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#pattern-77)** Девет последователни цифри</span><span class="sxs-lookup"><span data-stu-id="c6aff-109">**[Pattern:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#pattern-77)** Nine consecutive digits</span></span>

- <span data-ttu-id="c6aff-110">**[Контролна сума:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#checksum-76)** Не, няма контролна сума</span><span class="sxs-lookup"><span data-stu-id="c6aff-110">**[Checksum:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#checksum-76)** No, there is no Checksum</span></span>

- <span data-ttu-id="c6aff-111">**[Определение:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#definition-77)** Правилата на DLP са 75% уверени, че е открита тази информация, ако в близост до 300 знака:</span><span class="sxs-lookup"><span data-stu-id="c6aff-111">**[Definition:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#definition-77)** A DLP policy is 75% confident that it's detected this type of sensitive information if, within a proximity of 300 characters:</span></span>

  - <span data-ttu-id="c6aff-112">Функцията Func_usa_uk_passport намира съдържание, което съответства на модела.</span><span class="sxs-lookup"><span data-stu-id="c6aff-112">The function Func_usa_uk_passport finds content that matches the pattern.</span></span>

  - <span data-ttu-id="c6aff-113">Намерена е ключова дума от Keyword_passport.</span><span class="sxs-lookup"><span data-stu-id="c6aff-113">A keyword from Keyword_passport is found.</span></span>

    <span data-ttu-id="c6aff-114">Например, за правилата за номер на паспорт в **САЩ/Обединеното кралство** ще се задейства следната извадка: паспорт номер 123456789 в САЩ:</span><span class="sxs-lookup"><span data-stu-id="c6aff-114">For example, the following sample would trigger for the **US/UK passport number** policy: U.S. Passport number 123456789</span></span>

<span data-ttu-id="c6aff-115">За повече информация относно това, което е необходимо за да бъде открит номерът на паспорт за САЩ/Обединеното кралство за вашето съдържание, вижте следния раздел в тази статия: [Какво съдържа типовете чувствителни данни за САЩ/Великобритания паспортен номер](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#us--uk-passport-number)</span><span class="sxs-lookup"><span data-stu-id="c6aff-115">For more information on what is required for a US/UK Passport Number to be detected for your content, see the following section in this article: [What the Sensitive Information Types look for US/UK Passport Number](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#us--uk-passport-number)</span></span>
  
<span data-ttu-id="c6aff-116">С помощта на друг вграден тип поверителна информация вижте следната статия за информация за това какво е необходимо за други типове: [Какво се търси типовете информация за чувствителната информация](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions)</span><span class="sxs-lookup"><span data-stu-id="c6aff-116">Using a different built-in sensitive information type, see the following article for information on what is required for other types: [What the Sensitive Information Types look for](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions)</span></span>
  