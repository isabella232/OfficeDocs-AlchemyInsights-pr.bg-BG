---
title: SharePoint миграция ограничаване с 503 грешки
ms.author: pebaum
author: pebaum
ms.date: 8/8/2019
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.assetid: ''
ms.custom:
- "9000136"
- "2541"
ms.openlocfilehash: 7e12c74d33e3cee7c626ad899a4e7f2f0a409bca
ms.sourcegitcommit: b0d5b68366028abcf08610672d5bc9d3b25ac433
ms.translationtype: MT
ms.contentlocale: bg-BG
ms.lasthandoff: 03/24/2020
ms.locfileid: "42931647"
---
# <a name="sharepoint-migration-throttling-with-503-errors"></a><span data-ttu-id="0f7c2-102">SharePoint миграция ограничаване с 503 грешки</span><span class="sxs-lookup"><span data-stu-id="0f7c2-102">SharePoint migration throttling with 503 errors</span></span>

<span data-ttu-id="0f7c2-103">**Важно:** много sharePoint Online и OneDrive клиенти работят критични бизнес приложения срещу услугата, която се изпълнява във фонов режим.</span><span class="sxs-lookup"><span data-stu-id="0f7c2-103">**Important**: Many SharePoint Online and OneDrive customers run business-critical applications against the service that run in the background.</span></span> <span data-ttu-id="0f7c2-104">Те включват миграция на съдържанието, предотвратяване на загуба на данни (DLP) и архивиране на решения.</span><span class="sxs-lookup"><span data-stu-id="0f7c2-104">These include content migration, Data Loss Prevention (DLP), and backup solutions.</span></span> <span data-ttu-id="0f7c2-105">По време на тези безпрецедентни времена ние предприемаме стъпки, за да гарантираме, че SharePoint Online и OneDrive услуги остават високо достъпни и надеждни за вашите потребители, които зависят от услугата повече от всякога в отдалечени работни сценарии.</span><span class="sxs-lookup"><span data-stu-id="0f7c2-105">During these unprecedented times, we are taking steps to ensure that SharePoint Online and OneDrive services remain highly available and reliable for your users who depend on the service more than ever in remote work scenarios.</span></span>

<span data-ttu-id="0f7c2-106">В подкрепа на тази цел, ние сме внедрили по-строги ограничения за ограничаване на приложенията за фон (миграция, DLP и архивиране на решения) през делничните дни.</span><span class="sxs-lookup"><span data-stu-id="0f7c2-106">In support of this objective, we have implemented tighter throttling limits on background apps (migration, DLP and backup solutions) during weekday daytime hours.</span></span> <span data-ttu-id="0f7c2-107">Трябва да очаквате, че тези приложения ще постигнат много ограничена пропускателна информация по време на тези времена.</span><span class="sxs-lookup"><span data-stu-id="0f7c2-107">You should expect that these apps will achieve very limited throughput during these times.</span></span> <span data-ttu-id="0f7c2-108">Въпреки това, по време на вечерните и почивните часове за региона, услугата ще бъде готова да обработи значително по-голям обем заявки от приложения за фон.</span><span class="sxs-lookup"><span data-stu-id="0f7c2-108">However, during evening and weekend hours for the region, the service will be ready to process a significantly higher volume of requests from background apps.</span></span>

<span data-ttu-id="0f7c2-109">**503 грешки при мигриране на SharePoint Online**</span><span class="sxs-lookup"><span data-stu-id="0f7c2-109">**503 errors when migrating to SharePoint Online**</span></span>

<span data-ttu-id="0f7c2-110">Изглежда, че мигрирате към SharePoint Online и получавате 503 грешки.</span><span class="sxs-lookup"><span data-stu-id="0f7c2-110">It appears you are migrating to SharePoint Online and receiving 503 errors.</span></span> <span data-ttu-id="0f7c2-111">Моля, следвайте стъпките по-долу, така че ние може да ви помогне възможно най-скоро.</span><span class="sxs-lookup"><span data-stu-id="0f7c2-111">Please follow the steps below so we may assist you as soon as possible.</span></span> 

1. <span data-ttu-id="0f7c2-112">Щракнете върху **връзка с поддръжка**, след което нова заявка за **сервиз**.</span><span class="sxs-lookup"><span data-stu-id="0f7c2-112">Click **Contact Support**, and then **New Service Request**.</span></span>
2. <span data-ttu-id="0f7c2-113">За заглавието и описанието въведете **SharePoint migration ограничаване с 503**.</span><span class="sxs-lookup"><span data-stu-id="0f7c2-113">For the title and description, type **SharePoint Migration Throttling with 503**.</span></span>
3. <span data-ttu-id="0f7c2-114">След като билетът е изпратен, моля, актуализирайте го със следната информация:</span><span class="sxs-lookup"><span data-stu-id="0f7c2-114">Once the ticket has been submitted, please update it with the following information:</span></span>
    - <span data-ttu-id="0f7c2-115">Колко остава от миграцията (например колко TBs?).</span><span class="sxs-lookup"><span data-stu-id="0f7c2-115">How much left of migration (for example, how many TBs?).</span></span>
    - <span data-ttu-id="0f7c2-116">Начална и крайна дата на миграция.</span><span class="sxs-lookup"><span data-stu-id="0f7c2-116">Migration start and end date.</span></span>
    - <span data-ttu-id="0f7c2-117">Опишете откъде мигрирате съдържанието си, като например SharePoint Server, Box, GDrive, Споделени файлове и др.</span><span class="sxs-lookup"><span data-stu-id="0f7c2-117">Describe where you are migrating your content from, such as SharePoint Server, Box, GDrive, File shares, etc..</span></span>
    - <span data-ttu-id="0f7c2-118">Оценете броя на дроселиращите грешки (например, x дросел на час?) и кога се случи дроселирането.</span><span class="sxs-lookup"><span data-stu-id="0f7c2-118">Estimate the number of throttling errors (for example, x throttle per hour?) and when did the throttling happen.</span></span>
    - <span data-ttu-id="0f7c2-119">Кой инструмент за мигриране използвате (например SPMT или ShareGate).</span><span class="sxs-lookup"><span data-stu-id="0f7c2-119">Which migration tool you are using (for example, SPMT or ShareGate).</span></span>


