---
title: DLP правило за САЩ/Великобритания номер на паспорт не работи
ms.author: deniseb
author: denisebmsft
manager: laurawi
ms.date: 11/5/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1319"
- "3200001"
ms.assetid: fc178b8b-943b-4346-a2bd-a75c6af6f80f
ms.openlocfilehash: c63e814059c897531109aa78725e9811b311fb27
ms.sourcegitcommit: b0d5b68366028abcf08610672d5bc9d3b25ac433
ms.translationtype: MT
ms.contentlocale: bg-BG
ms.lasthandoff: 03/24/2020
ms.locfileid: "42931251"
---
# <a name="problems-with-dlp---usuk-passport-numbers"></a><span data-ttu-id="1cef3-102">Проблеми с DLP - САЩ /UK номера на паспорти</span><span class="sxs-lookup"><span data-stu-id="1cef3-102">Problems with DLP - US/UK passport numbers</span></span>

<span data-ttu-id="1cef3-103">**Важно:** много sharePoint Online и OneDrive клиенти работят критични бизнес приложения срещу услугата, която се изпълнява във фонов режим.</span><span class="sxs-lookup"><span data-stu-id="1cef3-103">**Important**: Many SharePoint Online and OneDrive customers run business-critical applications against the service that run in the background.</span></span> <span data-ttu-id="1cef3-104">Те включват миграция на съдържанието, предотвратяване на загуба на данни (DLP) и архивиране на решения.</span><span class="sxs-lookup"><span data-stu-id="1cef3-104">These include content migration, Data Loss Prevention (DLP), and backup solutions.</span></span> <span data-ttu-id="1cef3-105">По време на тези безпрецедентни времена ние предприемаме стъпки, за да гарантираме, че SharePoint Online и OneDrive услуги остават високо достъпни и надеждни за вашите потребители, които зависят от услугата повече от всякога в отдалечени работни сценарии.</span><span class="sxs-lookup"><span data-stu-id="1cef3-105">During these unprecedented times, we are taking steps to ensure that SharePoint Online and OneDrive services remain highly available and reliable for your users who depend on the service more than ever in remote work scenarios.</span></span>

<span data-ttu-id="1cef3-106">В подкрепа на тази цел, ние сме внедрили по-строги ограничения за ограничаване на приложенията за фон (миграция, DLP и архивиране на решения) през делничните дни.</span><span class="sxs-lookup"><span data-stu-id="1cef3-106">In support of this objective, we have implemented tighter throttling limits on background apps (migration, DLP and backup solutions) during weekday daytime hours.</span></span> <span data-ttu-id="1cef3-107">Трябва да очаквате, че тези приложения ще постигнат много ограничена пропускателна информация по време на тези времена.</span><span class="sxs-lookup"><span data-stu-id="1cef3-107">You should expect that these apps will achieve very limited throughput during these times.</span></span> <span data-ttu-id="1cef3-108">Въпреки това, по време на вечерните и почивните часове за региона, услугата ще бъде готова да обработи значително по-голям обем заявки от приложения за фон.</span><span class="sxs-lookup"><span data-stu-id="1cef3-108">However, during evening and weekend hours for the region, the service will be ready to process a significantly higher volume of requests from background apps.</span></span>

<span data-ttu-id="1cef3-109">**DLP проблеми с американски/великобритания паспортни номера**</span><span class="sxs-lookup"><span data-stu-id="1cef3-109">**DLP issues with US/UK passport numbers**</span></span>

<span data-ttu-id="1cef3-110">Имате проблеми с **предотвратяване на загуба на данни (DLP)** не работи за съдържание, съдържащо номер на **американски/английски паспорт** при използване на тип на чувствителна тайнствена ИНФОРМАЦИЯ DLP в O365?</span><span class="sxs-lookup"><span data-stu-id="1cef3-110">Are you having problems with **Data Loss Prevention (DLP)** not working for content containing a **US/UK passport number** when using a DLP sensitive information type in O365?</span></span> <span data-ttu-id="1cef3-111">Ако е така, уверете се, че съдържанието ви съдържа необходимата информация за това, което се търси dlp правила, когато се оценява.</span><span class="sxs-lookup"><span data-stu-id="1cef3-111">If so, make sure your content contains the needed information for what the DLP policy is looking for when it is evaluated.</span></span>
  
