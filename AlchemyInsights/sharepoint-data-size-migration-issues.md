---
title: Проблеми при мигриране на данни на SharePoint Online
ms.author: pebaum
author: pebaum
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 686e8f18-b871-4dd2-864f-8562947ab583
ms.collection: Adm_O365
ms.custom:
- "5300030"
- "1885"
ms.openlocfilehash: b53a98480bab48497274c7358f7e606caa477f5a
ms.sourcegitcommit: b0d5b68366028abcf08610672d5bc9d3b25ac433
ms.translationtype: MT
ms.contentlocale: bg-BG
ms.lasthandoff: 03/24/2020
ms.locfileid: "42931683"
---
# <a name="issues-while-migrating-data-to-sharepoint-online"></a><span data-ttu-id="96d62-102">Проблеми при мигриране на данни на SharePoint Online</span><span class="sxs-lookup"><span data-stu-id="96d62-102">Issues while migrating data to SharePoint Online</span></span>

<span data-ttu-id="96d62-103">**Важно:** много sharePoint Online и OneDrive клиенти работят критични бизнес приложения срещу услугата, която се изпълнява във фонов режим.</span><span class="sxs-lookup"><span data-stu-id="96d62-103">**Important**: Many SharePoint Online and OneDrive customers run business-critical applications against the service that run in the background.</span></span> <span data-ttu-id="96d62-104">Те включват миграция на съдържанието, предотвратяване на загуба на данни (DLP) и архивиране на решения.</span><span class="sxs-lookup"><span data-stu-id="96d62-104">These include content migration, Data Loss Prevention (DLP), and backup solutions.</span></span> <span data-ttu-id="96d62-105">По време на тези безпрецедентни времена ние предприемаме стъпки, за да гарантираме, че SharePoint Online и OneDrive услуги остават високо достъпни и надеждни за вашите потребители, които зависят от услугата повече от всякога в отдалечени работни сценарии.</span><span class="sxs-lookup"><span data-stu-id="96d62-105">During these unprecedented times, we are taking steps to ensure that SharePoint Online and OneDrive services remain highly available and reliable for your users who depend on the service more than ever in remote work scenarios.</span></span>

<span data-ttu-id="96d62-106">В подкрепа на тази цел, ние сме внедрили по-строги ограничения за ограничаване на приложенията за фон (миграция, DLP и архивиране на решения) през делничните дни.</span><span class="sxs-lookup"><span data-stu-id="96d62-106">In support of this objective, we have implemented tighter throttling limits on background apps (migration, DLP and backup solutions) during weekday daytime hours.</span></span> <span data-ttu-id="96d62-107">Трябва да очаквате, че тези приложения ще постигнат много ограничена пропускателна информация по време на тези времена.</span><span class="sxs-lookup"><span data-stu-id="96d62-107">You should expect that these apps will achieve very limited throughput during these times.</span></span> <span data-ttu-id="96d62-108">Въпреки това, по време на вечерните и почивните часове за региона, услугата ще бъде готова да обработи значително по-голям обем заявки от приложения за фон.</span><span class="sxs-lookup"><span data-stu-id="96d62-108">However, during evening and weekend hours for the region, the service will be ready to process a significantly higher volume of requests from background apps.</span></span>

<span data-ttu-id="96d62-109">**Мигриране на над 100 ТБ данни**</span><span class="sxs-lookup"><span data-stu-id="96d62-109">**Migrating over 100TB of data**</span></span>

<span data-ttu-id="96d62-110">Изглежда, че мигрирате над 100TB данни на SharePoint Online.</span><span class="sxs-lookup"><span data-stu-id="96d62-110">It appears you are migrating over 100TB of data to SharePoint Online.</span></span> <span data-ttu-id="96d62-111">Моля, следвайте стъпките по-долу, така че ние може да ви помогне възможно най-скоро.</span><span class="sxs-lookup"><span data-stu-id="96d62-111">Please follow the steps below so we may assist you as soon as possible.</span></span> 

1. <span data-ttu-id="96d62-112">Изберете **Нова заявка за сервиз**, след което щракнете върху Нова заявка за **сервиз**.</span><span class="sxs-lookup"><span data-stu-id="96d62-112">Select **New Service Request**, and then **New Service Request**.</span></span> 
2. <span data-ttu-id="96d62-113">Оставете заглавието и описанието като **мигриране на SharePoint над 100TB**.</span><span class="sxs-lookup"><span data-stu-id="96d62-113">Leave the title and description as **SharePoint migration over 100TB**.</span></span>
3. <span data-ttu-id="96d62-114">След като билетът е изпратен, моля, актуализирайте го със следната информация:</span><span class="sxs-lookup"><span data-stu-id="96d62-114">Once the ticket has been submitted, please update it with the following information:</span></span> 

    - <span data-ttu-id="96d62-115">Очакван размер на миграцията.</span><span class="sxs-lookup"><span data-stu-id="96d62-115">Estimated size of your migration.</span></span>
    - <span data-ttu-id="96d62-116">Оценка кога искате да започнете и завършите миграцията си.</span><span class="sxs-lookup"><span data-stu-id="96d62-116">An estimate of when you would like to start and complete your migration.</span></span>
    - <span data-ttu-id="96d62-117">Опишете откъде мигрирате съдържанието си, като например SharePoint Server, Box, GDrive, Споделени файлове и др.</span><span class="sxs-lookup"><span data-stu-id="96d62-117">Describe where you are migrating your content from, such as SharePoint Server, Box, GDrive, File shares, etc..</span></span>


  

