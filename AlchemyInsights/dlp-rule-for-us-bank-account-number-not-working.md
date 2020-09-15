---
title: DLP правило за номер на банкова сметка в САЩ не работи
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
- "1287"
- "3200001"
ms.assetid: 80b40145-8376-4c3a-8d22-6efb9f9cb271
ms.openlocfilehash: eb399e4b23de32a757562833ed32d97daa6a1247
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: bg-BG
ms.lasthandoff: 09/14/2020
ms.locfileid: "47679285"
---
# <a name="dlp-issues-with-us-bank-account-numbers"></a><span data-ttu-id="164ec-102">DLP проблеми с номерата на банковите сметки в САЩ</span><span class="sxs-lookup"><span data-stu-id="164ec-102">DLP issues with US bank account numbers</span></span>

<span data-ttu-id="164ec-103">**Важно**: през тези безпрецедентни времена ние предприемаме стъпки, за да гарантираме, че услугите на SharePoint Online и OneDrive остават на пълно разположение – за повече информация посетете [Временни корекции на функции на SharePoint Online](https://aka.ms/ODSPAdjustments).</span><span class="sxs-lookup"><span data-stu-id="164ec-103">**Important**: During these unprecedented times, we are taking steps to ensure that SharePoint Online and OneDrive services remain highly available – Please visit [SharePoint Online Temporary Feature Adjustments](https://aka.ms/ODSPAdjustments) for more information.</span></span>

<span data-ttu-id="164ec-104">**DLP проблеми с номерата на банковите сметки в САЩ**</span><span class="sxs-lookup"><span data-stu-id="164ec-104">**DLP issues with US bank account numbers**</span></span>

<span data-ttu-id="164ec-105">Имате ли проблеми с **предотвратяване на загуба на данни (DLP)** , които не работят за съдържание, съдържащо **номер на банкова сметка в САЩ** , когато се използва тип на DLP за чувствителна информация в O365?</span><span class="sxs-lookup"><span data-stu-id="164ec-105">Are you having problems with **Data Loss Prevention (DLP)** not working for content containing a **US Bank Account Number** when using a DLP sensitive information type in O365?</span></span> <span data-ttu-id="164ec-106">Ако е така, трябва да се уверите, че вашето съдържание съдържа необходимата информация за това, което се търси в DLP политиката, когато бъде изчислена.</span><span class="sxs-lookup"><span data-stu-id="164ec-106">If so, make sure your content contains the needed information for what the DLP policy is looking for when it is evaluated.</span></span>
  
<span data-ttu-id="164ec-107">Например за правилата за **номер на банкова сметка в САЩ** , конфигурирани с ниво на надеждност от 85%, следва да бъдат оценени следните неща и трябва да бъдат открити, за да се задейства правилото:</span><span class="sxs-lookup"><span data-stu-id="164ec-107">For example, for a **US Bank Account Number** policy configured with a confidence level of 85%, the following are evaluated and must be detected for the rule to trigger:</span></span>
  
- <span data-ttu-id="164ec-108">**[Формат:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#format-77)** 8-17 цифри</span><span class="sxs-lookup"><span data-stu-id="164ec-108">**[Format:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#format-77)** 8-17 digits</span></span>

- <span data-ttu-id="164ec-109">**[Шарка:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#pattern-77)** 8-17 последователни цифри.</span><span class="sxs-lookup"><span data-stu-id="164ec-109">**[Pattern:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#pattern-77)** 8-17 consecutive digits.</span></span>

- <span data-ttu-id="164ec-110">**[Контролна сума:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#checksum-76)** Не, няма шах</span><span class="sxs-lookup"><span data-stu-id="164ec-110">**[Checksum:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#checksum-76)** No, there is no Checksum</span></span>

- <span data-ttu-id="164ec-111">**[Дефиниция:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions)** DLP правилата е 75% сигурни, че той е открил този тип поверителна информация, ако в близост до знаците на 300:</span><span class="sxs-lookup"><span data-stu-id="164ec-111">**[Definition:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions)** A DLP policy is 75% confident that it's detected this type of sensitive information if, within a proximity of 300 characters:</span></span>

  - <span data-ttu-id="164ec-112">Регулярният израз Regex_usa_bank_account_number намира съдържание, което съответства на модела</span><span class="sxs-lookup"><span data-stu-id="164ec-112">The regular expression Regex_usa_bank_account_number finds content that matches the pattern</span></span>

  - <span data-ttu-id="164ec-113">Намерена е ключова дума от Keyword_usa_Bank_Account.</span><span class="sxs-lookup"><span data-stu-id="164ec-113">A keyword from Keyword_usa_Bank_Account is found.</span></span>

    <span data-ttu-id="164ec-114">Например примерът по-долу би активирал за правилата за **номер на банкова сметка на САЩ** : проверка на акаунт 78344011</span><span class="sxs-lookup"><span data-stu-id="164ec-114">For example, the following sample would trigger for the **US Bank Account Number** policy: Checking Account 78344011</span></span>

<span data-ttu-id="164ec-115">За повече информация за това, което е необходимо, за да бъде открит **номерът на банкова сметка на САЩ** за вашето съдържание, вижте раздела по-долу в тази статия: [какви типове чувствителна информация търси в САЩ номер на банкова сметка](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#us-bank-account-number)</span><span class="sxs-lookup"><span data-stu-id="164ec-115">For more information on what is required for a **US Bank Account Number** to be detected for your content, see the following section in this article: [What the Sensitive Information Types look for US Bank Account Number](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#us-bank-account-number)</span></span>
  
<span data-ttu-id="164ec-116">С помощта на различен вграден тип чувствителна информация вижте статията по-долу за информация относно това, което е необходимо за други типове: [какви типове чувствителна информация търсите](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions)</span><span class="sxs-lookup"><span data-stu-id="164ec-116">Using a different built-in sensitive information type, see the following article for information on what is required for other types: [What the Sensitive Information Types look for](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions)</span></span>
  