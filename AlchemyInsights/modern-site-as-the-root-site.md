---
title: Модерен сайт като корен сайт
ms.author: pebaum
author: pebaum
ms.audience: ITPro
ms.topic: article
ms.date: 04/21/2020
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000265"
- "1874"
ms.openlocfilehash: 0388f95e2b7815dcbbb6aca200f44e55e9c5724f
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: bg-BG
ms.lasthandoff: 04/22/2020
ms.locfileid: "43713780"
---
# <a name="modern-site-as-root-site"></a><span data-ttu-id="1e082-102">Модерен сайт като корен сайт</span><span class="sxs-lookup"><span data-stu-id="1e082-102">Modern site as root site</span></span>

<span data-ttu-id="1e082-103">Започнахме да разгръщаме нова функция, която ще ви позволи да [замените коренния си сайт с модерен сайт.](https://docs.microsoft.com/sharepoint/modern-root-site)</span><span class="sxs-lookup"><span data-stu-id="1e082-103">We have begun to rollout a new feature that will allow you to [swap your classic site root site with a modern site](https://docs.microsoft.com/sharepoint/modern-root-site).</span></span> <span data-ttu-id="1e082-104">Използвайте [Invoke-SPOSiteSwap](https://docs.microsoft.com/powershell/module/sharepoint-online/invoke-spositeswap?view=sharepoint-ps) за размяна на местоположението на сайт с друг сайт, докато архивирате оригиналния сайт.</span><span class="sxs-lookup"><span data-stu-id="1e082-104">Use [Invoke-SPOSiteSwap](https://docs.microsoft.com/powershell/module/sharepoint-online/invoke-spositeswap?view=sharepoint-ps) to swap the location of a site with another site while archiving the original site.</span></span> <span data-ttu-id="1e082-105">Предлага се за двете екипни сайтове (не свързани с група) и сайт за комуникация.</span><span class="sxs-lookup"><span data-stu-id="1e082-105">Available for both Team Site (not connected to a group) and Communication Site.</span></span>

>[!Important]
> <span data-ttu-id="1e082-106">Не изтривайте класическия си корен сайт, за да създадете модерен сайт за комуникация.</span><span class="sxs-lookup"><span data-stu-id="1e082-106">Do not delete your classic root site to create a modern Communication Site.</span></span> <span data-ttu-id="1e082-107">Това не се поддържа от Microsoft.</span><span class="sxs-lookup"><span data-stu-id="1e082-107">This is not supported by Microsoft.</span></span> <span data-ttu-id="1e082-108">Изтриването на главния сайт ще направи всички сайтове на SharePoint във вашата организация недостъпни за всички потребители, докато не възстановите сайта или създадете нов сайт със същия URL адрес.</span><span class="sxs-lookup"><span data-stu-id="1e082-108">Deleting the root site will make all SharePoint sites in your organization inaccessible to all users, until you restore the site or create a new site at the same URL.</span></span> <span data-ttu-id="1e082-109">Ще комуникираме тази функция чрез центъра за съобщения.</span><span class="sxs-lookup"><span data-stu-id="1e082-109">We’ll be communicating this feature via the message center.</span></span> <span data-ttu-id="1e082-110">Трябва да очаквате, че функцията ще бъде включена в клиента ви скоро.</span><span class="sxs-lookup"><span data-stu-id="1e082-110">You should expect the feature to be turned on in your tenant shortly.</span></span>

## <a name="known-issues-with-swapping-sites"></a><span data-ttu-id="1e082-111">Известни проблеми при смяна на сайтове</span><span class="sxs-lookup"><span data-stu-id="1e082-111">Known issues with swapping sites</span></span>
- <span data-ttu-id="1e082-112">Целевият сайт може да върне грешка "не е намерена" (HTTP 404) за кратък период от време.</span><span class="sxs-lookup"><span data-stu-id="1e082-112">The target site may return a "not found" (HTTP 404) error for a short period of time.</span></span>
- <span data-ttu-id="1e082-113">Съдържанието ще трябва да бъде обхождано, за да се актуализира индексът за търсене.</span><span class="sxs-lookup"><span data-stu-id="1e082-113">Content will need to be recrawled to update the search index.</span></span> <span data-ttu-id="1e082-114">Тук не се изисква ръчна стъпка, това ще бъде направено автоматично.</span><span class="sxs-lookup"><span data-stu-id="1e082-114">There is no manual step required here, this will be done automatically.</span></span>
- <span data-ttu-id="1e082-115">Всичко зависимо от "статични" връзки (като синхронизиране на файлове и файлове на OneNote) ще трябва да бъдат коригирани ръчно.</span><span class="sxs-lookup"><span data-stu-id="1e082-115">Anything dependent on "static" links (such as File Sync and OneNote files) will need to be manually corrected.</span></span>
- <span data-ttu-id="1e082-116">Project Server сайтове може да се наложи да се провери да се гарантира, че те все още са свързани правилно.</span><span class="sxs-lookup"><span data-stu-id="1e082-116">Project Server sites may need to be validated to ensure that they are still associated correctly.</span></span> 
