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
ms.openlocfilehash: bb7d8ca91af73fa4ebed5992ec848128beb18830
ms.sourcegitcommit: d108a2da2f5dab05246e30b5108cca5173e09051
ms.translationtype: MT
ms.contentlocale: bg-BG
ms.lasthandoff: 03/26/2020
ms.locfileid: "42977151"
---
# <a name="dlp-issues-with-us-bank-account-numbers"></a><span data-ttu-id="628be-102">DLP проблеми с номера на банкови сметки в САЩ</span><span class="sxs-lookup"><span data-stu-id="628be-102">DLP issues with US bank account numbers</span></span>

<span data-ttu-id="628be-103">**Важно**: По време на тези безпрецедентни времена, ние предприемаме стъпки, за да се гарантира, че SharePoint Online и OneDrive услуги остават високо достъпни – посетете [SharePoint Online временни функция корекции](https://aka.ms/ODSPAdjustments) за повече информация.</span><span class="sxs-lookup"><span data-stu-id="628be-103">**Important**: During these unprecedented times, we are taking steps to ensure that SharePoint Online and OneDrive services remain highly available – Please visit [SharePoint Online Temporary Feature Adjustments](https://aka.ms/ODSPAdjustments) for more information.</span></span>

<span data-ttu-id="628be-104">**DLP проблеми с номера на банкови сметки в САЩ**</span><span class="sxs-lookup"><span data-stu-id="628be-104">**DLP issues with US bank account numbers**</span></span>

<span data-ttu-id="628be-105">Имате проблеми с **предотвратяване на загуба на данни (DLP)** не работи за съдържание, съдържащо номер на банкова сметка в **САЩ** при използване на тип на чувствителна тайнствена ИНФОРМАЦИЯ DLP в O365?</span><span class="sxs-lookup"><span data-stu-id="628be-105">Are you having problems with **Data Loss Prevention (DLP)** not working for content containing a **US Bank Account Number** when using a DLP sensitive information type in O365?</span></span> <span data-ttu-id="628be-106">Ако е така, уверете се, че съдържанието ви съдържа необходимата информация за това, което се търси dlp правила, когато се оценява.</span><span class="sxs-lookup"><span data-stu-id="628be-106">If so, make sure your content contains the needed information for what the DLP policy is looking for when it is evaluated.</span></span>
  
<span data-ttu-id="628be-107">Например за политика на **парични тет,** конфигурирани с ниво на сигурност от 85%, се оценяват следното и трябва да бъдат открити за правилото да се задейства:</span><span class="sxs-lookup"><span data-stu-id="628be-107">For example, for a **US Bank Account Number** policy configured with a confidence level of 85%, the following are evaluated and must be detected for the rule to trigger:</span></span>
  
- <span data-ttu-id="628be-108">**[Формат:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#format-77)** 8-17 цифри</span><span class="sxs-lookup"><span data-stu-id="628be-108">**[Format:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#format-77)** 8-17 digits</span></span>

- <span data-ttu-id="628be-109">**[Модел:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#pattern-77)** 8-17 последователни цифри.</span><span class="sxs-lookup"><span data-stu-id="628be-109">**[Pattern:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#pattern-77)** 8-17 consecutive digits.</span></span>

- <span data-ttu-id="628be-110">**[Контролна сума:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#checksum-76)** Не, няма чексума</span><span class="sxs-lookup"><span data-stu-id="628be-110">**[Checksum:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#checksum-76)** No, there is no Checksum</span></span>

- <span data-ttu-id="628be-111">**[Определение:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for)** DLP политика е 75% уверен, че е открит този тип чувствителна информация, ако в близост до 300 знака:</span><span class="sxs-lookup"><span data-stu-id="628be-111">**[Definition:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for)** A DLP policy is 75% confident that it's detected this type of sensitive information if, within a proximity of 300 characters:</span></span>

  - <span data-ttu-id="628be-112">Регулярният израз Regex_usa_bank_account_number намира съдържание, което съответства на</span><span class="sxs-lookup"><span data-stu-id="628be-112">The regular expression Regex_usa_bank_account_number finds content that matches the pattern</span></span>

  - <span data-ttu-id="628be-113">Намира се ключова дума от Keyword_usa_Bank_Account.</span><span class="sxs-lookup"><span data-stu-id="628be-113">A keyword from Keyword_usa_Bank_Account is found.</span></span>

    <span data-ttu-id="628be-114">Например следните примерни ще предизвика за сащ **парични номера** политика: проверка на акаунт 78344011</span><span class="sxs-lookup"><span data-stu-id="628be-114">For example, the following sample would trigger for the **US Bank Account Number** policy: Checking Account 78344011</span></span>

<span data-ttu-id="628be-115">За повече информация за това, какво е необходимо за да бъде открит **номер на банкова сметка** в САЩ за вашето съдържание, вижте раздела в тази статия: Какъв вид информация за [чувствителна тава търси за номер на банкова сметка в САЩ](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#us-bank-account-number)</span><span class="sxs-lookup"><span data-stu-id="628be-115">For more information on what is required for a **US Bank Account Number** to be detected for your content, see the following section in this article: [What the Sensitive Information Types look for US Bank Account Number](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#us-bank-account-number)</span></span>
  
<span data-ttu-id="628be-116">Използвайки друг вграден тип поверителна информация, вижте следната статия за информация за това какво се изисква за други типове: [Какво търсят типовете поверителна информация за](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for)</span><span class="sxs-lookup"><span data-stu-id="628be-116">Using a different built-in sensitive information type, see the following article for information on what is required for other types: [What the Sensitive Information Types look for](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for)</span></span>
  