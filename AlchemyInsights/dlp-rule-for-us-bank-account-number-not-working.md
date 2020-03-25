---
title: DLP правило за сащ номер на парични средства не работи
ms.author: deniseb
author: denisebmsft
manager: laurawi
ms.date: 11/5/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1287"
- "3200001"
ms.assetid: 80b40145-8376-4c3a-8d22-6efb9f9cb271
ms.openlocfilehash: 0b5c1fb175275028c56e47080708520fe115fb38
ms.sourcegitcommit: b0d5b68366028abcf08610672d5bc9d3b25ac433
ms.translationtype: MT
ms.contentlocale: bg-BG
ms.lasthandoff: 03/24/2020
ms.locfileid: "42932504"
---
# <a name="dlp-issues-with-us-bank-account-numbers"></a><span data-ttu-id="0a4bc-102">DLP проблеми с номера на банкови сметки в САЩ</span><span class="sxs-lookup"><span data-stu-id="0a4bc-102">DLP issues with US bank account numbers</span></span>

<span data-ttu-id="0a4bc-103">**Важно:** много sharePoint Online и OneDrive клиенти работят критични бизнес приложения срещу услугата, която се изпълнява във фонов режим.</span><span class="sxs-lookup"><span data-stu-id="0a4bc-103">**Important**: Many SharePoint Online and OneDrive customers run business-critical applications against the service that run in the background.</span></span> <span data-ttu-id="0a4bc-104">Те включват миграция на съдържанието, предотвратяване на загуба на данни (DLP) и архивиране на решения.</span><span class="sxs-lookup"><span data-stu-id="0a4bc-104">These include content migration, Data Loss Prevention (DLP), and backup solutions.</span></span> <span data-ttu-id="0a4bc-105">По време на тези безпрецедентни времена ние предприемаме стъпки, за да гарантираме, че SharePoint Online и OneDrive услуги остават високо достъпни и надеждни за вашите потребители, които зависят от услугата повече от всякога в отдалечени работни сценарии.</span><span class="sxs-lookup"><span data-stu-id="0a4bc-105">During these unprecedented times, we are taking steps to ensure that SharePoint Online and OneDrive services remain highly available and reliable for your users who depend on the service more than ever in remote work scenarios.</span></span>

<span data-ttu-id="0a4bc-106">В подкрепа на тази цел, ние сме внедрили по-строги ограничения за ограничаване на приложенията за фон (миграция, DLP и архивиране на решения) през делничните дни.</span><span class="sxs-lookup"><span data-stu-id="0a4bc-106">In support of this objective, we have implemented tighter throttling limits on background apps (migration, DLP and backup solutions) during weekday daytime hours.</span></span> <span data-ttu-id="0a4bc-107">Трябва да очаквате, че тези приложения ще постигнат много ограничена пропускателна информация по време на тези времена.</span><span class="sxs-lookup"><span data-stu-id="0a4bc-107">You should expect that these apps will achieve very limited throughput during these times.</span></span> <span data-ttu-id="0a4bc-108">Въпреки това, по време на вечерните и почивните часове за региона, услугата ще бъде готова да обработи значително по-голям обем заявки от приложения за фон.</span><span class="sxs-lookup"><span data-stu-id="0a4bc-108">However, during evening and weekend hours for the region, the service will be ready to process a significantly higher volume of requests from background apps.</span></span>

<span data-ttu-id="0a4bc-109">**DLP проблеми с номера на банкови сметки в САЩ**</span><span class="sxs-lookup"><span data-stu-id="0a4bc-109">**DLP issues with US bank account numbers**</span></span>

