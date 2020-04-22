---
title: Може да се нуждаете от персонализиран тип DLP
ms.author: pebaum
author: pebaum
manager: laurawi
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.prod: office-online-server
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1647"
- "3200001"
ms.assetid: ''
ms.openlocfilehash: b83bb77383e2ae7e78c31f35c972182c54487c60
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: bg-BG
ms.lasthandoff: 04/22/2020
ms.locfileid: "43704478"
---
# <a name="dlp-might-need-a-custom-type"></a><span data-ttu-id="89072-102">Може да се нуждаете от персонализиран тип DLP</span><span class="sxs-lookup"><span data-stu-id="89072-102">DLP might need a custom type</span></span>

<span data-ttu-id="89072-103">**Важно**: през тези безпрецедентни времена ние предприемаме стъпки, за да гарантираме, че услугите на SharePoint Online и OneDrive остават на пълно разположение – за повече информация посетете [Временни корекции на функции на SharePoint Online](https://aka.ms/ODSPAdjustments).</span><span class="sxs-lookup"><span data-stu-id="89072-103">**Important**: During these unprecedented times, we are taking steps to ensure that SharePoint Online and OneDrive services remain highly available – Please visit [SharePoint Online Temporary Feature Adjustments](https://aka.ms/ODSPAdjustments) for more information.</span></span>

<span data-ttu-id="89072-104">**DLP може да изисква персонализиран тип информация**</span><span class="sxs-lookup"><span data-stu-id="89072-104">**DLP may require a custom information type**</span></span>

<span data-ttu-id="89072-105">С правилата за предотвратяване на загуба на данни (DLP) можете да идентифицирате и защитавате конфиденциални данни във вашата организация.</span><span class="sxs-lookup"><span data-stu-id="89072-105">With a data loss prevention (DLP) policy, you can identify and protect sensitive data in your organization.</span></span> <span data-ttu-id="89072-106">В някои случаи може да се наложи да създадете свой **собствен персонализиран** тип информация, за да защитите данните на вашата организация.</span><span class="sxs-lookup"><span data-stu-id="89072-106">In some scenarios, you might need to create your own **custom** sensitive information type to protect your organization's data.</span></span>

<span data-ttu-id="89072-107">Например, вашата организация може да се наложи да идентифицира и защитава идентификационните данни на служителите или други данни в определен формат, специфичен за вашата организация. Ако е така, вижте следните статии за повече информация.</span><span class="sxs-lookup"><span data-stu-id="89072-107">For example, your organization might need to identify and protect employee IDs or other data in some format specific to your org. If so, see the following articles for more information.</span></span>
  
 <span data-ttu-id="89072-108">**Персонализиране на вграден тип поверителна информация**</span><span class="sxs-lookup"><span data-stu-id="89072-108">**Customize a built-in sensitive information type**</span></span>
  
<span data-ttu-id="89072-109">Ако вграден тип поверителна информация ще отговаря на вашите нужди само с няколко ощипвания, можете да [персонализирате вграден тип на поверителна информация.](https://docs.microsoft.com/office365/securitycompliance/customize-a-built-in-sensitive-information-type)</span><span class="sxs-lookup"><span data-stu-id="89072-109">If a built-in sensitive information type would meet your needs with just a few tweaks, you can [customize a built-in sensitive information type](https://docs.microsoft.com/office365/securitycompliance/customize-a-built-in-sensitive-information-type).</span></span> <span data-ttu-id="89072-110">Можете например да добавяте или премахвате ключови думи, или да добавяте или премахвате подкрепящи доказателства, като например дата или адрес.</span><span class="sxs-lookup"><span data-stu-id="89072-110">For example, you can add or remove keywords, or add or remove supporting evidence such as a date or address.</span></span>
  
 <span data-ttu-id="89072-111">**Създаване на персонализиран тип информация за поверителна информация**</span><span class="sxs-lookup"><span data-stu-id="89072-111">**Create a custom sensitive information type**</span></span>
  
<span data-ttu-id="89072-112">Но ако трябва да идентифицирате и защитите напълно различен тип поверителна информация, можете да [създадете персонализиран тип поверителна информация](https://docs.microsoft.com/office365/securitycompliance/create-a-custom-sensitive-information-type) в потребителския интерфейс на центъра за съответствие на & за сигурност.</span><span class="sxs-lookup"><span data-stu-id="89072-112">But if you need to identify and protect a different type of sensitive information altogether, you can [create a custom sensitive information type](https://docs.microsoft.com/office365/securitycompliance/create-a-custom-sensitive-information-type) in the UI of the Security & Compliance Center.</span></span>
  
<span data-ttu-id="89072-113">**Създаване на потребителски поверителна информация тип в центъра за сигурност & PowerShell**</span><span class="sxs-lookup"><span data-stu-id="89072-113">**Create a custom sensitive information type in Security & Compliance Center PowerShell**</span></span>

<span data-ttu-id="89072-114">И накрая, ако потребителският интерфейс не предоставя всички необходими опции, можете да [създадете персонализиран тип поверителна информация в Security & Съответствие то powerShell](https://docs.microsoft.com/office365/securitycompliance/create-a-custom-sensitive-information-type-in-scc-powershell).</span><span class="sxs-lookup"><span data-stu-id="89072-114">Finally, if the UI doesn't provide all the options you need, you can [create a custom sensitive information type in Security & Compliance Center PowerShell](https://docs.microsoft.com/office365/securitycompliance/create-a-custom-sensitive-information-type-in-scc-powershell).</span></span> <span data-ttu-id="89072-115">Като започнете с XML файл, можете да използвате всяка налична опция.</span><span class="sxs-lookup"><span data-stu-id="89072-115">By starting with an XML file, you can use every option available.</span></span>
