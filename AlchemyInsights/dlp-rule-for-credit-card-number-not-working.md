---
title: DLP правило за кредитна карта номер не работи
ms.author: deniseb
author: denisebmsft
manager: laurawi
ms.date: 11/5/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1270"
- "3200001"
ms.assetid: 30496c79-c8b4-4337-a46d-abed12864209
ms.openlocfilehash: 6b28534d072c024a98a9b05f6cb55bfdc3435db6
ms.sourcegitcommit: b0d5b68366028abcf08610672d5bc9d3b25ac433
ms.translationtype: MT
ms.contentlocale: bg-BG
ms.lasthandoff: 03/24/2020
ms.locfileid: "42932432"
---
# <a name="dlp-issues-with-credit-card-numbers"></a><span data-ttu-id="7c969-102">DLP проблеми с номера на кредитни карти</span><span class="sxs-lookup"><span data-stu-id="7c969-102">DLP issues with credit card numbers</span></span>

<span data-ttu-id="7c969-103">**Важно:** много sharePoint Online и OneDrive клиенти работят критични бизнес приложения срещу услугата, която се изпълнява във фонов режим.</span><span class="sxs-lookup"><span data-stu-id="7c969-103">**Important**: Many SharePoint Online and OneDrive customers run business-critical applications against the service that run in the background.</span></span> <span data-ttu-id="7c969-104">Те включват миграция на съдържанието, предотвратяване на загуба на данни (DLP) и архивиране на решения.</span><span class="sxs-lookup"><span data-stu-id="7c969-104">These include content migration, Data Loss Prevention (DLP), and backup solutions.</span></span> <span data-ttu-id="7c969-105">По време на тези безпрецедентни времена ние предприемаме стъпки, за да гарантираме, че SharePoint Online и OneDrive услуги остават високо достъпни и надеждни за вашите потребители, които зависят от услугата повече от всякога в отдалечени работни сценарии.</span><span class="sxs-lookup"><span data-stu-id="7c969-105">During these unprecedented times, we are taking steps to ensure that SharePoint Online and OneDrive services remain highly available and reliable for your users who depend on the service more than ever in remote work scenarios.</span></span>

<span data-ttu-id="7c969-106">В подкрепа на тази цел, ние сме внедрили по-строги ограничения за ограничаване на приложенията за фон (миграция, DLP и архивиране на решения) през делничните дни.</span><span class="sxs-lookup"><span data-stu-id="7c969-106">In support of this objective, we have implemented tighter throttling limits on background apps (migration, DLP and backup solutions) during weekday daytime hours.</span></span> <span data-ttu-id="7c969-107">Трябва да очаквате, че тези приложения ще постигнат много ограничена пропускателна информация по време на тези времена.</span><span class="sxs-lookup"><span data-stu-id="7c969-107">You should expect that these apps will achieve very limited throughput during these times.</span></span> <span data-ttu-id="7c969-108">Въпреки това, по време на вечерните и почивните часове за региона, услугата ще бъде готова да обработи значително по-голям обем заявки от приложения за фон.</span><span class="sxs-lookup"><span data-stu-id="7c969-108">However, during evening and weekend hours for the region, the service will be ready to process a significantly higher volume of requests from background apps.</span></span>

<span data-ttu-id="7c969-109">**DLP проблеми с номера на кредитни карти**</span><span class="sxs-lookup"><span data-stu-id="7c969-109">**DLP issues with credit card numbers**</span></span>

<span data-ttu-id="7c969-110">Имате проблеми с **предотвратяване на загуба на данни (DLP)** не работи за съдържание, съдържащо номер на кредитна **карта,** когато използвате тип на чувствителна тайнствена СТОЙНОСТ в O365?</span><span class="sxs-lookup"><span data-stu-id="7c969-110">Are you having problems with **Data Loss Prevention (DLP)** not working for content containing a **Credit Card Number** when using a DLP sensitive information type in O365?</span></span> <span data-ttu-id="7c969-111">Ако е така, уверете се, че съдържанието ви съдържа необходимата информация за задействане на правилата на DLP, когато се оценява.</span><span class="sxs-lookup"><span data-stu-id="7c969-111">If so, make sure your content contains the needed information to trigger the the DLP policy when it is evaluated.</span></span> <span data-ttu-id="7c969-112">Например за правила за **кредитна карта,** конфигурирани с ниво на сигурност от 85%, се оценяват следните и трябва да бъдат открити, за да се задейства правилото:</span><span class="sxs-lookup"><span data-stu-id="7c969-112">For example, for a **Credit Card policy** configured with a confidence level of 85%, the following are evaluated and must be detected for the rule to trigger:</span></span>
  
