---
title: Онлайн търсене в SharePoint
ms.author: efrene
author: efrene
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: fe00f4c0-44d5-49d4-9db0-a62698bcd1d1
ms.openlocfilehash: fc49978fbd2c07381dae83061b1a1868cd1df0d0
ms.sourcegitcommit: 327a2c77afc2ff3d67d3aaaea1a92068a3c4bb1f
ms.translationtype: MT
ms.contentlocale: bg-BG
ms.lasthandoff: 08/06/2019
ms.locfileid: "36059241"
---
# <a name="search-in-sharepoint-online"></a><span data-ttu-id="c5852-102">Онлайн търсене в SharePoint</span><span class="sxs-lookup"><span data-stu-id="c5852-102">Search in SharePoint Online</span></span>

<span data-ttu-id="c5852-103">Съдържанието трябва да бъде обходен и добавя към индекса на търсачката за потребителите да намерят това, което те търсят в SharePoint Online.</span><span class="sxs-lookup"><span data-stu-id="c5852-103">Content must be crawled and added to the search index for users to find what they're searching for in SharePoint Online.</span></span> <span data-ttu-id="c5852-104">Съдържанието е автоматично обходен въз основа на предварително дефинирани обхождане график (графика на обхождането не може да се променя).</span><span class="sxs-lookup"><span data-stu-id="c5852-104">Content is automatically crawled based on a pre-defined crawl schedule (the crawl schedule cannot be changed).</span></span> <span data-ttu-id="c5852-105">Роботът вдига съдържание, което се е променило след последното обхождане и актуализира индекса.</span><span class="sxs-lookup"><span data-stu-id="c5852-105">The crawler picks up content that has changed since the last crawl and updates the index.</span></span> <span data-ttu-id="c5852-106">Да осигури се обхожда съдържанието и индексът се актуализира, обърнете внимание на следното:</span><span class="sxs-lookup"><span data-stu-id="c5852-106">To ensure content is crawled and the index is updated, note the following:</span></span>

- <span data-ttu-id="c5852-107">Уверете се, че съдържанието може да се намери чрез [съдържанието на сайта за търсене](https://docs.microsoft.com/sharepoint/make-site-content-searchable).</span><span class="sxs-lookup"><span data-stu-id="c5852-107">Make sure content can be found by [making site content searchable](https://docs.microsoft.com/sharepoint/make-site-content-searchable).</span></span>

- <span data-ttu-id="c5852-108">Когато сте променили контролирано свойство, или когато сте променили картографиране на обходен и управлявани свойства, сайтът трябва да бъде повторно обходени преди вашите промени ще бъдат отразени в индекса за търсене.</span><span class="sxs-lookup"><span data-stu-id="c5852-108">When you have changed a managed property, or when you have changed the mapping of crawled and managed properties, the site must be re-crawled before your changes will be reflected in the search index.</span></span> 

    <span data-ttu-id="c5852-109">Тъй като промените са направени в схемата на търсене, а не към самия сайт, интернет роботът не автоматично ще реиндексира сайта.</span><span class="sxs-lookup"><span data-stu-id="c5852-109">Because your changes are made in the search schema, and not to the actual site, the crawler will not automatically re-index the site.</span></span> 

    <span data-ttu-id="c5852-110">За повече информация вижте [ги поискате ръчно обхождане и повторно индексиране на даден сайт, списък или библиотека](https://docs.microsoft.com/sharepoint/crawl-site-conten).</span><span class="sxs-lookup"><span data-stu-id="c5852-110">For more info, see [Manually request crawling and re-indexing of a site, a library or a list](https://docs.microsoft.com/sharepoint/crawl-site-conten).</span></span>

- <span data-ttu-id="c5852-111">Изчакайте поне 24 часа след ръчно да поискате обхождане и пълен реиндексира да видите, Ако продължавате да имате проблем.</span><span class="sxs-lookup"><span data-stu-id="c5852-111">Wait at least 24 hours after manually requesting a crawl and full re-index to see if you're still experiencing an issue.</span></span> 

    <span data-ttu-id="c5852-112">Ако повече от 24 часа са преминали, тъй като вие инициира обхождане и пълен реиндексира, моля влезте подкрепа случай.</span><span class="sxs-lookup"><span data-stu-id="c5852-112">If more than 24 hours have passed since you initiated the crawl and full re-index, please log a support case.</span></span> <span data-ttu-id="c5852-113">В много случаи ние вече работим върху решение.</span><span class="sxs-lookup"><span data-stu-id="c5852-113">In many cases, we're already working on a solution.</span></span> <span data-ttu-id="c5852-114">Моля, дайте ни най-малко 24 часа да завършите решение.</span><span class="sxs-lookup"><span data-stu-id="c5852-114">Please give us at least 24 hours to complete a solution.</span></span>

>[! Важно!]<span data-ttu-id="c5852-115">: Ако даден сайт, документ (библиотека) или списък е бил изтрит и все още се показва в резултатите от търсенето, потребителите трябва да получават **Грешка 404 Файлът не е намерен** при опит за достъп до него.</span><span class="sxs-lookup"><span data-stu-id="c5852-115">: If a site, document (library), or a list was deleted and still shows in the search results, users should receive an **Error 404 File Not Found** when trying to access it.</span></span> <span data-ttu-id="c5852-116">Този проблем трябва да се регистрират като поддръжка на делото за допълнително разследване.</span><span class="sxs-lookup"><span data-stu-id="c5852-116">This issue should be logged as a support case for further investigation.</span></span> 



