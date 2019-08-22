---
title: DLP, не работи както се очаква
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
ms.openlocfilehash: 102c8025571f840cf64091d75295acec50661df2
ms.sourcegitcommit: 1d98db8acb9959aba3b5e308a567ade6b62da56c
ms.translationtype: MT
ms.contentlocale: bg-BG
ms.lasthandoff: 08/22/2019
ms.locfileid: "36530268"
---
# <a name="dlp-not-working-as-expected"></a><span data-ttu-id="52a4e-102">DLP, не работи както се очаква</span><span class="sxs-lookup"><span data-stu-id="52a4e-102">DLP not working as expected</span></span>

<span data-ttu-id="52a4e-103">Имате ли проблеми с **Данни загуба предотвратяване (DLP)** в Office 365 не работи както се очаква?</span><span class="sxs-lookup"><span data-stu-id="52a4e-103">Are you having problems with **Data Loss Prevention (DLP)** in Office 365 not working as expected?</span></span> <span data-ttu-id="52a4e-104">Ако е така, уверете се, че вашата **DLP политика** е настроен правилно, и че вашите данни съдържат какви **DLP политика** се търси, когато тя се оценява.</span><span class="sxs-lookup"><span data-stu-id="52a4e-104">If so, make sure that your **DLP policy** is set up correctly, and that your data contains what the **DLP policy** is looking for when it is being evaluated.</span></span>
  
 <span data-ttu-id="52a4e-105">**Настройване на DLP**</span><span class="sxs-lookup"><span data-stu-id="52a4e-105">**Setting up DLP**</span></span>
  
<span data-ttu-id="52a4e-106">DLP политиките ви позволява да идентифицирате и защита на чувствителна информация във вашата организация.</span><span class="sxs-lookup"><span data-stu-id="52a4e-106">DLP policies allows you to identify and protect sensitive information in your organization.</span></span> <span data-ttu-id="52a4e-107">За настройка на DLP политиките, използвайте информацията [тук](https://docs.microsoft.com/office365/securitycompliance/prevent-data-loss#set-up-dlp).</span><span class="sxs-lookup"><span data-stu-id="52a4e-107">To setup DLP policies, use the information [here](https://docs.microsoft.com/office365/securitycompliance/prevent-data-loss#set-up-dlp).</span></span>
  
 <span data-ttu-id="52a4e-108">**Какво търси DLP политиките**</span><span class="sxs-lookup"><span data-stu-id="52a4e-108">**What DLP policies look for**</span></span>
  
<span data-ttu-id="52a4e-109">Когато използвате **вградени чувствителна информация типове** в Office 365 защита и съответствие център, DLP политиките търсите определени шарки и елементи при откриване на тези чувствителни видове.</span><span class="sxs-lookup"><span data-stu-id="52a4e-109">When using the **built-in sensitive information types** in Office 365 Security and Compliance center, DLP policies look for specific patterns and elements when detecting these sensitive types.</span></span>
  
- <span data-ttu-id="52a4e-110">**Типове вграден чувствителна информация**</span><span class="sxs-lookup"><span data-stu-id="52a4e-110">**Built-in Sensitive Information Types**</span></span>

    <span data-ttu-id="52a4e-111">За информация за вградени чувствителни типове и какво политика на DLP търси при откриване на чувствителни типа, вижте: [какви чувствителна информация търсят](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for).</span><span class="sxs-lookup"><span data-stu-id="52a4e-111">For information on the built-in Sensitive types and what a DLP policy looks for when detecting the Sensitive type, see: [What the sensitive information types look for](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for).</span></span>

- <span data-ttu-id="52a4e-112">**Типове потребителски чувствителна информация**</span><span class="sxs-lookup"><span data-stu-id="52a4e-112">**Custom Sensitive Information Types**</span></span>

    <span data-ttu-id="52a4e-113">Ако се опитвате да създадете типове потребителски чувствителна информация, използвайте следната статия за информация относно как да създадете персонализиран чувствителен тип: [Създаване на потребителски чувствителна информация тип](https://docs.microsoft.com/office365/securitycompliance/create-a-custom-sensitive-information-type).</span><span class="sxs-lookup"><span data-stu-id="52a4e-113">If you are trying to create custom sensitive information types, use the following article for information on how to create a custom sensitive type: [Create a custom sensitive information type](https://docs.microsoft.com/office365/securitycompliance/create-a-custom-sensitive-information-type).</span></span>

<span data-ttu-id="52a4e-114">**Тест на DLP политика**</span><span class="sxs-lookup"><span data-stu-id="52a4e-114">**Test a DLP policy**</span></span>

<span data-ttu-id="52a4e-115">За да тествате вашите данни с вградена или потребителска чувствителна информация тип, използвайте опцията **тест тип** под **класификации** > **типове чувствителна информация**.</span><span class="sxs-lookup"><span data-stu-id="52a4e-115">To test your data with a built-in or custom sensitive information type, use the **Test type** option under **Classifications** > **Sensitive info types**.</span></span> <span data-ttu-id="52a4e-116">За повече информация вижте [тест типове потребителски чувствителна информация](https://docs.microsoft.com/office365/securitycompliance/create-a-custom-sensitive-information-type#test-custom-sensitive-information-types-in-the-security--compliance-center).</span><span class="sxs-lookup"><span data-stu-id="52a4e-116">For more information, see [Test custom sensitive information types](https://docs.microsoft.com/office365/securitycompliance/create-a-custom-sensitive-information-type#test-custom-sensitive-information-types-in-the-security--compliance-center).</span></span>

 <span data-ttu-id="52a4e-117">**Доклади**</span><span class="sxs-lookup"><span data-stu-id="52a4e-117">**Reports**</span></span>
  
- <span data-ttu-id="52a4e-118">Вземи чувствителни данни прозрения с [DLP доклади.](https://docs.microsoft.com/office365/securitycompliance/data-loss-prevention-policies#dlp-reports)</span><span class="sxs-lookup"><span data-stu-id="52a4e-118">Get sensitive data insights with [DLP Reports.](https://docs.microsoft.com/office365/securitycompliance/data-loss-prevention-policies#dlp-reports)</span></span>

- <span data-ttu-id="52a4e-119">Вижте подробности за събитието [Инцидент доклад](https://docs.microsoft.com/office365/securitycompliance/data-loss-prevention-policies#incident-reports).</span><span class="sxs-lookup"><span data-stu-id="52a4e-119">See specific details of the event with an [Incident Report](https://docs.microsoft.com/office365/securitycompliance/data-loss-prevention-policies#incident-reports).</span></span>
