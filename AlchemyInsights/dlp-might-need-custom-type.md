---
title: Може да се нуждаете от персонализиран тип DLP
ms.author: pebaum
author: pebaum
manager: laurawi
ms.date: ''
ms.audience: ITPro
ms.topic: article
ms.prod: office-online-server
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1647"
- "3200001"
ms.assetid: ''
ms.openlocfilehash: 890bba57bc36c034c507e6124cd6593ef4d92af8
ms.sourcegitcommit: b0d5b68366028abcf08610672d5bc9d3b25ac433
ms.translationtype: MT
ms.contentlocale: bg-BG
ms.lasthandoff: 03/24/2020
ms.locfileid: "42932647"
---
# <a name="dlp-might-need-a-custom-type"></a><span data-ttu-id="4cb9b-102">Може да се нуждаете от персонализиран тип DLP</span><span class="sxs-lookup"><span data-stu-id="4cb9b-102">DLP might need a custom type</span></span>

<span data-ttu-id="4cb9b-103">**Важно:** много sharePoint Online и OneDrive клиенти работят критични бизнес приложения срещу услугата, която се изпълнява във фонов режим.</span><span class="sxs-lookup"><span data-stu-id="4cb9b-103">**Important**: Many SharePoint Online and OneDrive customers run business-critical applications against the service that run in the background.</span></span> <span data-ttu-id="4cb9b-104">Те включват миграция на съдържанието, предотвратяване на загуба на данни (DLP) и архивиране на решения.</span><span class="sxs-lookup"><span data-stu-id="4cb9b-104">These include content migration, Data Loss Prevention (DLP), and backup solutions.</span></span> <span data-ttu-id="4cb9b-105">По време на тези безпрецедентни времена ние предприемаме стъпки, за да гарантираме, че SharePoint Online и OneDrive услуги остават високо достъпни и надеждни за вашите потребители, които зависят от услугата повече от всякога в отдалечени работни сценарии.</span><span class="sxs-lookup"><span data-stu-id="4cb9b-105">During these unprecedented times, we are taking steps to ensure that SharePoint Online and OneDrive services remain highly available and reliable for your users who depend on the service more than ever in remote work scenarios.</span></span>

<span data-ttu-id="4cb9b-106">В подкрепа на тази цел, ние сме внедрили по-строги ограничения за ограничаване на приложенията за фон (миграция, DLP и архивиране на решения) през делничните дни.</span><span class="sxs-lookup"><span data-stu-id="4cb9b-106">In support of this objective, we have implemented tighter throttling limits on background apps (migration, DLP and backup solutions) during weekday daytime hours.</span></span> <span data-ttu-id="4cb9b-107">Трябва да очаквате, че тези приложения ще постигнат много ограничена пропускателна информация по време на тези времена.</span><span class="sxs-lookup"><span data-stu-id="4cb9b-107">You should expect that these apps will achieve very limited throughput during these times.</span></span> <span data-ttu-id="4cb9b-108">Въпреки това, по време на вечерните и почивните часове за региона, услугата ще бъде готова да обработи значително по-голям обем заявки от приложения за фон.</span><span class="sxs-lookup"><span data-stu-id="4cb9b-108">However, during evening and weekend hours for the region, the service will be ready to process a significantly higher volume of requests from background apps.</span></span>

<span data-ttu-id="4cb9b-109">**DLP може да изисква персонализиран тип информация**</span><span class="sxs-lookup"><span data-stu-id="4cb9b-109">**DLP may require a custom information type**</span></span>

<span data-ttu-id="4cb9b-110">С правилата за предотвратяване на загуба на данни (DLP) можете да идентифицирате и защитавате конфиденциални данни във вашата организация.</span><span class="sxs-lookup"><span data-stu-id="4cb9b-110">With a data loss prevention (DLP) policy, you can identify and protect sensitive data in your organization.</span></span> <span data-ttu-id="4cb9b-111">В някои случаи може да се наложи да създадете свой **собствен персонализиран** тип информация, за да защитите данните на вашата организация.</span><span class="sxs-lookup"><span data-stu-id="4cb9b-111">In some scenarios, you might need to create your own **custom** sensitive information type to protect your organization's data.</span></span>

