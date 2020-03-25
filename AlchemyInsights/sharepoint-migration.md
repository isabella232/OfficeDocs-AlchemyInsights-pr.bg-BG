---
title: Мигриране на опциите към SharePoint Online
ms.author: pebaum
author: v-miegge
manager: v-cojank
ms.date: 11/04/2019
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.assetid: c8c339c9-2e50-4daa-aa91-3eb5053e2bc6
ms.openlocfilehash: 830b39c51658cbc02f4be81acdfdf3b164a8df70
ms.sourcegitcommit: b0d5b68366028abcf08610672d5bc9d3b25ac433
ms.translationtype: MT
ms.contentlocale: bg-BG
ms.lasthandoff: 03/24/2020
ms.locfileid: "42932719"
---
# <a name="migrate-options-to-sharepoint-online"></a><span data-ttu-id="366d0-102">Мигриране на опциите към SharePoint Online</span><span class="sxs-lookup"><span data-stu-id="366d0-102">Migrate options to SharePoint Online</span></span>

<span data-ttu-id="366d0-103">**Важно:** много sharePoint Online и OneDrive клиенти работят критични бизнес приложения срещу услугата, която се изпълнява във фонов режим.</span><span class="sxs-lookup"><span data-stu-id="366d0-103">**Important**: Many SharePoint Online and OneDrive customers run business-critical applications against the service that run in the background.</span></span> <span data-ttu-id="366d0-104">Те включват миграция на съдържанието, предотвратяване на загуба на данни (DLP) и архивиране на решения.</span><span class="sxs-lookup"><span data-stu-id="366d0-104">These include content migration, Data Loss Prevention (DLP), and backup solutions.</span></span> <span data-ttu-id="366d0-105">По време на тези безпрецедентни времена ние предприемаме стъпки, за да гарантираме, че SharePoint Online и OneDrive услуги остават високо достъпни и надеждни за вашите потребители, които зависят от услугата повече от всякога в отдалечени работни сценарии.</span><span class="sxs-lookup"><span data-stu-id="366d0-105">During these unprecedented times, we are taking steps to ensure that SharePoint Online and OneDrive services remain highly available and reliable for your users who depend on the service more than ever in remote work scenarios.</span></span>

<span data-ttu-id="366d0-106">В подкрепа на тази цел, ние сме внедрили по-строги ограничения за ограничаване на приложенията за фон (миграция, DLP и архивиране на решения) през делничните дни.</span><span class="sxs-lookup"><span data-stu-id="366d0-106">In support of this objective, we have implemented tighter throttling limits on background apps (migration, DLP and backup solutions) during weekday daytime hours.</span></span> <span data-ttu-id="366d0-107">Трябва да очаквате, че тези приложения ще постигнат много ограничена пропускателна информация по време на тези времена.</span><span class="sxs-lookup"><span data-stu-id="366d0-107">You should expect that these apps will achieve very limited throughput during these times.</span></span> <span data-ttu-id="366d0-108">Въпреки това, по време на вечерните и почивните часове за региона, услугата ще бъде готова да обработи значително по-голям обем заявки от приложения за фон.</span><span class="sxs-lookup"><span data-stu-id="366d0-108">However, during evening and weekend hours for the region, the service will be ready to process a significantly higher volume of requests from background apps.</span></span>

<span data-ttu-id="366d0-109">**Опции за миграция**</span><span class="sxs-lookup"><span data-stu-id="366d0-109">**Migration options**</span></span>

<span data-ttu-id="366d0-110">Има различни опции за мигриране на съдържание към SharePoint Online, в зависимост от размера и количеството на файловете, които трябва да преместите, моля, вижте списък с [опции, намиращи се тук](https://docs.microsoft.com/sharepointmigration/migrate-to-sharepoint-online).</span><span class="sxs-lookup"><span data-stu-id="366d0-110">There are different options available to migrate content to SharePoint Online, depending on the size and quantity of files you need to move, please see a list of options [located here](https://docs.microsoft.com/sharepointmigration/migrate-to-sharepoint-online).</span></span>

<span data-ttu-id="366d0-111">За повече информация относно миграцията на съдържанието, моля, посетете връзките по-долу.</span><span class="sxs-lookup"><span data-stu-id="366d0-111">For more information on content migration, please visit the links below.</span></span>

- [<span data-ttu-id="366d0-112">Инструмент за мигриране на Sharepoint</span><span class="sxs-lookup"><span data-stu-id="366d0-112">Sharepoint Migration Tool</span></span>](https://docs.microsoft.com/sharepointmigration/introducing-the-sharepoint-migration-tool)

- [<span data-ttu-id="366d0-113">Първи стъпки с мениджъра по миграция</span><span class="sxs-lookup"><span data-stu-id="366d0-113">Get started with the Migration Manager</span></span>](https://docs.microsoft.com/sharepointmigration/mm-get-started)

- [<span data-ttu-id="366d0-114">Скорост на мигриране на Sharepoint онлайн и ODB</span><span class="sxs-lookup"><span data-stu-id="366d0-114">Sharepoint Online and ODB Migration Speed</span></span>](https://docs.microsoft.com/sharepointmigration/sharepoint-online-and-onedrive-migration-speed)

- [<span data-ttu-id="366d0-115">Избягвайте да се дросели или блокирани в SharePoint Online</span><span class="sxs-lookup"><span data-stu-id="366d0-115">Avoid getting throttled or blocked in SharePoint Online</span></span>](https://docs.microsoft.com/sharepoint/dev/general-development/how-to-avoid-getting-throttled-or-blocked-in-sharepoint-online)

- [<span data-ttu-id="366d0-116">Инструмент за оценка на миграцията на SharePoint (SMAT)</span><span class="sxs-lookup"><span data-stu-id="366d0-116">SharePoint Migration Assessment Tool (SMAT)</span></span>](https://www.microsoft.com/download/details.aspx?id=53598&amp;751be11f-ede8-5a0c-058c-2ee190a24fa6=True)

<span data-ttu-id="366d0-117">**Забележка:** В момента sharePoint миграция инструмент поддържа само мигриране от SharePoint 2010 и 2013.</span><span class="sxs-lookup"><span data-stu-id="366d0-117">**Note**: Currently the SharePoint Migration tool only support migrations from SharePoint 2010  and 2013.</span></span> <span data-ttu-id="366d0-118">В момента не се поддържат версии 2016 или 2019.</span><span class="sxs-lookup"><span data-stu-id="366d0-118">Version 2016 or 2019 are not supported at this time.</span></span>
