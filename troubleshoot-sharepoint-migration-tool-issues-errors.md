---
title: Отстраняване на проблеми и грешки при мигриране на SharePoint
ms.author: v-miegge
author: v-miegge
manager: v-cojank
ms.date: 10/31/2019
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "5300030"
- "3178"
ms.assetid: ''
ms.openlocfilehash: f9f5694b1d88bccebdc5448d5629ea5120c52511
ms.sourcegitcommit: b0d5b68366028abcf08610672d5bc9d3b25ac433
ms.translationtype: MT
ms.contentlocale: bg-BG
ms.lasthandoff: 03/24/2020
ms.locfileid: "42931107"
---
# <a name="troubleshooting-sharepoint-migration-tool-issues-and-errors"></a><span data-ttu-id="413dd-102">Отстраняване на проблеми и грешки при мигриране на SharePoint</span><span class="sxs-lookup"><span data-stu-id="413dd-102">Troubleshooting SharePoint Migration Tool issues and errors</span></span>

<span data-ttu-id="413dd-103">**Важно:** много sharePoint Online и OneDrive клиенти работят критични бизнес приложения срещу услугата, която се изпълнява във фонов режим.</span><span class="sxs-lookup"><span data-stu-id="413dd-103">**Important**: Many SharePoint Online and OneDrive customers run business-critical applications against the service that run in the background.</span></span> <span data-ttu-id="413dd-104">Те включват миграция на съдържанието, предотвратяване на загуба на данни (DLP) и архивиране на решения.</span><span class="sxs-lookup"><span data-stu-id="413dd-104">These include content migration, Data Loss Prevention (DLP), and backup solutions.</span></span> <span data-ttu-id="413dd-105">По време на тези безпрецедентни времена ние предприемаме стъпки, за да гарантираме, че SharePoint Online и OneDrive услуги остават високо достъпни и надеждни за вашите потребители, които зависят от услугата повече от всякога в отдалечени работни сценарии.</span><span class="sxs-lookup"><span data-stu-id="413dd-105">During these unprecedented times, we are taking steps to ensure that SharePoint Online and OneDrive services remain highly available and reliable for your users who depend on the service more than ever in remote work scenarios.</span></span>

<span data-ttu-id="413dd-106">В подкрепа на тази цел, ние сме внедрили по-строги ограничения за ограничаване на приложенията за фон (миграция, DLP и архивиране на решения) през делничните дни.</span><span class="sxs-lookup"><span data-stu-id="413dd-106">In support of this objective, we have implemented tighter throttling limits on background apps (migration, DLP and backup solutions) during weekday daytime hours.</span></span> <span data-ttu-id="413dd-107">Трябва да очаквате, че тези приложения ще постигнат много ограничена пропускателна информация по време на тези времена.</span><span class="sxs-lookup"><span data-stu-id="413dd-107">You should expect that these apps will achieve very limited throughput during these times.</span></span> <span data-ttu-id="413dd-108">Въпреки това, по време на вечерните и почивните часове за региона, услугата ще бъде готова да обработи значително по-голям обем заявки от приложения за фон.</span><span class="sxs-lookup"><span data-stu-id="413dd-108">However, during evening and weekend hours for the region, the service will be ready to process a significantly higher volume of requests from background apps.</span></span>

<span data-ttu-id="413dd-109">**Често срещани проблеми и грешки**</span><span class="sxs-lookup"><span data-stu-id="413dd-109">**Common issues and errors**</span></span>

<span data-ttu-id="413dd-110">Може да срещнете някои често срещани проблеми и грешки при използване на инструмента за мигриране на SharePoint (SPMT).</span><span class="sxs-lookup"><span data-stu-id="413dd-110">You may encounter some common issues and errors when using the SharePoint Migration Tool (SPMT).</span></span> <span data-ttu-id="413dd-111">Моля, посочете линковете по-долу за повече информация.</span><span class="sxs-lookup"><span data-stu-id="413dd-111">Please reference the links below for more information.</span></span>

* [<span data-ttu-id="413dd-112">Отстраняване на често срещани SPMT проблеми и грешки</span><span class="sxs-lookup"><span data-stu-id="413dd-112">Troubleshooting common SPMT issues and errors</span></span>](https://docs.microsoft.com/sharepointmigration/troubleshooting-common-spmt-issues)
* [<span data-ttu-id="413dd-113">Отстраняване на проблеми при инсталиране на SPMT</span><span class="sxs-lookup"><span data-stu-id="413dd-113">Troubleshooting SPMT install issues</span></span>](https://docs.microsoft.com/sharepointmigration/spmt-install-issues)