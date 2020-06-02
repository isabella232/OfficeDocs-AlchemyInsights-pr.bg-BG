---
title: DLP не работи според очакванията
ms.author: deniseb
author: denisebmsft
manager: laurawi
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.prod: office-online-server
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1241"
- "3200001"
ms.assetid: f6fcf5ad-55a1-4f25-af27-1f7c1ce06409
ms.openlocfilehash: e96904e2f0da2fe1fafb3f8722465eaf22681b71
ms.sourcegitcommit: bc7d6f4f3c9f7060d073f5130e1ec856e248d020
ms.translationtype: MT
ms.contentlocale: bg-BG
ms.lasthandoff: 06/02/2020
ms.locfileid: "44507467"
---
# <a name="dlp-not-working-as-expected"></a><span data-ttu-id="50d34-102">DLP не работи според очакванията</span><span class="sxs-lookup"><span data-stu-id="50d34-102">DLP not working as expected</span></span>

<span data-ttu-id="50d34-103">**Важно**: през тези безпрецедентни времена ние предприемаме стъпки, за да гарантираме, че услугите на SharePoint Online и OneDrive остават на пълно разположение – за повече информация посетете [Временни корекции на функции на SharePoint Online](https://aka.ms/ODSPAdjustments).</span><span class="sxs-lookup"><span data-stu-id="50d34-103">**Important**: During these unprecedented times, we are taking steps to ensure that SharePoint Online and OneDrive services remain highly available – Please visit [SharePoint Online Temporary Feature Adjustments](https://aka.ms/ODSPAdjustments) for more information.</span></span>

 <span data-ttu-id="50d34-104">**Настройване на DLP**</span><span class="sxs-lookup"><span data-stu-id="50d34-104">**Setting up DLP**</span></span>

<span data-ttu-id="50d34-105">Имате проблеми с **предотвратяване на загуба на данни (DLP)** в Office 365 не работи според очакванията?</span><span class="sxs-lookup"><span data-stu-id="50d34-105">Are you having problems with **Data Loss Prevention (DLP)** in Office 365 not working as expected?</span></span> <span data-ttu-id="50d34-106">Ако е така, уверете се, че вашата **DLP правила** е настроен правилно и че данните ви съдържа какво се търси **DLP политика,** когато се оценява.</span><span class="sxs-lookup"><span data-stu-id="50d34-106">If so, make sure that your **DLP policy** is set up correctly, and that your data contains what the **DLP policy** is looking for when it is being evaluated.</span></span>
  
<span data-ttu-id="50d34-107">Правилата на DLP ви позволяват да идентифицирате и защитавате поверителна информация във вашата организация.</span><span class="sxs-lookup"><span data-stu-id="50d34-107">DLP policies allows you to identify and protect sensitive information in your organization.</span></span> <span data-ttu-id="50d34-108">За да настроите DLP правила, използвайте информацията [тук](https://docs.microsoft.com/office365/securitycompliance/prevent-data-loss#set-up-dlp).</span><span class="sxs-lookup"><span data-stu-id="50d34-108">To setup DLP policies, use the information [here](https://docs.microsoft.com/office365/securitycompliance/prevent-data-loss#set-up-dlp).</span></span>
  
 <span data-ttu-id="50d34-109">**Какви правила за DLP се търсят**</span><span class="sxs-lookup"><span data-stu-id="50d34-109">**What DLP policies look for**</span></span>
  
<span data-ttu-id="50d34-110">Когато използвате **вградените типове поверителна информация в** центровете за защита и съответствие, правилата на DLP търсят конкретни модели и елементи при откриване на тези чувствителни типове.</span><span class="sxs-lookup"><span data-stu-id="50d34-110">When using the **built-in sensitive information types** in the Security and Compliance centers, DLP policies look for specific patterns and elements when detecting these sensitive types.</span></span>
  
- <span data-ttu-id="50d34-111">**Вградени типове поверителна информация**</span><span class="sxs-lookup"><span data-stu-id="50d34-111">**Built-in Sensitive Information Types**</span></span>

    <span data-ttu-id="50d34-112">За информация относно вградените чувствителни типове и какво търси DLP политиката при откриване на типа Sensitive вижте: [Какви типове чувствителна информация изглежда.](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions)</span><span class="sxs-lookup"><span data-stu-id="50d34-112">For information on the built-in Sensitive types and what a DLP policy looks for when detecting the Sensitive type, see: [What the sensitive information types look for](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions).</span></span>

- <span data-ttu-id="50d34-113">**Потребителски типове информация за конфиденциални**</span><span class="sxs-lookup"><span data-stu-id="50d34-113">**Custom Sensitive Information Types**</span></span>

    <span data-ttu-id="50d34-114">Ако се опитвате да създадете потребителски типове информация, използвайте следната статия за информация как да създадете потребителски чувствителен тип: [Създаване на потребителски чувствителен тип информация](https://docs.microsoft.com/microsoft-365/compliance/create-a-custom-sensitive-information-type)тип .</span><span class="sxs-lookup"><span data-stu-id="50d34-114">If you are trying to create custom sensitive information types, use the following article for information on how to create a custom sensitive type: [Create a custom sensitive information type](https://docs.microsoft.com/microsoft-365/compliance/create-a-custom-sensitive-information-type).</span></span>

<span data-ttu-id="50d34-115">**Тествайте DLP политика**</span><span class="sxs-lookup"><span data-stu-id="50d34-115">**Test a DLP policy**</span></span>

<span data-ttu-id="50d34-116">За да тествате данните си с вграден или персонализиран тип информация, използвайте опцията **Тип тест** под **Класификации**  >  **Поверителна информация типове**.</span><span class="sxs-lookup"><span data-stu-id="50d34-116">To test your data with a built-in or custom sensitive information type, use the **Test type** option under **Classifications** > **Sensitive info types**.</span></span> <span data-ttu-id="50d34-117">За повече информация вижте [Тестване на типовете потребителска поверителна информация](https://docs.microsoft.com/microsoft-365/compliance/create-a-custom-sensitive-information-type#create-custom-sensitive-information-types-in-the-security--compliance-center).</span><span class="sxs-lookup"><span data-stu-id="50d34-117">For more information, see [Test custom sensitive information types](https://docs.microsoft.com/microsoft-365/compliance/create-a-custom-sensitive-information-type#create-custom-sensitive-information-types-in-the-security--compliance-center).</span></span>

 <span data-ttu-id="50d34-118">**Доклади**</span><span class="sxs-lookup"><span data-stu-id="50d34-118">**Reports**</span></span>
  
- <span data-ttu-id="50d34-119">Получаване на поверителни данни за данни с [отчетите за DLP.](https://docs.microsoft.com/microsoft-365/compliance/data-loss-prevention-policies#dlp-reports)</span><span class="sxs-lookup"><span data-stu-id="50d34-119">Get sensitive data insights with [DLP Reports.](https://docs.microsoft.com/microsoft-365/compliance/data-loss-prevention-policies#dlp-reports)</span></span>

- <span data-ttu-id="50d34-120">Вижте конкретни подробности за събитието с [доклад за инцидент](https://docs.microsoft.com/microsoft-365/compliance/data-loss-prevention-policies#incident-reports).</span><span class="sxs-lookup"><span data-stu-id="50d34-120">See specific details of the event with an [Incident Report](https://docs.microsoft.com/microsoft-365/compliance/data-loss-prevention-policies#incident-reports).</span></span>
