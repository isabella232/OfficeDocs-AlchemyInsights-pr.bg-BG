---
title: DLP може да се нуждае от персонализиран тип
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
ms.openlocfilehash: 1ec8959a479f1a8f7bfcffb55f440e8c4ab435fb
ms.sourcegitcommit: bc7d6f4f3c9f7060d073f5130e1ec856e248d020
ms.translationtype: MT
ms.contentlocale: bg-BG
ms.lasthandoff: 06/02/2020
ms.locfileid: "44507503"
---
# <a name="dlp-might-need-a-custom-type"></a><span data-ttu-id="f99f4-102">DLP може да се нуждае от персонализиран тип</span><span class="sxs-lookup"><span data-stu-id="f99f4-102">DLP might need a custom type</span></span>

<span data-ttu-id="f99f4-103">**Важно**: през тези безпрецедентни времена ние предприемаме стъпки, за да гарантираме, че услугите на SharePoint Online и OneDrive остават на пълно разположение – за повече информация посетете [Временни корекции на функции на SharePoint Online](https://aka.ms/ODSPAdjustments).</span><span class="sxs-lookup"><span data-stu-id="f99f4-103">**Important**: During these unprecedented times, we are taking steps to ensure that SharePoint Online and OneDrive services remain highly available – Please visit [SharePoint Online Temporary Feature Adjustments](https://aka.ms/ODSPAdjustments) for more information.</span></span>

<span data-ttu-id="f99f4-104">**DLP може да изисква тип потребителска информация**</span><span class="sxs-lookup"><span data-stu-id="f99f4-104">**DLP may require a custom information type**</span></span>

<span data-ttu-id="f99f4-105">С правилата за защита от загуба на данни (DLP) можете да идентифицирате и защитавате поверителни данни във вашата организация.</span><span class="sxs-lookup"><span data-stu-id="f99f4-105">With a data loss prevention (DLP) policy, you can identify and protect sensitive data in your organization.</span></span> <span data-ttu-id="f99f4-106">В някои случаи може да се наложи да създадете **свой** собствен потребителски чувствителен тип информация, за да защитите данните на вашата организация.</span><span class="sxs-lookup"><span data-stu-id="f99f4-106">In some scenarios, you might need to create your own **custom** sensitive information type to protect your organization's data.</span></span>

<span data-ttu-id="f99f4-107">Например, вашата организация може да се наложи да идентифицира и защити ТА на служител или други данни в някакъв формат, който е специфичен за вашата организация. Ако е така, вижте следните статии за повече информация.</span><span class="sxs-lookup"><span data-stu-id="f99f4-107">For example, your organization might need to identify and protect employee IDs or other data in some format specific to your org. If so, see the following articles for more information.</span></span>
  
 <span data-ttu-id="f99f4-108">**Персонализиране на вграден тип поверителна информация**</span><span class="sxs-lookup"><span data-stu-id="f99f4-108">**Customize a built-in sensitive information type**</span></span>
  
<span data-ttu-id="f99f4-109">Ако вграден тип чувствителна информация ще отговори на вашите нужди само с няколко ощипвам, можете да [персонализирате вграден тип чувствителна информация](https://docs.microsoft.com/microsoft-365/compliance/customize-a-built-in-sensitive-information-type).</span><span class="sxs-lookup"><span data-stu-id="f99f4-109">If a built-in sensitive information type would meet your needs with just a few tweaks, you can [customize a built-in sensitive information type](https://docs.microsoft.com/microsoft-365/compliance/customize-a-built-in-sensitive-information-type).</span></span> <span data-ttu-id="f99f4-110">Можете например да добавяте или премахвате ключови думи или да добавяте или премахвате подкрепящи доказателства, като например дата или адрес.</span><span class="sxs-lookup"><span data-stu-id="f99f4-110">For example, you can add or remove keywords, or add or remove supporting evidence such as a date or address.</span></span>
  
 <span data-ttu-id="f99f4-111">**Създаване на потребителски тип информация за конфиденциални**</span><span class="sxs-lookup"><span data-stu-id="f99f4-111">**Create a custom sensitive information type**</span></span>
  
<span data-ttu-id="f99f4-112">Но ако трябва да идентифицирате и защитите напълно различен тип чувствителна информация, можете да [създадете потребителски тип поверителна информация](https://docs.microsoft.com/microsoft-365/compliance/create-a-custom-sensitive-information-type) в потребителския интерфейс на Центъра за защита & съответствие.</span><span class="sxs-lookup"><span data-stu-id="f99f4-112">But if you need to identify and protect a different type of sensitive information altogether, you can [create a custom sensitive information type](https://docs.microsoft.com/microsoft-365/compliance/create-a-custom-sensitive-information-type) in the UI of the Security & Compliance Center.</span></span>
  
<span data-ttu-id="f99f4-113">**Създаване на потребителски чувствителен тип информация в центъра за защита & съответствие Център PowerShell**</span><span class="sxs-lookup"><span data-stu-id="f99f4-113">**Create a custom sensitive information type in Security & Compliance Center PowerShell**</span></span>

<span data-ttu-id="f99f4-114">И накрая, ако потребителският интерфейс не предоставя всички опции, които ви трябват, можете да [създадете потребителски тип поверителна информация в Security & Център за съответствие PowerShell](https://docs.microsoft.com/microsoft-365/compliance/create-a-custom-sensitive-information-type-in-scc-powershell).</span><span class="sxs-lookup"><span data-stu-id="f99f4-114">Finally, if the UI doesn't provide all the options you need, you can [create a custom sensitive information type in Security & Compliance Center PowerShell](https://docs.microsoft.com/microsoft-365/compliance/create-a-custom-sensitive-information-type-in-scc-powershell).</span></span> <span data-ttu-id="f99f4-115">Като започнете с XML файл, можете да използвате всяка налична опция.</span><span class="sxs-lookup"><span data-stu-id="f99f4-115">By starting with an XML file, you can use every option available.</span></span>
