---
title: Модерен сайт като корен сайт
ms.author: pebaum
author: pebaum
ms.audience: ITPro
ms.topic: article
ms.date: 8/7/2019
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000265"
- "1874"
ms.openlocfilehash: 2e2bb02b9dbaf7f8ede0b4c5ba8c8f29453309cb
ms.sourcegitcommit: 0f0186044a3597e42ad14c32ca58e7224344dcfa
ms.translationtype: MT
ms.contentlocale: bg-BG
ms.lasthandoff: 12/15/2019
ms.locfileid: "40054691"
---
# <a name="modern-site-as-root-site"></a><span data-ttu-id="e515f-102">Модерен сайт като корен сайт</span><span class="sxs-lookup"><span data-stu-id="e515f-102">Modern site as root site</span></span>

<span data-ttu-id="e515f-103">Ние сме започнали да разгръщане на нова функция, която ще ви позволи да [замените класическия сайт корен сайт с модерен сайт](https://docs.microsoft.com/sharepoint/modern-root-site).</span><span class="sxs-lookup"><span data-stu-id="e515f-103">We have begun to rollout a new feature that will allow you to [swap your classic site root site with a modern site](https://docs.microsoft.com/sharepoint/modern-root-site).</span></span> <span data-ttu-id="e515f-104">Използвайте [извикване-SPOSiteSwap](https://docs.microsoft.com/powershell/module/sharepoint-online/invoke-spositeswap?view=sharepoint-ps) да замените местоположението на сайт с друг сайт, докато архивирате оригиналния сайт.</span><span class="sxs-lookup"><span data-stu-id="e515f-104">Use [Invoke-SPOSiteSwap](https://docs.microsoft.com/powershell/module/sharepoint-online/invoke-spositeswap?view=sharepoint-ps) to swap the location of a site with another site while archiving the original site.</span></span> <span data-ttu-id="e515f-105">Предлага се и за двата екипен сайт (не е свързан с група) и сайт за комуникация.</span><span class="sxs-lookup"><span data-stu-id="e515f-105">Available for both Team Site (not connected to a group) and Communication Site.</span></span>

>[!Important]
> <span data-ttu-id="e515f-106">Не изтривайте класическия корен сайт, за да създадете модерен комуникационен сайт.</span><span class="sxs-lookup"><span data-stu-id="e515f-106">Do not delete your classic root site to create a modern Communication Site.</span></span> <span data-ttu-id="e515f-107">Това не се поддържа от Microsoft.</span><span class="sxs-lookup"><span data-stu-id="e515f-107">This is not supported by Microsoft.</span></span> <span data-ttu-id="e515f-108">Изтриването на главния сайт ще направи всички сайтове на SharePoint във вашата организация недостъпни за всички потребители, докато не възстановите сайта или не създадете нов сайт на същия URL адрес.</span><span class="sxs-lookup"><span data-stu-id="e515f-108">Deleting the root site will make all SharePoint sites in your organization inaccessible to all users, until you restore the site or create a new site at the same URL.</span></span> <span data-ttu-id="e515f-109">Ще общуваме с тази функция чрез центъра за съобщения.</span><span class="sxs-lookup"><span data-stu-id="e515f-109">We’ll be communicating this feature via the message center.</span></span> <span data-ttu-id="e515f-110">Трябва да очаквате функцията да бъде включена в вашия наемател скоро.</span><span class="sxs-lookup"><span data-stu-id="e515f-110">You should expect the feature to be turned on in your tenant shortly.</span></span>

## <a name="known-issues-with-swapping-sites"></a><span data-ttu-id="e515f-111">Известни проблеми с размяна на сайтове</span><span class="sxs-lookup"><span data-stu-id="e515f-111">Known issues with swapping sites</span></span>
- <span data-ttu-id="e515f-112">Целевият сайт може да върне грешка "не е намерен" (HTTP 404) за кратък период от време.</span><span class="sxs-lookup"><span data-stu-id="e515f-112">The target site may return a "not found" (HTTP 404) error for a short period of time.</span></span>
- <span data-ttu-id="e515f-113">Съдържанието ще трябва да бъде преприложено, за да се актуализира индексът за търсене.</span><span class="sxs-lookup"><span data-stu-id="e515f-113">Content will need to be recrawled to update the search index.</span></span> <span data-ttu-id="e515f-114">Не е необходима ръчна стъпка тук, това ще бъде направено автоматично.</span><span class="sxs-lookup"><span data-stu-id="e515f-114">There is no manual step required here, this will be done automatically.</span></span>
- <span data-ttu-id="e515f-115">Всичко, зависимо от "статични" връзки (като файл Sync и OneNote файлове) ще трябва да бъдат ръчно коригирани.</span><span class="sxs-lookup"><span data-stu-id="e515f-115">Anything dependent on "static" links (such as File Sync and OneNote files) will need to be manually corrected.</span></span>
- <span data-ttu-id="e515f-116">Project Server сайтове може да се наложи да бъдат валидирани, за да се уверите, че те все още са свързани правилно.</span><span class="sxs-lookup"><span data-stu-id="e515f-116">Project Server sites may need to be validated to ensure that they are still associated correctly.</span></span> 
