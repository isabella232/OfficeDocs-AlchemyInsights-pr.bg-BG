---
title: Производителност при мигриране на SharePoint
ms.author: pebaum
author: pebaum
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.assetid: 686e8f18-b871-4dd2-864f-8562947ab583
ms.collection: Adm_O365
ms.custom:
- "5300030"
- "2700"
ms.openlocfilehash: 812444589d5a5bf766bbc6f466077d4ca829d79f
ms.sourcegitcommit: b0d5b68366028abcf08610672d5bc9d3b25ac433
ms.translationtype: HT
ms.contentlocale: bg-BG
ms.lasthandoff: 03/24/2020
ms.locfileid: "42931822"
---
# <a name="sharepoint-migration-performance"></a><span data-ttu-id="fb66e-102">Производителност при мигриране на SharePoint</span><span class="sxs-lookup"><span data-stu-id="fb66e-102">SharePoint migration performance</span></span>

<span data-ttu-id="fb66e-103">**Важно**: много клиенти на SharePoint Online и OneDrive изпълняват критични за бизнеса приложения спрямо услугата, която се изпълнява във фонов режим.</span><span class="sxs-lookup"><span data-stu-id="fb66e-103">**Important**: Many SharePoint Online and OneDrive customers run business-critical applications against the service that run in the background.</span></span> <span data-ttu-id="fb66e-104">Те включват миграция на съдържание, защита от загуба на данни (DLP) и решения за архивиране.</span><span class="sxs-lookup"><span data-stu-id="fb66e-104">These include content migration, Data Loss Prevention (DLP), and backup solutions.</span></span> <span data-ttu-id="fb66e-105">В тези безпрецедентни времена предприемаме стъпки, за да гарантираме, че услугите на SharePoint Online и OneDrive остават високо достъпни и надеждни за вашите потребители, които зависят от услугата повече от всякога в сценариите за отдалечена работа.</span><span class="sxs-lookup"><span data-stu-id="fb66e-105">During these unprecedented times, we are taking steps to ensure that SharePoint Online and OneDrive services remain highly available and reliable for your users who depend on the service more than ever in remote work scenarios.</span></span>

<span data-ttu-id="fb66e-106">В подкрепа на тази цел сме внедрили строги мерки за ограничаване на фоновите приложенията (миграция, DLP и решения за архивиране) по време на делничните дни през деня.</span><span class="sxs-lookup"><span data-stu-id="fb66e-106">In support of this objective, we have implemented tighter throttling limits on background apps (migration, DLP and backup solutions) during weekday daytime hours.</span></span> <span data-ttu-id="fb66e-107">Би трябвало да очаквате, че тези приложения ще бъдат с много ограничена пропускателната способност през тези часове.</span><span class="sxs-lookup"><span data-stu-id="fb66e-107">You should expect that these apps will achieve very limited throughput during these times.</span></span> <span data-ttu-id="fb66e-108">Въпреки това, вечерта и през почивните дни за вашия регион услугата ще бъде готова за обработка на значително по-голям обем заявки от фонови приложения.</span><span class="sxs-lookup"><span data-stu-id="fb66e-108">However, during evening and weekend hours for the region, the service will be ready to process a significantly higher volume of requests from background apps.</span></span>

<span data-ttu-id="fb66e-109">**Фактори за производителността при мигриране**</span><span class="sxs-lookup"><span data-stu-id="fb66e-109">**Migration performance**</span></span>

<span data-ttu-id="fb66e-110">Производителността при мигриране може да бъде повлияна от мрежовата инфраструктура, размера на файла, времето за мигриране и ограничаването.</span><span class="sxs-lookup"><span data-stu-id="fb66e-110">Migration performance can be impacted by network infrastructure, file size, migration time, and throttling.</span></span> <span data-ttu-id="fb66e-111">Разбирането на тези неща ще ви помогне да планирате и увеличите ефективността на своята миграция.</span><span class="sxs-lookup"><span data-stu-id="fb66e-111">Understanding these will help you plan and maximize the efficiency of your migration.</span></span>

<span data-ttu-id="fb66e-112">За повече информация посетете тази връзките по-долу.</span><span class="sxs-lookup"><span data-stu-id="fb66e-112">For more information, please visit the links below.</span></span>

- [<span data-ttu-id="fb66e-113">Скорост на мигриране на SharePoint Online и ODB</span><span class="sxs-lookup"><span data-stu-id="fb66e-113">Sharepoint Online and ODB Migration Speed</span></span>](https://docs.microsoft.com/sharepointmigration/sharepoint-online-and-onedrive-migration-speed)

- [<span data-ttu-id="fb66e-114">Избягване на ограничаването или блокирането в SharePoint Online</span><span class="sxs-lookup"><span data-stu-id="fb66e-114">Avoid getting throttled or blocked in SharePoint Online</span></span>](https://docs.microsoft.com/sharepoint/dev/general-development/how-to-avoid-getting-throttled-or-blocked-in-sharepoint-online)

- [<span data-ttu-id="fb66e-115">Изтегляне и инсталиране на инструмента за мигриране на SharePoint</span><span class="sxs-lookup"><span data-stu-id="fb66e-115">Download and install the SharePoint Migration Tool</span></span>](https://docs.microsoft.com/sharepointmigration/introducing-the-sharepoint-migration-tool)
