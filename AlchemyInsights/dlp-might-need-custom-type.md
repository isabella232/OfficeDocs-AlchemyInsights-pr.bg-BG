---
title: DLP може да се нуждае от тип по избор
ms.author: pebaum
author: pebaum
manager: laurawi
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1647"
- "3200001"
ms.assetid: ''
ms.openlocfilehash: 72b16d437f97de27cbdc364f022c3e2059b31ef0
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: bg-BG
ms.lasthandoff: 09/14/2020
ms.locfileid: "47712173"
---
# <a name="dlp-might-need-a-custom-type"></a><span data-ttu-id="fef11-102">DLP може да се нуждае от тип по избор</span><span class="sxs-lookup"><span data-stu-id="fef11-102">DLP might need a custom type</span></span>

<span data-ttu-id="fef11-103">**Важно**: през тези безпрецедентни времена ние предприемаме стъпки, за да гарантираме, че услугите на SharePoint Online и OneDrive остават на пълно разположение – за повече информация посетете [Временни корекции на функции на SharePoint Online](https://aka.ms/ODSPAdjustments).</span><span class="sxs-lookup"><span data-stu-id="fef11-103">**Important**: During these unprecedented times, we are taking steps to ensure that SharePoint Online and OneDrive services remain highly available – Please visit [SharePoint Online Temporary Feature Adjustments](https://aka.ms/ODSPAdjustments) for more information.</span></span>

<span data-ttu-id="fef11-104">**DLP може да изисква тип информация по избор**</span><span class="sxs-lookup"><span data-stu-id="fef11-104">**DLP may require a custom information type**</span></span>

<span data-ttu-id="fef11-105">Чрез правилата за защита от загуба на данни (DLP) можете да идентифицирате и защитавате поверителните данни във вашата организация.</span><span class="sxs-lookup"><span data-stu-id="fef11-105">With a data loss prevention (DLP) policy, you can identify and protect sensitive data in your organization.</span></span> <span data-ttu-id="fef11-106">В някои случаи може да се наложи да създадете свой собствен **персонализиран** тип информация, за да защитите данните на вашата организация.</span><span class="sxs-lookup"><span data-stu-id="fef11-106">In some scenarios, you might need to create your own **custom** sensitive information type to protect your organization's data.</span></span>

<span data-ttu-id="fef11-107">Например във вашата организация може да е необходимо да се идентифицират и защитават ИД на служител или други данни в някакъв формат, който е конкретен за организацията ви. Ако е така, вижте следните статии за повече информация.</span><span class="sxs-lookup"><span data-stu-id="fef11-107">For example, your organization might need to identify and protect employee IDs or other data in some format specific to your org. If so, see the following articles for more information.</span></span>
  
 <span data-ttu-id="fef11-108">**Персонализиране на вграден тип на поверителна информация**</span><span class="sxs-lookup"><span data-stu-id="fef11-108">**Customize a built-in sensitive information type**</span></span>
  
<span data-ttu-id="fef11-109">Ако вграден тип чувствителна информация би задоволил нуждите ви само с няколко ощипвам, можете да [персонализирате вграден тип на поверителна информация](https://docs.microsoft.com/microsoft-365/compliance/customize-a-built-in-sensitive-information-type).</span><span class="sxs-lookup"><span data-stu-id="fef11-109">If a built-in sensitive information type would meet your needs with just a few tweaks, you can [customize a built-in sensitive information type](https://docs.microsoft.com/microsoft-365/compliance/customize-a-built-in-sensitive-information-type).</span></span> <span data-ttu-id="fef11-110">Например можете да добавяте или премахвате ключови думи или да добавяте или премахвате доказателствени материали, например дата или адрес.</span><span class="sxs-lookup"><span data-stu-id="fef11-110">For example, you can add or remove keywords, or add or remove supporting evidence such as a date or address.</span></span>
  
 <span data-ttu-id="fef11-111">**Създаване на тип чувствителна информация по избор**</span><span class="sxs-lookup"><span data-stu-id="fef11-111">**Create a custom sensitive information type**</span></span>
  
<span data-ttu-id="fef11-112">Но ако искате да идентифицирате и защитавате различен тип поверителна информация като цяло, можете да [създадете персонализиран тип информация](https://docs.microsoft.com/microsoft-365/compliance/create-a-custom-sensitive-information-type) в потребителския интерфейс на центъра за съответствие на & за защита.</span><span class="sxs-lookup"><span data-stu-id="fef11-112">But if you need to identify and protect a different type of sensitive information altogether, you can [create a custom sensitive information type](https://docs.microsoft.com/microsoft-365/compliance/create-a-custom-sensitive-information-type) in the UI of the Security & Compliance Center.</span></span>
  
<span data-ttu-id="fef11-113">**Създаване на тип чувствителна информация по избор в центъра за защита на &**</span><span class="sxs-lookup"><span data-stu-id="fef11-113">**Create a custom sensitive information type in Security & Compliance Center PowerShell**</span></span>

<span data-ttu-id="fef11-114">И накрая, ако ИНТЕРФЕЙСът не предоставя всички опции, от които имате нужда, можете да [създадете персонализиран тип информация по избор в центъра за защита на & за съответствие на PowerShell](https://docs.microsoft.com/microsoft-365/compliance/create-a-custom-sensitive-information-type-in-scc-powershell).</span><span class="sxs-lookup"><span data-stu-id="fef11-114">Finally, if the UI doesn't provide all the options you need, you can [create a custom sensitive information type in Security & Compliance Center PowerShell](https://docs.microsoft.com/microsoft-365/compliance/create-a-custom-sensitive-information-type-in-scc-powershell).</span></span> <span data-ttu-id="fef11-115">Като започнете с XML файл, можете да използвате всяка налична опция.</span><span class="sxs-lookup"><span data-stu-id="fef11-115">By starting with an XML file, you can use every option available.</span></span>
