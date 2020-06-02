---
title: DLP правило за кредитна карта номер не работи
ms.author: deniseb
author: denisebmsft
manager: laurawi
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1270"
- "3200001"
ms.assetid: 30496c79-c8b4-4337-a46d-abed12864209
ms.openlocfilehash: e2e93bed44749b9017dc6ff919a151d46da7a3fc
ms.sourcegitcommit: bc7d6f4f3c9f7060d073f5130e1ec856e248d020
ms.translationtype: MT
ms.contentlocale: bg-BG
ms.lasthandoff: 06/02/2020
ms.locfileid: "44507395"
---
# <a name="dlp-issues-with-credit-card-numbers"></a><span data-ttu-id="98299-102">Проблеми с DLP с номера на кредитни карти</span><span class="sxs-lookup"><span data-stu-id="98299-102">DLP issues with credit card numbers</span></span>

<span data-ttu-id="98299-103">**Важно**: през тези безпрецедентни времена ние предприемаме стъпки, за да гарантираме, че услугите на SharePoint Online и OneDrive остават на пълно разположение – за повече информация посетете [Временни корекции на функции на SharePoint Online](https://aka.ms/ODSPAdjustments).</span><span class="sxs-lookup"><span data-stu-id="98299-103">**Important**: During these unprecedented times, we are taking steps to ensure that SharePoint Online and OneDrive services remain highly available – Please visit [SharePoint Online Temporary Feature Adjustments](https://aka.ms/ODSPAdjustments) for more information.</span></span>

<span data-ttu-id="98299-104">**Проблеми с DLP с номера на кредитни карти**</span><span class="sxs-lookup"><span data-stu-id="98299-104">**DLP issues with credit card numbers**</span></span>

<span data-ttu-id="98299-105">Имате проблеми с **предотвратяване на загуба на данни (DLP),** които не работят за съдържание, съдържащо номер на кредитна **карта,** когато използвате DLP чувствителен тип информация в O365?</span><span class="sxs-lookup"><span data-stu-id="98299-105">Are you having problems with **Data Loss Prevention (DLP)** not working for content containing a **Credit Card Number** when using a DLP sensitive information type in O365?</span></span> <span data-ttu-id="98299-106">Ако е така, уверете се, че съдържанието съдържа необходимата информация, за да задействате правилата на DLP, когато се оценява.</span><span class="sxs-lookup"><span data-stu-id="98299-106">If so, make sure your content contains the needed information to trigger the the DLP policy when it is evaluated.</span></span> <span data-ttu-id="98299-107">Например за **кредитна карта правила** конфигуриран с ниво на доверие от 85 %, се оценяват следното и трябва да бъдат открити за правилото да задейства:</span><span class="sxs-lookup"><span data-stu-id="98299-107">For example, for a **Credit Card policy** configured with a confidence level of 85%, the following are evaluated and must be detected for the rule to trigger:</span></span>
  
- <span data-ttu-id="98299-108">**[Формат:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#format-19)** 16 цифри, които могат да бъдат форматирани или неформатирани (ddddddddddddddddddddddddddddddddddddddddddddddddddddddddddddddddddddddddddddddddddddddddddddddddddddddddddddddd)</span><span class="sxs-lookup"><span data-stu-id="98299-108">**[Format:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#format-19)** 16 digits which can be formatted or unformatted (dddddddddddddddd) and must pass the Luhn test.</span></span>

- <span data-ttu-id="98299-109">**[Модел:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#pattern-19)** Много сложен и здрав модел, който открива карти от всички големи марки в света, включително Visa, MasterCard, Discover Card, JCB, American Express, карти за подаръчни подаръци, и закусвални карти.</span><span class="sxs-lookup"><span data-stu-id="98299-109">**[Pattern:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#pattern-19)** Very complex and robust pattern that detects cards from all major brands worldwide, including Visa, MasterCard, Discover Card, JCB, American Express, gift cards, and diner cards.</span></span>

- <span data-ttu-id="98299-110">**[Контролна сума:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#checksum-19)** Да, сумата на Лун</span><span class="sxs-lookup"><span data-stu-id="98299-110">**[Checksum:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#checksum-19)** Yes, the Luhn checksum</span></span>

- <span data-ttu-id="98299-111">**[Определение:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#definition-19)** DLP политика е 85% уверени, че е открита този тип чувствителна информация, ако в близост до 300 знака:</span><span class="sxs-lookup"><span data-stu-id="98299-111">**[Definition:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#definition-19)** A DLP policy is 85% confident that it's detected this type of sensitive information if, within a proximity of 300 characters:</span></span>

  - <span data-ttu-id="98299-112">Функцията Func_credit_card намира съдържание, което съответства на модела.</span><span class="sxs-lookup"><span data-stu-id="98299-112">The function Func_credit_card finds content that matches the pattern.</span></span>

  - <span data-ttu-id="98299-113">Едно от следните е вярно:</span><span class="sxs-lookup"><span data-stu-id="98299-113">One of the following is true:</span></span>

  - <span data-ttu-id="98299-114">Намерена е ключова дума от Keyword_cc_verification.</span><span class="sxs-lookup"><span data-stu-id="98299-114">A keyword from Keyword_cc_verification is found.</span></span>

  - <span data-ttu-id="98299-115">Намерена е ключова дума от Keyword_cc_name</span><span class="sxs-lookup"><span data-stu-id="98299-115">A keyword from Keyword_cc_name is found</span></span>

  - <span data-ttu-id="98299-116">Функцията Func_expiration_date намери дата в правилния формат на датата.</span><span class="sxs-lookup"><span data-stu-id="98299-116">The function Func_expiration_date finds a date in the right date format.</span></span>

  - <span data-ttu-id="98299-117">Контролната сума преминава</span><span class="sxs-lookup"><span data-stu-id="98299-117">The checksum passes</span></span>

    <span data-ttu-id="98299-118">Например следната пример ще задейства DLP кредитна карта номер политика:</span><span class="sxs-lookup"><span data-stu-id="98299-118">For example, the following sample would trigger for a DLP Credit Card Number Policy:</span></span>

  - <span data-ttu-id="98299-119">Виза: 4485 3647 3952 7352</span><span class="sxs-lookup"><span data-stu-id="98299-119">Visa: 4485 3647 3952 7352</span></span>
  
  - <span data-ttu-id="98299-120">Изтича на: 2/2009</span><span class="sxs-lookup"><span data-stu-id="98299-120">Expires: 2/2009</span></span>

<span data-ttu-id="98299-121">За повече информация относно това, което е необходимо за да бъде открит **номер на кредитна карта** за вашето съдържание, вижте следния раздел в тази статия: Какво чувствителна информация видове изглежда за кредитна карта [#](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#credit-card-number)</span><span class="sxs-lookup"><span data-stu-id="98299-121">For more information on what is required for a **Credit Card Number** to be detected for your content, see the following section in this article: [What the Sensitive Information Types look for Credit Card#](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#credit-card-number)</span></span>
  
<span data-ttu-id="98299-122">С помощта на друг вграден тип поверителна информация вижте следната статия за информация за това какво е необходимо за други типове: [Какво се търси типовете информация за чувствителната информация](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions)</span><span class="sxs-lookup"><span data-stu-id="98299-122">Using a different built-in sensitive information type, see the following article for information on what is required for other types: [What the Sensitive Information Types look for](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions)</span></span>
  