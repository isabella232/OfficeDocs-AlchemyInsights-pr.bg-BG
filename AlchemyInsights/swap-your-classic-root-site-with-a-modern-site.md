---
title: Сменяте си класически коренен сайт с модерен сайт
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
ms.openlocfilehash: ffb1466fe436d6cab7ae5fdd60c671f5dd2654dd
ms.sourcegitcommit: 1d98db8acb9959aba3b5e308a567ade6b62da56c
ms.translationtype: MT
ms.contentlocale: bg-BG
ms.lasthandoff: 08/22/2019
ms.locfileid: "36501068"
---
# <a name="swap-your-classic-root-site-with-a-modern-site"></a><span data-ttu-id="e591c-102">Сменяте си класически коренен сайт с модерен сайт</span><span class="sxs-lookup"><span data-stu-id="e591c-102">Swap your Classic root site with a Modern site</span></span>

<span data-ttu-id="e591c-103">Ако вашата среда е настроен преди април 2019, можете да промените вашия главен сайт сайт на модерната с помощта на Microsoft PowerShell:</span><span class="sxs-lookup"><span data-stu-id="e591c-103">If your environment was set up before April 2019, you can change your root site to a modern site by using Microsoft PowerShell:</span></span>

- <span data-ttu-id="e591c-104">Ако имате различен сайт, който искате да използвате като вашия главен сайт, можете да замените (суап) корена сайта с него.</span><span class="sxs-lookup"><span data-stu-id="e591c-104">If you have a different site that you want to use as your root site, you can replace (swap) the root site with it.</span></span> 
    - <span data-ttu-id="e591c-105">Използвайте [Invoke-SPOSiteSwap](https://docs.microsoft.com/powershell/module/sharepoint-online/invoke-spositeswap?view=sharepoint-ps) да сменяте местоположението на един сайт с друг сайт при архивирането на оригиналния сайт.</span><span class="sxs-lookup"><span data-stu-id="e591c-105">Use [Invoke-SPOSiteSwap](https://docs.microsoft.com/powershell/module/sharepoint-online/invoke-spositeswap?view=sharepoint-ps) to swap the location of a site with another site while archiving the original site.</span></span> <span data-ttu-id="e591c-106">Налични за екипен сайт (не е свързан към група) и комуникация сайт.</span><span class="sxs-lookup"><span data-stu-id="e591c-106">Available for both Team Site (not connected to a group) and Communication Site.</span></span> 

- <span data-ttu-id="e591c-107">Допълнителни възможности ще бъдат въведени скоро това ще ви позволи да продължите да използвате съдържанието на сайта, но конвертирате съществуващия сайт сайт на комуникация.</span><span class="sxs-lookup"><span data-stu-id="e591c-107">Additional capabilities will be introduced soon that will allow you to keep using the content on the site, but convert the existing site to a communication site.</span></span> 
>[!Important]
><span data-ttu-id="e591c-108">Тези възможности ще се разточва постепенно.</span><span class="sxs-lookup"><span data-stu-id="e591c-108">These capabilities will be rolled out gradually.</span></span> <span data-ttu-id="e591c-109">Продължи да проверите центъра за съобщение на Office 365 за актуализации.</span><span class="sxs-lookup"><span data-stu-id="e591c-109">Continue to check the Office 365 Message Center for updates.</span></span> 

## <a name="known-issues-with-swapping-sites"></a><span data-ttu-id="e591c-110">Известни проблеми с swapping сайтове</span><span class="sxs-lookup"><span data-stu-id="e591c-110">Known issues with swapping sites</span></span>

- <span data-ttu-id="e591c-111">Целта на сайта може да се върне "не е намерена" грешка (HTTP 404) за кратък период от време.</span><span class="sxs-lookup"><span data-stu-id="e591c-111">The target site may return a "not found" (HTTP 404) error for a short period of time.</span></span>
- <span data-ttu-id="e591c-112">Съдържанието ще трябва да бъде обходен отново да актуализирате индекса за търсене.</span><span class="sxs-lookup"><span data-stu-id="e591c-112">Content will need to be recrawled to update the search index.</span></span> <span data-ttu-id="e591c-113">Там не е ръчно стъпка изисква - това ще бъде направено автоматично.</span><span class="sxs-lookup"><span data-stu-id="e591c-113">There is no manual step required - this will be done automatically.</span></span>
- <span data-ttu-id="e591c-114">Всичко зависи от "статичен" връзки (например файл синхронизация и OneNote файлове) ще трябва да бъдат коригирани ръчно.</span><span class="sxs-lookup"><span data-stu-id="e591c-114">Anything dependent on "static" links (such as File Sync and OneNote files) will need to be manually corrected.</span></span>
- <span data-ttu-id="e591c-115">Ако сайта източник е организационна новинарски сайт, актуализира URL.</span><span class="sxs-lookup"><span data-stu-id="e591c-115">If the source site was an organizational news site, update the URL.</span></span><span data-ttu-id="e591c-116">Получите списък на всички организационни новинарски сайтове.</span><span class="sxs-lookup"><span data-stu-id="e591c-116"> Get a list of all organizational news sites.</span></span>
- <span data-ttu-id="e591c-117">Проект сървър сайтове може да се наложи да се проверяват, за да се гарантира, че те все още са свързани правилно.</span><span class="sxs-lookup"><span data-stu-id="e591c-117">Project Server sites may need to be validated to ensure that they are still associated correctly.</span></span>