- <span data-ttu-id="7c969-113">**[Формат:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#format-19)** 16 цифри, които могат да бъдат форматирани или неформатирани (dddddddddddddddddddddddddddddddddddddddddddddddddddddddddddddddddddddddddddddddddddddddddddddddddddddddddddd</span><span class="sxs-lookup"><span data-stu-id="7c969-113">**[Format:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#format-19)** 16 digits which can be formatted or unformatted (dddddddddddddddd) and must pass the Luhn test.</span></span>

- <span data-ttu-id="7c969-114">**[Модел:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#pattern-19)** Много сложен и здрав модел, който открива карти от всички основни марки в света, включително Visa, MasterCard, Discover Card, JCB, American Express, карти за подаръци и карти за закусва.</span><span class="sxs-lookup"><span data-stu-id="7c969-114">**[Pattern:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#pattern-19)** Very complex and robust pattern that detects cards from all major brands worldwide, including Visa, MasterCard, Discover Card, JCB, American Express, gift cards, and diner cards.</span></span>

- <span data-ttu-id="7c969-115">**[Контролна сума:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#checksum-19)** Да, чексумата на Луен</span><span class="sxs-lookup"><span data-stu-id="7c969-115">**[Checksum:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#checksum-19)** Yes, the Luhn checksum</span></span>

- <span data-ttu-id="7c969-116">**[Определение:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#definition-19)** DLP политика е 85% уверен, че е открит този тип чувствителна информация, ако в близост до 300 знака:</span><span class="sxs-lookup"><span data-stu-id="7c969-116">**[Definition:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#definition-19)** A DLP policy is 85% confident that it's detected this type of sensitive information if, within a proximity of 300 characters:</span></span>

  - <span data-ttu-id="7c969-117">Функцията Func_credit_card намира съдържание, което съответства на шаблона.</span><span class="sxs-lookup"><span data-stu-id="7c969-117">The function Func_credit_card finds content that matches the pattern.</span></span>

  - <span data-ttu-id="7c969-118">Едно от следните неща е вярно:</span><span class="sxs-lookup"><span data-stu-id="7c969-118">One of the following is true:</span></span>

  - <span data-ttu-id="7c969-119">Намерена е ключова дума от Keyword_cc_verification.</span><span class="sxs-lookup"><span data-stu-id="7c969-119">A keyword from Keyword_cc_verification is found.</span></span>

  - <span data-ttu-id="7c969-120">Намерена е ключова дума от Keyword_cc_name</span><span class="sxs-lookup"><span data-stu-id="7c969-120">A keyword from Keyword_cc_name is found</span></span>

  - <span data-ttu-id="7c969-121">Функцията Func_expiration_date намира дата в правилния формат на датата.</span><span class="sxs-lookup"><span data-stu-id="7c969-121">The function Func_expiration_date finds a date in the right date format.</span></span>

  - <span data-ttu-id="7c969-122">Контролната сума</span><span class="sxs-lookup"><span data-stu-id="7c969-122">The checksum passes</span></span>

    <span data-ttu-id="7c969-123">Например следните примерни ще предизвика за DLP кредитна карта номер политика:</span><span class="sxs-lookup"><span data-stu-id="7c969-123">For example, the following sample would trigger for a DLP Credit Card Number Policy:</span></span>

  - <span data-ttu-id="7c969-124">Виза: 4485 3647 3952 7352</span><span class="sxs-lookup"><span data-stu-id="7c969-124">Visa: 4485 3647 3952 7352</span></span>
  
  - <span data-ttu-id="7c969-125">Изтича на: 2/2009</span><span class="sxs-lookup"><span data-stu-id="7c969-125">Expires: 2/2009</span></span>

<span data-ttu-id="7c969-126">За повече информация относно това, което е необходимо за да бъде открит **номер на кредитна карта** за вашето съдържание, вижте следния раздел в тази статия: Какви типове [поверителна информация търсят кредитна карта#](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#credit-card-number)</span><span class="sxs-lookup"><span data-stu-id="7c969-126">For more information on what is required for a **Credit Card Number** to be detected for your content, see the following section in this article: [What the Sensitive Information Types look for Credit Card#](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#credit-card-number)</span></span>
  
<span data-ttu-id="7c969-127">Използвайки друг вграден тип поверителна информация, вижте следната статия за информация за това какво се изисква за други типове: [Какво търсят типовете поверителна информация за](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for)</span><span class="sxs-lookup"><span data-stu-id="7c969-127">Using a different built-in sensitive information type, see the following article for information on what is required for other types: [What the Sensitive Information Types look for](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for)</span></span>
  