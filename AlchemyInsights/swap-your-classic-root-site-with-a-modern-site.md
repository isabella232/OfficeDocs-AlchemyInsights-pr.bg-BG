---
title: Размени класическия си корен сайт с модерен сайт
ms.author: efrene
author: efrene
ms.date: 8/6/2019
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.assetid: ''
ms.custom:
- "9000687"
- "2579"
ms.openlocfilehash: bd477d90ab7e6737aafffc57d931aad2bd0351e8
ms.sourcegitcommit: a65d196d00adb70045af5caca9828fe44b951f61
ms.translationtype: MT
ms.contentlocale: bg-BG
ms.lasthandoff: 09/04/2019
ms.locfileid: "36749249"
---
# <a name="swap-your-classic-root-site-with-a-modern-site"></a><span data-ttu-id="7636b-102">Размени класическия си корен сайт с модерен сайт</span><span class="sxs-lookup"><span data-stu-id="7636b-102">Swap your Classic root site with a Modern site</span></span>

<span data-ttu-id="7636b-103">Ако вашата среда е настроена преди април 2019, можете да промените вашия корен сайт на модерен сайт с помощта на Microsoft PowerShell:</span><span class="sxs-lookup"><span data-stu-id="7636b-103">If your environment was set up before April 2019, you can change your root site to a modern site by using Microsoft PowerShell:</span></span>

- <span data-ttu-id="7636b-104">Ако имате друг сайт, който искате да използвате като главен сайт, можете да замените [(суап) главния сайт](https://docs.microsoft.com/sharepoint/modern-root-site) с него.</span><span class="sxs-lookup"><span data-stu-id="7636b-104">If you have a different site that you want to use as your root site, you can replace [(swap) the root site](https://docs.microsoft.com/sharepoint/modern-root-site) with it.</span></span> 
    - <span data-ttu-id="7636b-105">Използвайте [извикване-SPOSiteSwap](https://docs.microsoft.com/powershell/module/sharepoint-online/invoke-spositeswap?view=sharepoint-ps) да замените местоположението на сайт с друг сайт, докато архивирате оригиналния сайт.</span><span class="sxs-lookup"><span data-stu-id="7636b-105">Use [Invoke-SPOSiteSwap](https://docs.microsoft.com/powershell/module/sharepoint-online/invoke-spositeswap?view=sharepoint-ps) to swap the location of a site with another site while archiving the original site.</span></span> <span data-ttu-id="7636b-106">Предлага се и за двата екипен сайт (не е свързан с група) и сайт за комуникация.</span><span class="sxs-lookup"><span data-stu-id="7636b-106">Available for both Team Site (not connected to a group) and Communication Site.</span></span> 

- <span data-ttu-id="7636b-107">Скоро ще бъдат въведени допълнителни възможности, които ще ви позволят да използвате съдържанието на сайта, но да конвертирате съществуващия сайт в сайт за комуникация.</span><span class="sxs-lookup"><span data-stu-id="7636b-107">Additional capabilities will be introduced soon that will allow you to keep using the content on the site, but convert the existing site to a communication site.</span></span> 
>[!Important]
><span data-ttu-id="7636b-108">Тези възможности ще се извършват постепенно.</span><span class="sxs-lookup"><span data-stu-id="7636b-108">These capabilities will be rolled out gradually.</span></span> <span data-ttu-id="7636b-109">Продължете да проверявате центъра за съобщения на Office 365 за актуализации.</span><span class="sxs-lookup"><span data-stu-id="7636b-109">Continue to check the Office 365 Message Center for updates.</span></span> 

## <a name="known-issues-with-swapping-sites"></a><span data-ttu-id="7636b-110">Известни проблеми с размяна на сайтове</span><span class="sxs-lookup"><span data-stu-id="7636b-110">Known issues with swapping sites</span></span>

- <span data-ttu-id="7636b-111">Целевият сайт може да върне грешка "не е намерен" (HTTP 404) за кратък период от време.</span><span class="sxs-lookup"><span data-stu-id="7636b-111">The target site may return a "not found" (HTTP 404) error for a short period of time.</span></span>
- <span data-ttu-id="7636b-112">Съдържанието ще трябва да бъде преприложено, за да се актуализира индексът за търсене.</span><span class="sxs-lookup"><span data-stu-id="7636b-112">Content will need to be recrawled to update the search index.</span></span> <span data-ttu-id="7636b-113">Не е необходима ръчна стъпка-това ще бъде направено автоматично.</span><span class="sxs-lookup"><span data-stu-id="7636b-113">There is no manual step required - this will be done automatically.</span></span>
- <span data-ttu-id="7636b-114">Всичко, зависимо от "статични" връзки (като файл Sync и OneNote файлове) ще трябва да бъдат ръчно коригирани.</span><span class="sxs-lookup"><span data-stu-id="7636b-114">Anything dependent on "static" links (such as File Sync and OneNote files) will need to be manually corrected.</span></span>
- <span data-ttu-id="7636b-115">Ако сайтът източник е сайт за организационни новини, актуализирайте URL адреса.</span><span class="sxs-lookup"><span data-stu-id="7636b-115">If the source site was an organizational news site, update the URL.</span></span><span data-ttu-id="7636b-116">Получете списък с всички сайтове за организационни новини.</span><span class="sxs-lookup"><span data-stu-id="7636b-116"> Get a list of all organizational news sites.</span></span>
- <span data-ttu-id="7636b-117">Project Server сайтове може да се наложи да бъдат валидирани, за да се уверите, че те все още са свързани правилно.</span><span class="sxs-lookup"><span data-stu-id="7636b-117">Project Server sites may need to be validated to ensure that they are still associated correctly.</span></span>





