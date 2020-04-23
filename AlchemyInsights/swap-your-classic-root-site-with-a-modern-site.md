---
title: Разменете класическия си главен сайт с модерен сайт
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.assetid: ''
ms.custom:
- "9000687"
- "2579"
ms.openlocfilehash: f4831c6a232a4dee0f8f5ac0c83e4307221cfe2d
ms.sourcegitcommit: 631cbb5f03e5371f0995e976536d24e9d13746c3
ms.translationtype: MT
ms.contentlocale: bg-BG
ms.lasthandoff: 04/22/2020
ms.locfileid: "43741533"
---
# <a name="swap-your-classic-root-site-with-a-modern-site"></a><span data-ttu-id="b389a-102">Разменете класическия си главен сайт с модерен сайт</span><span class="sxs-lookup"><span data-stu-id="b389a-102">Swap your Classic root site with a Modern site</span></span>

<span data-ttu-id="b389a-103">Ако вашата среда е създадена преди април 2019 г., можете да промените вашия главен сайт модерен сайт с помощта на Microsoft PowerShell:</span><span class="sxs-lookup"><span data-stu-id="b389a-103">If your environment was set up before April 2019, you can change your root site to a modern site by using Microsoft PowerShell:</span></span>

- <span data-ttu-id="b389a-104">Ако имате друг сайт, който искате да използвате като корен, можете да [замените (замени) коренния сайт](https://docs.microsoft.com/sharepoint/modern-root-site) с него.</span><span class="sxs-lookup"><span data-stu-id="b389a-104">If you have a different site that you want to use as your root site, you can replace [(swap) the root site](https://docs.microsoft.com/sharepoint/modern-root-site) with it.</span></span> 
    - <span data-ttu-id="b389a-105">Използвайте [Invoke-SPOSiteSwap](https://docs.microsoft.com/powershell/module/sharepoint-online/invoke-spositeswap?view=sharepoint-ps) за размяна на местоположението на сайт с друг сайт, докато архивирате оригиналния сайт.</span><span class="sxs-lookup"><span data-stu-id="b389a-105">Use [Invoke-SPOSiteSwap](https://docs.microsoft.com/powershell/module/sharepoint-online/invoke-spositeswap?view=sharepoint-ps) to swap the location of a site with another site while archiving the original site.</span></span> <span data-ttu-id="b389a-106">Предлага се за двете екипни сайтове (не свързани с група) и сайт за комуникация.</span><span class="sxs-lookup"><span data-stu-id="b389a-106">Available for both Team Site (not connected to a group) and Communication Site.</span></span> 

- <span data-ttu-id="b389a-107">Скоро ще бъдат въведени допълнителни възможности, които ще ви позволят да продължите да използвате съдържанието на сайта, но да конвертирате съществуващия сайт в комуникационен сайт.</span><span class="sxs-lookup"><span data-stu-id="b389a-107">Additional capabilities will be introduced soon that will allow you to keep using the content on the site, but convert the existing site to a communication site.</span></span> 
>[!Important]
><span data-ttu-id="b389a-108">Тези възможности ще бъдат постепенно разточени.</span><span class="sxs-lookup"><span data-stu-id="b389a-108">These capabilities will be rolled out gradually.</span></span> <span data-ttu-id="b389a-109">Продължете да проверявате центъра за съобщения за актуализации.</span><span class="sxs-lookup"><span data-stu-id="b389a-109">Continue to check the Message Center for updates.</span></span> 

## <a name="known-issues-with-swapping-sites"></a><span data-ttu-id="b389a-110">Известни проблеми при смяна на сайтове</span><span class="sxs-lookup"><span data-stu-id="b389a-110">Known issues with swapping sites</span></span>

- <span data-ttu-id="b389a-111">Целевият сайт може да върне грешка "не е намерена" (HTTP 404) за кратък период от време.</span><span class="sxs-lookup"><span data-stu-id="b389a-111">The target site may return a "not found" (HTTP 404) error for a short period of time.</span></span>
- <span data-ttu-id="b389a-112">Съдържанието ще трябва да бъде обхождано, за да се актуализира индексът за търсене.</span><span class="sxs-lookup"><span data-stu-id="b389a-112">Content will need to be recrawled to update the search index.</span></span> <span data-ttu-id="b389a-113">Няма необходима ръчна стъпка - това ще бъде направено автоматично.</span><span class="sxs-lookup"><span data-stu-id="b389a-113">There is no manual step required - this will be done automatically.</span></span>
- <span data-ttu-id="b389a-114">Всичко зависимо от "статични" връзки (като синхронизиране на файлове и файлове на OneNote) ще трябва да бъдат коригирани ръчно.</span><span class="sxs-lookup"><span data-stu-id="b389a-114">Anything dependent on "static" links (such as File Sync and OneNote files) will need to be manually corrected.</span></span>
- <span data-ttu-id="b389a-115">Ако сайтът източник е сайт за организационни новини, актуализирайте URL адреса.</span><span class="sxs-lookup"><span data-stu-id="b389a-115">If the source site was an organizational news site, update the URL.</span></span><span data-ttu-id="b389a-116">Получете списък с всички сайтове за организационни новини.</span><span class="sxs-lookup"><span data-stu-id="b389a-116"> Get a list of all organizational news sites.</span></span>
- <span data-ttu-id="b389a-117">Project Server сайтове може да се наложи да се провери да се гарантира, че те все още са свързани правилно.</span><span class="sxs-lookup"><span data-stu-id="b389a-117">Project Server sites may need to be validated to ensure that they are still associated correctly.</span></span>