<span data-ttu-id="0a4bc-110">Имате проблеми с **предотвратяване на загуба на данни (DLP)** не работи за съдържание, съдържащо номер на банкова сметка в **САЩ** при използване на тип на чувствителна тайнствена ИНФОРМАЦИЯ DLP в O365?</span><span class="sxs-lookup"><span data-stu-id="0a4bc-110">Are you having problems with **Data Loss Prevention (DLP)** not working for content containing a **US Bank Account Number** when using a DLP sensitive information type in O365?</span></span> <span data-ttu-id="0a4bc-111">Ако е така, уверете се, че съдържанието ви съдържа необходимата информация за това, което се търси dlp правила, когато се оценява.</span><span class="sxs-lookup"><span data-stu-id="0a4bc-111">If so, make sure your content contains the needed information for what the DLP policy is looking for when it is evaluated.</span></span>
  
<span data-ttu-id="0a4bc-112">Например за политика на **парични тет,** конфигурирани с ниво на сигурност от 85%, се оценяват следното и трябва да бъдат открити за правилото да се задейства:</span><span class="sxs-lookup"><span data-stu-id="0a4bc-112">For example, for a **US Bank Account Number** policy configured with a confidence level of 85%, the following are evaluated and must be detected for the rule to trigger:</span></span>
  
- <span data-ttu-id="0a4bc-113">**[Формат:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#format-77)** 8-17 цифри</span><span class="sxs-lookup"><span data-stu-id="0a4bc-113">**[Format:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#format-77)** 8-17 digits</span></span>

- <span data-ttu-id="0a4bc-114">**[Модел:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#pattern-77)** 8-17 последователни цифри.</span><span class="sxs-lookup"><span data-stu-id="0a4bc-114">**[Pattern:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#pattern-77)** 8-17 consecutive digits.</span></span>

- <span data-ttu-id="0a4bc-115">**[Контролна сума:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#checksum-76)** Не, няма чексума</span><span class="sxs-lookup"><span data-stu-id="0a4bc-115">**[Checksum:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#checksum-76)** No, there is no Checksum</span></span>

- <span data-ttu-id="0a4bc-116">**[Определение:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for)** DLP политика е 75% уверен, че е открит този тип чувствителна информация, ако в близост до 300 знака:</span><span class="sxs-lookup"><span data-stu-id="0a4bc-116">**[Definition:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for)** A DLP policy is 75% confident that it's detected this type of sensitive information if, within a proximity of 300 characters:</span></span>

  - <span data-ttu-id="0a4bc-117">Регулярният израз Regex_usa_bank_account_number намира съдържание, което съответства на</span><span class="sxs-lookup"><span data-stu-id="0a4bc-117">The regular expression Regex_usa_bank_account_number finds content that matches the pattern</span></span>

  - <span data-ttu-id="0a4bc-118">Намира се ключова дума от Keyword_usa_Bank_Account.</span><span class="sxs-lookup"><span data-stu-id="0a4bc-118">A keyword from Keyword_usa_Bank_Account is found.</span></span>

    <span data-ttu-id="0a4bc-119">Например следните примерни ще предизвика за сащ **парични номера** политика: проверка на акаунт 78344011</span><span class="sxs-lookup"><span data-stu-id="0a4bc-119">For example, the following sample would trigger for the **US Bank Account Number** policy: Checking Account 78344011</span></span>

<span data-ttu-id="0a4bc-120">За повече информация за това, какво е необходимо за да бъде открит **номер на банкова сметка** в САЩ за вашето съдържание, вижте раздела в тази статия: Какъв вид информация за [чувствителна тава търси за номер на банкова сметка в САЩ](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#us-bank-account-number)</span><span class="sxs-lookup"><span data-stu-id="0a4bc-120">For more information on what is required for a **US Bank Account Number** to be detected for your content, see the following section in this article: [What the Sensitive Information Types look for US Bank Account Number](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#us-bank-account-number)</span></span>
  
<span data-ttu-id="0a4bc-121">Използвайки друг вграден тип поверителна информация, вижте следната статия за информация за това какво се изисква за други типове: [Какво търсят типовете поверителна информация за](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for)</span><span class="sxs-lookup"><span data-stu-id="0a4bc-121">Using a different built-in sensitive information type, see the following article for information on what is required for other types: [What the Sensitive Information Types look for](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for)</span></span>
  