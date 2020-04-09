---
title: DLP не работи според очакванията
ms.author: deniseb
author: denisebmsft
manager: laurawi
ms.date: 1/9/2019
ms.audience: ITPro
ms.topic: article
ms.prod: office-online-server
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1241"
- "3200001"
ms.assetid: f6fcf5ad-55a1-4f25-af27-1f7c1ce06409
ms.openlocfilehash: 574a8a43d8264e98c6af2bfeb1bb472475e6e334
ms.sourcegitcommit: 940169c0edf638b5086d70cc275049f01dcff3cf
ms.translationtype: MT
ms.contentlocale: bg-BG
ms.lasthandoff: 04/08/2020
ms.locfileid: "42977427"
---
# <a name="dlp-not-working-as-expected"></a><span data-ttu-id="378be-102">DLP не работи според очакванията</span><span class="sxs-lookup"><span data-stu-id="378be-102">DLP not working as expected</span></span>

<span data-ttu-id="378be-103">**Важно**: през тези безпрецедентни времена ние предприемаме стъпки, за да гарантираме, че услугите на SharePoint Online и OneDrive остават на пълно разположение – за повече информация посетете [Временни корекции на функции на SharePoint Online](https://aka.ms/ODSPAdjustments).</span><span class="sxs-lookup"><span data-stu-id="378be-103">**Important**: During these unprecedented times, we are taking steps to ensure that SharePoint Online and OneDrive services remain highly available – Please visit [SharePoint Online Temporary Feature Adjustments](https://aka.ms/ODSPAdjustments) for more information.</span></span>

 <span data-ttu-id="378be-104">**Настройване на DLP**</span><span class="sxs-lookup"><span data-stu-id="378be-104">**Setting up DLP**</span></span>

<span data-ttu-id="378be-105">Имате проблеми с **предотвратяване на загуба на данни (DLP)** в Office 365 не работи според очакванията?</span><span class="sxs-lookup"><span data-stu-id="378be-105">Are you having problems with **Data Loss Prevention (DLP)** in Office 365 not working as expected?</span></span> <span data-ttu-id="378be-106">Ако е така, уверете се, че **вашите DLP правила** е настроен правилно и че вашите данни съдържа това, което се търси **dlp правила,** когато се оценява.</span><span class="sxs-lookup"><span data-stu-id="378be-106">If so, make sure that your **DLP policy** is set up correctly, and that your data contains what the **DLP policy** is looking for when it is being evaluated.</span></span>
  
<span data-ttu-id="378be-107">DLP правилата ви позволяват да идентифицирате и защитавате поверителна информация във вашата организация.</span><span class="sxs-lookup"><span data-stu-id="378be-107">DLP policies allows you to identify and protect sensitive information in your organization.</span></span> <span data-ttu-id="378be-108">За да настроите DLP правила, използвайте информацията [тук](https://docs.microsoft.com/office365/securitycompliance/prevent-data-loss#set-up-dlp).</span><span class="sxs-lookup"><span data-stu-id="378be-108">To setup DLP policies, use the information [here](https://docs.microsoft.com/office365/securitycompliance/prevent-data-loss#set-up-dlp).</span></span>
  
 <span data-ttu-id="378be-109">**Какви dlp политики търсят**</span><span class="sxs-lookup"><span data-stu-id="378be-109">**What DLP policies look for**</span></span>
  
<span data-ttu-id="378be-110">Когато използвате **вградените поверителни типове информация** в центъра за защита и съответствие на Office 365, DLP правила търсят конкретни модели и елементи при откриване на тези типове.</span><span class="sxs-lookup"><span data-stu-id="378be-110">When using the **built-in sensitive information types** in Office 365 Security and Compliance center, DLP policies look for specific patterns and elements when detecting these sensitive types.</span></span>
  
- <span data-ttu-id="378be-111">**Вградени типове поверителна информация**</span><span class="sxs-lookup"><span data-stu-id="378be-111">**Built-in Sensitive Information Types**</span></span>

    <span data-ttu-id="378be-112">За информация относно вградените типове чувствителни и какво търси правилото на DLP при откриване на типа "Чувствителен", вижте: [Какво търсят типовете поверителна информация за](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for).</span><span class="sxs-lookup"><span data-stu-id="378be-112">For information on the built-in Sensitive types and what a DLP policy looks for when detecting the Sensitive type, see: [What the sensitive information types look for](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for).</span></span>

- <span data-ttu-id="378be-113">**Типове поверителни по избор информация**</span><span class="sxs-lookup"><span data-stu-id="378be-113">**Custom Sensitive Information Types**</span></span>

    <span data-ttu-id="378be-114">Ако се опитвате да създадете потребителски поверителни типове информация, използвайте следната статия за информация как да създадете персонализиран тип на поверителна [информация: Създаване на потребителски поверителен тип информация](https://docs.microsoft.com/office365/securitycompliance/create-a-custom-sensitive-information-type).</span><span class="sxs-lookup"><span data-stu-id="378be-114">If you are trying to create custom sensitive information types, use the following article for information on how to create a custom sensitive type: [Create a custom sensitive information type](https://docs.microsoft.com/office365/securitycompliance/create-a-custom-sensitive-information-type).</span></span>

<span data-ttu-id="378be-115">**Проверка на DLP правила**</span><span class="sxs-lookup"><span data-stu-id="378be-115">**Test a DLP policy**</span></span>

<span data-ttu-id="378be-116">За да тествате данните си с вграден или персонализиран тип информация, използвайте опцията **Тип тест** под **Класификация** > **Sensitive видове информация**.</span><span class="sxs-lookup"><span data-stu-id="378be-116">To test your data with a built-in or custom sensitive information type, use the **Test type** option under **Classifications** > **Sensitive info types**.</span></span> <span data-ttu-id="378be-117">За повече информация вижте [Тестване на персонализирани типове информация за поверителни информация](https://docs.microsoft.com/office365/securitycompliance/create-a-custom-sensitive-information-type#test-custom-sensitive-information-types-in-the-security--compliance-center).</span><span class="sxs-lookup"><span data-stu-id="378be-117">For more information, see [Test custom sensitive information types](https://docs.microsoft.com/office365/securitycompliance/create-a-custom-sensitive-information-type#test-custom-sensitive-information-types-in-the-security--compliance-center).</span></span>

 <span data-ttu-id="378be-118">**Доклади**</span><span class="sxs-lookup"><span data-stu-id="378be-118">**Reports**</span></span>
  
- <span data-ttu-id="378be-119">Получете аналитични данни за конфиденциални данни с [DLP отчети.](https://docs.microsoft.com/office365/securitycompliance/data-loss-prevention-policies#dlp-reports)</span><span class="sxs-lookup"><span data-stu-id="378be-119">Get sensitive data insights with [DLP Reports.](https://docs.microsoft.com/office365/securitycompliance/data-loss-prevention-policies#dlp-reports)</span></span>

- <span data-ttu-id="378be-120">Вижте конкретни подробности за събитието с [доклад за инцидент .](https://docs.microsoft.com/office365/securitycompliance/data-loss-prevention-policies#incident-reports)</span><span class="sxs-lookup"><span data-stu-id="378be-120">See specific details of the event with an [Incident Report](https://docs.microsoft.com/office365/securitycompliance/data-loss-prevention-policies#incident-reports).</span></span>
