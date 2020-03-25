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
ms.openlocfilehash: a56e18ddadef3a2f9056978b8542c1dba8f29665
ms.sourcegitcommit: b0d5b68366028abcf08610672d5bc9d3b25ac433
ms.translationtype: MT
ms.contentlocale: bg-BG
ms.lasthandoff: 03/24/2020
ms.locfileid: "42932611"
---
# <a name="dlp-not-working-as-expected"></a><span data-ttu-id="1503a-102">DLP не работи според очакванията</span><span class="sxs-lookup"><span data-stu-id="1503a-102">DLP not working as expected</span></span>

<span data-ttu-id="1503a-103">**Важно:** много sharePoint Online и OneDrive клиенти работят критични бизнес приложения срещу услугата, която се изпълнява във фонов режим.</span><span class="sxs-lookup"><span data-stu-id="1503a-103">**Important**: Many SharePoint Online and OneDrive customers run business-critical applications against the service that run in the background.</span></span> <span data-ttu-id="1503a-104">Те включват миграция на съдържанието, предотвратяване на загуба на данни (DLP) и архивиране на решения.</span><span class="sxs-lookup"><span data-stu-id="1503a-104">These include content migration, Data Loss Prevention (DLP), and backup solutions.</span></span> <span data-ttu-id="1503a-105">По време на тези безпрецедентни времена ние предприемаме стъпки, за да гарантираме, че SharePoint Online и OneDrive услуги остават високо достъпни и надеждни за вашите потребители, които зависят от услугата повече от всякога в отдалечени работни сценарии.</span><span class="sxs-lookup"><span data-stu-id="1503a-105">During these unprecedented times, we are taking steps to ensure that SharePoint Online and OneDrive services remain highly available and reliable for your users who depend on the service more than ever in remote work scenarios.</span></span>

<span data-ttu-id="1503a-106">В подкрепа на тази цел, ние сме внедрили по-строги ограничения за ограничаване на приложенията за фон (миграция, DLP и архивиране на решения) през делничните дни.</span><span class="sxs-lookup"><span data-stu-id="1503a-106">In support of this objective, we have implemented tighter throttling limits on background apps (migration, DLP and backup solutions) during weekday daytime hours.</span></span> <span data-ttu-id="1503a-107">Трябва да очаквате, че тези приложения ще постигнат много ограничена пропускателна информация по време на тези времена.</span><span class="sxs-lookup"><span data-stu-id="1503a-107">You should expect that these apps will achieve very limited throughput during these times.</span></span> <span data-ttu-id="1503a-108">Въпреки това, по време на вечерните и почивните часове за региона, услугата ще бъде готова да обработи значително по-голям обем заявки от приложения за фон.</span><span class="sxs-lookup"><span data-stu-id="1503a-108">However, during evening and weekend hours for the region, the service will be ready to process a significantly higher volume of requests from background apps.</span></span>

 <span data-ttu-id="1503a-109">**Настройване на DLP**</span><span class="sxs-lookup"><span data-stu-id="1503a-109">**Setting up DLP**</span></span>

<span data-ttu-id="1503a-110">Имате проблеми с **предотвратяване на загуба на данни (DLP)** в Office 365 не работи според очакванията?</span><span class="sxs-lookup"><span data-stu-id="1503a-110">Are you having problems with **Data Loss Prevention (DLP)** in Office 365 not working as expected?</span></span> <span data-ttu-id="1503a-111">Ако е така, уверете се, че **вашите DLP правила** е настроен правилно и че вашите данни съдържа това, което се търси **dlp правила,** когато се оценява.</span><span class="sxs-lookup"><span data-stu-id="1503a-111">If so, make sure that your **DLP policy** is set up correctly, and that your data contains what the **DLP policy** is looking for when it is being evaluated.</span></span>
  