<span data-ttu-id="1cef3-112">Например, за политика за **номер на паспорт сащ/Обединеното кралство,** конфигурирана с ниво на сигурност от 75%, се оценяват следните и трябва да бъдат открити, за да се задейства правилото</span><span class="sxs-lookup"><span data-stu-id="1cef3-112">For example, for a **US/UK passport number** policy configured with a confidence level of 75%, the following are evaluated and must be detected for the rule to trigger</span></span>
  
- <span data-ttu-id="1cef3-113">**[Формат на](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#format-77)** Девет цифри</span><span class="sxs-lookup"><span data-stu-id="1cef3-113">**[Format:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#format-77)** Nine digits</span></span>

- <span data-ttu-id="1cef3-114">**[Модел:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#pattern-77)** Девет последователни цифри</span><span class="sxs-lookup"><span data-stu-id="1cef3-114">**[Pattern:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#pattern-77)** Nine consecutive digits</span></span>

- <span data-ttu-id="1cef3-115">**[Контролна сума:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#checksum-76)** Не, няма чексума</span><span class="sxs-lookup"><span data-stu-id="1cef3-115">**[Checksum:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#checksum-76)** No, there is no Checksum</span></span>

- <span data-ttu-id="1cef3-116">**[Определение:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#definition-77)** DLP политика е 75% уверен, че е открит този тип чувствителна информация, ако в близост до 300 знака:</span><span class="sxs-lookup"><span data-stu-id="1cef3-116">**[Definition:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#definition-77)** A DLP policy is 75% confident that it's detected this type of sensitive information if, within a proximity of 300 characters:</span></span>

  - <span data-ttu-id="1cef3-117">Функцията Func_usa_uk_passport намира съдържание, което съответства на шаблона.</span><span class="sxs-lookup"><span data-stu-id="1cef3-117">The function Func_usa_uk_passport finds content that matches the pattern.</span></span>

  - <span data-ttu-id="1cef3-118">Намира се ключова дума от Keyword_passport.</span><span class="sxs-lookup"><span data-stu-id="1cef3-118">A keyword from Keyword_passport is found.</span></span>

    <span data-ttu-id="1cef3-119">Например следната извадка ще задейства за **САЩ/Великобритания паспорт номер** политика: Номер на паспорт а в САЩ 123456789</span><span class="sxs-lookup"><span data-stu-id="1cef3-119">For example, the following sample would trigger for the **US/UK passport number** policy: U.S. Passport number 123456789</span></span>

<span data-ttu-id="1cef3-120">За повече информация относно това, което е необходимо за да бъде открит номер на американски/британски паспорт за вашето съдържание, вижте раздела по-долу в тази статия: [Какви типове информация за сащ/Великобритания търсят за сащ/UK Passport Number](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#us--uk-passport-number)</span><span class="sxs-lookup"><span data-stu-id="1cef3-120">For more information on what is required for a US/UK Passport Number to be detected for your content, see the following section in this article: [What the Sensitive Information Types look for US/UK Passport Number](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#us--uk-passport-number)</span></span>
  
<span data-ttu-id="1cef3-121">Използвайки друг вграден тип поверителна информация, вижте следната статия за информация за това какво се изисква за други типове: [Какво търсят типовете поверителна информация за](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for)</span><span class="sxs-lookup"><span data-stu-id="1cef3-121">Using a different built-in sensitive information type, see the following article for information on what is required for other types: [What the Sensitive Information Types look for](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for)</span></span>
  