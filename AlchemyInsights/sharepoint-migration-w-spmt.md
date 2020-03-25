---
title: Мигриране на SharePoint с SPMT
ms.author: v-todmc
author: todmccoy
manager: mnirkhe
ms.date: 9/18/19
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "5300030"
- "2594"
ms.openlocfilehash: e7719d1fc6dda0d5bd340775219401dade2933fe
ms.sourcegitcommit: b0d5b68366028abcf08610672d5bc9d3b25ac433
ms.translationtype: MT
ms.contentlocale: bg-BG
ms.lasthandoff: 03/24/2020
ms.locfileid: "42931539"
---
# <a name="sharepoint-migration-with-spmt"></a><span data-ttu-id="096f3-102">Мигриране на SharePoint с SPMT</span><span class="sxs-lookup"><span data-stu-id="096f3-102">SharePoint Migration with SPMT</span></span>

<span data-ttu-id="096f3-103">**Важно:** много sharePoint Online и OneDrive клиенти работят критични бизнес приложения срещу услугата, която се изпълнява във фонов режим.</span><span class="sxs-lookup"><span data-stu-id="096f3-103">**Important**: Many SharePoint Online and OneDrive customers run business-critical applications against the service that run in the background.</span></span> <span data-ttu-id="096f3-104">Те включват миграция на съдържанието, предотвратяване на загуба на данни (DLP) и архивиране на решения.</span><span class="sxs-lookup"><span data-stu-id="096f3-104">These include content migration, Data Loss Prevention (DLP), and backup solutions.</span></span> <span data-ttu-id="096f3-105">По време на тези безпрецедентни времена ние предприемаме стъпки, за да гарантираме, че SharePoint Online и OneDrive услуги остават високо достъпни и надеждни за вашите потребители, които зависят от услугата повече от всякога в отдалечени работни сценарии.</span><span class="sxs-lookup"><span data-stu-id="096f3-105">During these unprecedented times, we are taking steps to ensure that SharePoint Online and OneDrive services remain highly available and reliable for your users who depend on the service more than ever in remote work scenarios.</span></span>

<span data-ttu-id="096f3-106">В подкрепа на тази цел, ние сме внедрили по-строги ограничения за ограничаване на приложенията за фон (миграция, DLP и архивиране на решения) през делничните дни.</span><span class="sxs-lookup"><span data-stu-id="096f3-106">In support of this objective, we have implemented tighter throttling limits on background apps (migration, DLP and backup solutions) during weekday daytime hours.</span></span> <span data-ttu-id="096f3-107">Трябва да очаквате, че тези приложения ще постигнат много ограничена пропускателна информация по време на тези времена.</span><span class="sxs-lookup"><span data-stu-id="096f3-107">You should expect that these apps will achieve very limited throughput during these times.</span></span> <span data-ttu-id="096f3-108">Въпреки това, по време на вечерните и почивните часове за региона, услугата ще бъде готова да обработи значително по-голям обем заявки от приложения за фон.</span><span class="sxs-lookup"><span data-stu-id="096f3-108">However, during evening and weekend hours for the region, the service will be ready to process a significantly higher volume of requests from background apps.</span></span>

<span data-ttu-id="096f3-109">**Инструмент за мигриране на SharePoint**</span><span class="sxs-lookup"><span data-stu-id="096f3-109">**SharePoint Migration Tool**</span></span>

<span data-ttu-id="096f3-110">Проектиран да се използва за миграции, вариращи от най-малкия набор от файлове до мащабна корпоративна миграция, инструмента за миграция на SharePoint ще ви позволи да прехвърлите вашата информация в облака и да се възползвате от най-новите сътрудничество, разузнаване, и решения за защита с Office 365.</span><span class="sxs-lookup"><span data-stu-id="096f3-110">Designed to be used for migrations ranging from the smallest set of files to a large scale enterprise migration, the SharePoint Migration Tool will allow you to transfer your information to the cloud and take advantage of the newest collaboration, intelligence, and security solutions with Office 365.</span></span>

- [<span data-ttu-id="096f3-111">Изтеглете и инсталирайте инструмента за мигриране на SharePoint</span><span class="sxs-lookup"><span data-stu-id="096f3-111">Download and install the SharePoint Migration Tool</span></span>](https://docs.microsoft.com/sharepointmigration/introducing-the-sharepoint-migration-tool)
- [<span data-ttu-id="096f3-112">Отстраняване на често срещани SPMT проблеми и грешки</span><span class="sxs-lookup"><span data-stu-id="096f3-112">Troubleshooting common SPMT issues and errors</span></span>](https://docs.microsoft.com/sharepointmigration/troubleshooting-common-spmt-issues)
- [<span data-ttu-id="096f3-113">Отстраняване на проблеми при инсталиране на SPMT</span><span class="sxs-lookup"><span data-stu-id="096f3-113">Troubleshooting SPMT installation issues</span></span>](https://docs.microsoft.com/sharepointmigration/spmt-install-issues#troubleshooting-spmt-installation-issues)