<span data-ttu-id="1503a-112">DLP правилата ви позволяват да идентифицирате и защитавате поверителна информация във вашата организация.</span><span class="sxs-lookup"><span data-stu-id="1503a-112">DLP policies allows you to identify and protect sensitive information in your organization.</span></span> <span data-ttu-id="1503a-113">За да настроите DLP правила, използвайте информацията [тук](https://docs.microsoft.com/office365/securitycompliance/prevent-data-loss#set-up-dlp).</span><span class="sxs-lookup"><span data-stu-id="1503a-113">To setup DLP policies, use the information [here](https://docs.microsoft.com/office365/securitycompliance/prevent-data-loss#set-up-dlp).</span></span>
  
 <span data-ttu-id="1503a-114">**Какви dlp политики търсят**</span><span class="sxs-lookup"><span data-stu-id="1503a-114">**What DLP policies look for**</span></span>
  
<span data-ttu-id="1503a-115">Когато използвате **вградените поверителни типове информация** в центъра за защита и съответствие на Office 365, DLP правила търсят конкретни модели и елементи при откриване на тези типове.</span><span class="sxs-lookup"><span data-stu-id="1503a-115">When using the **built-in sensitive information types** in Office 365 Security and Compliance center, DLP policies look for specific patterns and elements when detecting these sensitive types.</span></span>
  
- <span data-ttu-id="1503a-116">**Вградени типове поверителна информация**</span><span class="sxs-lookup"><span data-stu-id="1503a-116">**Built-in Sensitive Information Types**</span></span>

    <span data-ttu-id="1503a-117">За информация относно вградените типове чувствителни и какво търси правилото на DLP при откриване на типа "Чувствителен", вижте: [Какво търсят типовете поверителна информация за](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for).</span><span class="sxs-lookup"><span data-stu-id="1503a-117">For information on the built-in Sensitive types and what a DLP policy looks for when detecting the Sensitive type, see: [What the sensitive information types look for](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for).</span></span>

- <span data-ttu-id="1503a-118">**Типове поверителни по избор информация**</span><span class="sxs-lookup"><span data-stu-id="1503a-118">**Custom Sensitive Information Types**</span></span>

    <span data-ttu-id="1503a-119">Ако се опитвате да създадете потребителски поверителни типове информация, използвайте следната статия за информация как да създадете персонализиран тип на поверителна [информация: Създаване на потребителски поверителен тип информация](https://docs.microsoft.com/office365/securitycompliance/create-a-custom-sensitive-information-type).</span><span class="sxs-lookup"><span data-stu-id="1503a-119">If you are trying to create custom sensitive information types, use the following article for information on how to create a custom sensitive type: [Create a custom sensitive information type](https://docs.microsoft.com/office365/securitycompliance/create-a-custom-sensitive-information-type).</span></span>

<span data-ttu-id="1503a-120">**Проверка на DLP правила**</span><span class="sxs-lookup"><span data-stu-id="1503a-120">**Test a DLP policy**</span></span>

<span data-ttu-id="1503a-121">За да тествате данните си с вграден или персонализиран тип информация, използвайте опцията **Тип тест** под **Класификация** > **Sensitive видове информация**.</span><span class="sxs-lookup"><span data-stu-id="1503a-121">To test your data with a built-in or custom sensitive information type, use the **Test type** option under **Classifications** > **Sensitive info types**.</span></span> <span data-ttu-id="1503a-122">За повече информация вижте [Тестване на персонализирани типове информация за поверителни информация](https://docs.microsoft.com/office365/securitycompliance/create-a-custom-sensitive-information-type#test-custom-sensitive-information-types-in-the-security--compliance-center).</span><span class="sxs-lookup"><span data-stu-id="1503a-122">For more information, see [Test custom sensitive information types](https://docs.microsoft.com/office365/securitycompliance/create-a-custom-sensitive-information-type#test-custom-sensitive-information-types-in-the-security--compliance-center).</span></span>

 <span data-ttu-id="1503a-123">**Доклади**</span><span class="sxs-lookup"><span data-stu-id="1503a-123">**Reports**</span></span>
  
- <span data-ttu-id="1503a-124">Получете аналитични данни за конфиденциални данни с [DLP отчети.](https://docs.microsoft.com/office365/securitycompliance/data-loss-prevention-policies#dlp-reports)</span><span class="sxs-lookup"><span data-stu-id="1503a-124">Get sensitive data insights with [DLP Reports.](https://docs.microsoft.com/office365/securitycompliance/data-loss-prevention-policies#dlp-reports)</span></span>

- <span data-ttu-id="1503a-125">Вижте конкретни подробности за събитието с [доклад за инцидент .](https://docs.microsoft.com/office365/securitycompliance/data-loss-prevention-policies#incident-reports)</span><span class="sxs-lookup"><span data-stu-id="1503a-125">See specific details of the event with an [Incident Report](https://docs.microsoft.com/office365/securitycompliance/data-loss-prevention-policies#incident-reports).</span></span>
