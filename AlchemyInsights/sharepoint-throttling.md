---
title: Онлайн ограничаване на SharePoint
ms.author: pebaum
author: pebaum
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: b376d8ea-50c4-47f0-9720-50d80aa3f7f1
ms.openlocfilehash: 9af4f09d50992c04a1f3d5a164093049a3ec3517
ms.sourcegitcommit: b0d5b68366028abcf08610672d5bc9d3b25ac433
ms.translationtype: MT
ms.contentlocale: bg-BG
ms.lasthandoff: 03/24/2020
ms.locfileid: "42931431"
---
# <a name="sharepoint-online-throttling"></a><span data-ttu-id="cd06e-102">Онлайн ограничаване на SharePoint</span><span class="sxs-lookup"><span data-stu-id="cd06e-102">SharePoint Online throttling</span></span>

<span data-ttu-id="cd06e-103">**Важно:** много sharePoint Online и OneDrive клиенти работят критични бизнес приложения срещу услугата, която се изпълнява във фонов режим.</span><span class="sxs-lookup"><span data-stu-id="cd06e-103">**Important**: Many SharePoint Online and OneDrive customers run business-critical applications against the service that run in the background.</span></span> <span data-ttu-id="cd06e-104">Те включват миграция на съдържанието, предотвратяване на загуба на данни (DLP) и архивиране на решения.</span><span class="sxs-lookup"><span data-stu-id="cd06e-104">These include content migration, Data Loss Prevention (DLP), and backup solutions.</span></span> <span data-ttu-id="cd06e-105">По време на тези безпрецедентни времена ние предприемаме стъпки, за да гарантираме, че SharePoint Online и OneDrive услуги остават високо достъпни и надеждни за вашите потребители, които зависят от услугата повече от всякога в отдалечени работни сценарии.</span><span class="sxs-lookup"><span data-stu-id="cd06e-105">During these unprecedented times, we are taking steps to ensure that SharePoint Online and OneDrive services remain highly available and reliable for your users who depend on the service more than ever in remote work scenarios.</span></span>

<span data-ttu-id="cd06e-106">В подкрепа на тази цел, ние сме внедрили по-строги ограничения за ограничаване на приложенията за фон (миграция, DLP и архивиране на решения) през делничните дни.</span><span class="sxs-lookup"><span data-stu-id="cd06e-106">In support of this objective, we have implemented tighter throttling limits on background apps (migration, DLP and backup solutions) during weekday daytime hours.</span></span> <span data-ttu-id="cd06e-107">Трябва да очаквате, че тези приложения ще постигнат много ограничена пропускателна информация по време на тези времена.</span><span class="sxs-lookup"><span data-stu-id="cd06e-107">You should expect that these apps will achieve very limited throughput during these times.</span></span> <span data-ttu-id="cd06e-108">Въпреки това, по време на вечерните и почивните часове за региона, услугата ще бъде готова да обработи значително по-голям обем заявки от приложения за фон.</span><span class="sxs-lookup"><span data-stu-id="cd06e-108">However, during evening and weekend hours for the region, the service will be ready to process a significantly higher volume of requests from background apps.</span></span>

<span data-ttu-id="cd06e-109">**Онлайн ограничаване на SharePoint**</span><span class="sxs-lookup"><span data-stu-id="cd06e-109">**SharePoint Online throttling**</span></span>

<span data-ttu-id="cd06e-110">SharePoint Online използва дроселиране да поддържа оптимално производителност и надеждност на услугата на SharePoint Online.</span><span class="sxs-lookup"><span data-stu-id="cd06e-110">SharePoint Online uses throttling to maintain optimal performance and reliability of the SharePoint Online service.</span></span> <span data-ttu-id="cd06e-111">Ограничаването ограничава броя на действията на потребителя или едновременните повиквания (със скрипт или код), за да се предотврати превес на ресурсите.</span><span class="sxs-lookup"><span data-stu-id="cd06e-111">Throttling limits the number of user actions or concurrent calls (by script or code) to prevent overuse of resources.</span></span> <span data-ttu-id="cd06e-112">За повече информация, моля, посетете връзките по-долу.</span><span class="sxs-lookup"><span data-stu-id="cd06e-112">For more information, please visit the links below.</span></span>

- [<span data-ttu-id="cd06e-113">Избягвайте да се дросели или блокирани в SharePoint Online</span><span class="sxs-lookup"><span data-stu-id="cd06e-113">Avoid getting throttled or blocked in SharePoint Online</span></span>](https://docs.microsoft.com/sharepoint/dev/general-development/how-to-avoid-getting-throttled-or-blocked-in-sharepoint-online)

- [<span data-ttu-id="cd06e-114">Миграция на данни и SPO ограничаване</span><span class="sxs-lookup"><span data-stu-id="cd06e-114">Data Migration and SPO Throttling </span></span>](https://blogs.technet.microsoft.com/sposupport/2017/08/12/data-migration-and-spo-service-throttling/)

- [<span data-ttu-id="cd06e-115">SharePoint Онлайн и скоростта на преместване на OneDrive</span><span class="sxs-lookup"><span data-stu-id="cd06e-115">SharePoint Online and OneDrive Migration Speed</span></span>](https://docs.microsoft.com/sharepointmigration/sharepoint-online-and-onedrive-migration-speed)

 - [<span data-ttu-id="cd06e-116">Манипулиране на SharePoint Online ограничаване чрез експоненциално отказваме</span><span class="sxs-lookup"><span data-stu-id="cd06e-116">Handle SharePoint Online throttling by using exponential back off</span></span>](https://docs.microsoft.com/sharepoint/dev/solution-guidance/handle-sharepoint-online-throttling-by-using-exponential-back-off)

- [<span data-ttu-id="cd06e-117">Планиране на капацитет и тестване на натоварването на SharePoint Online</span><span class="sxs-lookup"><span data-stu-id="cd06e-117">Capacity planning and load testing SharePoint Online</span></span>](https://docs.microsoft.com/office365/enterprise/capacity-planning-and-load-testing-sharepoint-online)