<span data-ttu-id="4cb9b-112">Например, вашата организация може да се наложи да идентифицира и защитава идентификационните данни на служителите или други данни в определен формат, специфичен за вашата организация. Ако е така, вижте следните статии за повече информация.</span><span class="sxs-lookup"><span data-stu-id="4cb9b-112">For example, your organization might need to identify and protect employee IDs or other data in some format specific to your org. If so, see the following articles for more information.</span></span>
  
 <span data-ttu-id="4cb9b-113">**Персонализиране на вграден тип поверителна информация**</span><span class="sxs-lookup"><span data-stu-id="4cb9b-113">**Customize a built-in sensitive information type**</span></span>
  
<span data-ttu-id="4cb9b-114">Ако вграден тип поверителна информация ще отговаря на вашите нужди само с няколко ощипвания, можете да [персонализирате вграден тип на поверителна информация.](https://docs.microsoft.com/office365/securitycompliance/customize-a-built-in-sensitive-information-type)</span><span class="sxs-lookup"><span data-stu-id="4cb9b-114">If a built-in sensitive information type would meet your needs with just a few tweaks, you can [customize a built-in sensitive information type](https://docs.microsoft.com/office365/securitycompliance/customize-a-built-in-sensitive-information-type).</span></span> <span data-ttu-id="4cb9b-115">Можете например да добавяте или премахвате ключови думи, или да добавяте или премахвате подкрепящи доказателства, като например дата или адрес.</span><span class="sxs-lookup"><span data-stu-id="4cb9b-115">For example, you can add or remove keywords, or add or remove supporting evidence such as a date or address.</span></span>
  
 <span data-ttu-id="4cb9b-116">**Създаване на персонализиран тип информация за поверителна информация**</span><span class="sxs-lookup"><span data-stu-id="4cb9b-116">**Create a custom sensitive information type**</span></span>
  
<span data-ttu-id="4cb9b-117">Но ако трябва да идентифицирате и защитите напълно различен тип поверителна информация, можете да [създадете персонализиран тип поверителна информация](https://docs.microsoft.com/office365/securitycompliance/create-a-custom-sensitive-information-type) в потребителския интерфейс на центъра за съответствие на & за сигурност.</span><span class="sxs-lookup"><span data-stu-id="4cb9b-117">But if you need to identify and protect a different type of sensitive information altogether, you can [create a custom sensitive information type](https://docs.microsoft.com/office365/securitycompliance/create-a-custom-sensitive-information-type) in the UI of the Security & Compliance Center.</span></span>
  
<span data-ttu-id="4cb9b-118">**Създаване на потребителски поверителна информация тип в центъра за сигурност & PowerShell**</span><span class="sxs-lookup"><span data-stu-id="4cb9b-118">**Create a custom sensitive information type in Security & Compliance Center PowerShell**</span></span>

<span data-ttu-id="4cb9b-119">И накрая, ако потребителският интерфейс не предоставя всички необходими опции, можете да [създадете персонализиран тип поверителна информация в Security & Съответствие то powerShell](https://docs.microsoft.com/office365/securitycompliance/create-a-custom-sensitive-information-type-in-scc-powershell).</span><span class="sxs-lookup"><span data-stu-id="4cb9b-119">Finally, if the UI doesn't provide all the options you need, you can [create a custom sensitive information type in Security & Compliance Center PowerShell](https://docs.microsoft.com/office365/securitycompliance/create-a-custom-sensitive-information-type-in-scc-powershell).</span></span> <span data-ttu-id="4cb9b-120">Като започнете с XML файл, можете да използвате всяка налична опция.</span><span class="sxs-lookup"><span data-stu-id="4cb9b-120">By starting with an XML file, you can use every option available.</span></span>
