---
title: DLP не работи по очаквания начин
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
- "1241"
- "3200001"
ms.assetid: f6fcf5ad-55a1-4f25-af27-1f7c1ce06409
ms.openlocfilehash: 0ed893420b5813d5d18639c2c226c12f0306a13f
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: bg-BG
ms.lasthandoff: 09/14/2020
ms.locfileid: "47679682"
---
# <a name="dlp-not-working-as-expected"></a><span data-ttu-id="e9884-102">DLP не работи по очаквания начин</span><span class="sxs-lookup"><span data-stu-id="e9884-102">DLP not working as expected</span></span>

<span data-ttu-id="e9884-103">**Важно**: през тези безпрецедентни времена ние предприемаме стъпки, за да гарантираме, че услугите на SharePoint Online и OneDrive остават на пълно разположение – за повече информация посетете [Временни корекции на функции на SharePoint Online](https://aka.ms/ODSPAdjustments).</span><span class="sxs-lookup"><span data-stu-id="e9884-103">**Important**: During these unprecedented times, we are taking steps to ensure that SharePoint Online and OneDrive services remain highly available – Please visit [SharePoint Online Temporary Feature Adjustments](https://aka.ms/ODSPAdjustments) for more information.</span></span>

 <span data-ttu-id="e9884-104">**Настройване на DLP**</span><span class="sxs-lookup"><span data-stu-id="e9884-104">**Setting up DLP**</span></span>

<span data-ttu-id="e9884-105">Имате ли проблеми с **предотвратяване на загуба на данни (DLP)** в Office 365 не работи, както се очаква?</span><span class="sxs-lookup"><span data-stu-id="e9884-105">Are you having problems with **Data Loss Prevention (DLP)** in Office 365 not working as expected?</span></span> <span data-ttu-id="e9884-106">Ако е така, уверете се, че вашата **DLP политика** е настроена правилно и че вашите данни съдържат това, което се намира в **DLP политиката** , когато тя се изчислява.</span><span class="sxs-lookup"><span data-stu-id="e9884-106">If so, make sure that your **DLP policy** is set up correctly, and that your data contains what the **DLP policy** is looking for when it is being evaluated.</span></span>
  
<span data-ttu-id="e9884-107">DLP правила ви позволява да идентифицирате и защитавате поверителната информация във вашата организация.</span><span class="sxs-lookup"><span data-stu-id="e9884-107">DLP policies allows you to identify and protect sensitive information in your organization.</span></span> <span data-ttu-id="e9884-108">За да настроите DLP правила, използвайте информацията [тук](https://docs.microsoft.com/office365/securitycompliance/prevent-data-loss#set-up-dlp).</span><span class="sxs-lookup"><span data-stu-id="e9884-108">To setup DLP policies, use the information [here](https://docs.microsoft.com/office365/securitycompliance/prevent-data-loss#set-up-dlp).</span></span>
  
 <span data-ttu-id="e9884-109">**Какви правила за DLP търсят**</span><span class="sxs-lookup"><span data-stu-id="e9884-109">**What DLP policies look for**</span></span>
  
<span data-ttu-id="e9884-110">Когато използвате **вградените типове деликатни данни** в центъра за защита и съответствие, DLP правилата търсят определени модели и елементи, когато откриват тези типове чувствителни.</span><span class="sxs-lookup"><span data-stu-id="e9884-110">When using the **built-in sensitive information types** in the Security and Compliance centers, DLP policies look for specific patterns and elements when detecting these sensitive types.</span></span>
  
- <span data-ttu-id="e9884-111">**Вградени типове деликатни данни**</span><span class="sxs-lookup"><span data-stu-id="e9884-111">**Built-in Sensitive Information Types**</span></span>

    <span data-ttu-id="e9884-112">За информация относно вградените типове чувствителни и за това какво търси DLP политика при откриването на типа чувствителна, вижте: [какви типове чувствителна информация търсите](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions).</span><span class="sxs-lookup"><span data-stu-id="e9884-112">For information on the built-in Sensitive types and what a DLP policy looks for when detecting the Sensitive type, see: [What the sensitive information types look for](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions).</span></span>

- <span data-ttu-id="e9884-113">**Типове чувствителна информация по избор**</span><span class="sxs-lookup"><span data-stu-id="e9884-113">**Custom Sensitive Information Types**</span></span>

    <span data-ttu-id="e9884-114">Ако се опитвате да създадете типове чувствителна информация по избор, използвайте следната статия за информация как да създадете персонализиран тип чувствителна информация: [Създаване на персонализиран тип данни по избор](https://docs.microsoft.com/microsoft-365/compliance/create-a-custom-sensitive-information-type).</span><span class="sxs-lookup"><span data-stu-id="e9884-114">If you are trying to create custom sensitive information types, use the following article for information on how to create a custom sensitive type: [Create a custom sensitive information type](https://docs.microsoft.com/microsoft-365/compliance/create-a-custom-sensitive-information-type).</span></span>

<span data-ttu-id="e9884-115">**Тестване на DLP правила**</span><span class="sxs-lookup"><span data-stu-id="e9884-115">**Test a DLP policy**</span></span>

<span data-ttu-id="e9884-116">За да тествате вашите данни с помощта на вграден или персонализиран тип информация, използвайте опцията **тип** на теста **под**  >  **типове чувствителна информация**.</span><span class="sxs-lookup"><span data-stu-id="e9884-116">To test your data with a built-in or custom sensitive information type, use the **Test type** option under **Classifications** > **Sensitive info types**.</span></span> <span data-ttu-id="e9884-117">За повече информация вижте [проверка на типовете чувствителна информация по избор](https://docs.microsoft.com/microsoft-365/compliance/create-a-custom-sensitive-information-type#create-custom-sensitive-information-types-in-the-security--compliance-center).</span><span class="sxs-lookup"><span data-stu-id="e9884-117">For more information, see [Test custom sensitive information types](https://docs.microsoft.com/microsoft-365/compliance/create-a-custom-sensitive-information-type#create-custom-sensitive-information-types-in-the-security--compliance-center).</span></span>

 <span data-ttu-id="e9884-118">**Отчети**</span><span class="sxs-lookup"><span data-stu-id="e9884-118">**Reports**</span></span>
  
- <span data-ttu-id="e9884-119">Получете данни за чувствителна информация с [DLP отчети.](https://docs.microsoft.com/microsoft-365/compliance/data-loss-prevention-policies#dlp-reports)</span><span class="sxs-lookup"><span data-stu-id="e9884-119">Get sensitive data insights with [DLP Reports.](https://docs.microsoft.com/microsoft-365/compliance/data-loss-prevention-policies#dlp-reports)</span></span>

- <span data-ttu-id="e9884-120">Вижте конкретни подробности за събитието със съобщение за [инцидент](https://docs.microsoft.com/microsoft-365/compliance/data-loss-prevention-policies#incident-reports).</span><span class="sxs-lookup"><span data-stu-id="e9884-120">See specific details of the event with an [Incident Report](https://docs.microsoft.com/microsoft-365/compliance/data-loss-prevention-policies#incident-reports).</span></span>
