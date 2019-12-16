---
title: Търсене в SharePoint online
ms.author: pebaum
author: pebaum
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: fe00f4c0-44d5-49d4-9db0-a62698bcd1d1
ms.openlocfilehash: c4ff98f0cf928834c803542340b32da15a40d583
ms.sourcegitcommit: 0f0186044a3597e42ad14c32ca58e7224344dcfa
ms.translationtype: MT
ms.contentlocale: bg-BG
ms.lasthandoff: 12/15/2019
ms.locfileid: "40044032"
---
# <a name="content-crawling-and-indexing-in-sharepoint-online"></a><span data-ttu-id="c1f18-102">Обхождане на съдържание и индексиране в SharePoint online</span><span class="sxs-lookup"><span data-stu-id="c1f18-102">Content crawling and indexing in SharePoint Online</span></span>

<span data-ttu-id="c1f18-103">Съдържанието трябва да бъде обходено и добавено към индекса за търсене, за да могат потребителите да намерят това, което търсят в SharePoint online.</span><span class="sxs-lookup"><span data-stu-id="c1f18-103">Content must be crawled and added to the search index for users to find what they're searching for in SharePoint Online.</span></span> <span data-ttu-id="c1f18-104">Съдържанието се обхожда автоматично въз основа на предварително дефиниран график за обхождане (графикът на обхождането не може да бъде променен).</span><span class="sxs-lookup"><span data-stu-id="c1f18-104">Content is automatically crawled based on a pre-defined crawl schedule (the crawl schedule cannot be changed).</span></span> <span data-ttu-id="c1f18-105">Роботът улавя съдържание, което се е променило след последното обхождане и актуализира индекса.</span><span class="sxs-lookup"><span data-stu-id="c1f18-105">The crawler picks up content that has changed since the last crawl and updates the index.</span></span> <span data-ttu-id="c1f18-106">За да се гарантира, че съдържанието се обхожда и индексът се актуализира, обърнете внимание на следното:</span><span class="sxs-lookup"><span data-stu-id="c1f18-106">To ensure content is crawled and the index is updated, note the following:</span></span>

- <span data-ttu-id="c1f18-107">Уверете се, че съдържанието може да бъде намерено, като [направите търсене на съдържание на сайта](https://docs.microsoft.com/sharepoint/make-site-content-searchable).</span><span class="sxs-lookup"><span data-stu-id="c1f18-107">Make sure content can be found by [making site content searchable](https://docs.microsoft.com/sharepoint/make-site-content-searchable).</span></span>

- <span data-ttu-id="c1f18-108">Когато сте променили контролирано свойство или сте променили съпоставянето на обходените и управлявани свойства, сайтът трябва да бъде повторно обходено, преди промените ви да бъдат отразени в индекса за търсене.</span><span class="sxs-lookup"><span data-stu-id="c1f18-108">When you have changed a managed property, or when you have changed the mapping of crawled and managed properties, the site must be re-crawled before your changes will be reflected in the search index.</span></span> 

    <span data-ttu-id="c1f18-109">Тъй като промените са направени в схемата за търсене, а не на действителния сайт, роботът няма автоматично да индексирате сайта.</span><span class="sxs-lookup"><span data-stu-id="c1f18-109">Because your changes are made in the search schema, and not to the actual site, the crawler will not automatically re-index the site.</span></span> 

    <span data-ttu-id="c1f18-110">За повече информация вижте [ръчно заявка за обхождане и повторно индексиране на сайт, библиотека или списък](https://docs.microsoft.com/sharepoint/crawl-site-conten).</span><span class="sxs-lookup"><span data-stu-id="c1f18-110">For more info, see [Manually request crawling and re-indexing of a site, a library or a list](https://docs.microsoft.com/sharepoint/crawl-site-conten).</span></span>

- <span data-ttu-id="c1f18-111">Изчакайте поне 24 часа след ръчно искане за обхождане и пълен повторен индекс, за да видите дали все още имате проблем.</span><span class="sxs-lookup"><span data-stu-id="c1f18-111">Wait at least 24 hours after manually requesting a crawl and full re-index to see if you're still experiencing an issue.</span></span> 

    <span data-ttu-id="c1f18-112">Ако са изминали повече от 24 часа от началото на обхождането и пълното повторно индексиране, моля, влезте в случай на поддръжка.</span><span class="sxs-lookup"><span data-stu-id="c1f18-112">If more than 24 hours have passed since you initiated the crawl and full re-index, please log a support case.</span></span> <span data-ttu-id="c1f18-113">В много случаи вече работим по решение.</span><span class="sxs-lookup"><span data-stu-id="c1f18-113">In many cases, we're already working on a solution.</span></span> <span data-ttu-id="c1f18-114">Моля, дайте ни поне 24 часа, за да завършим решение.</span><span class="sxs-lookup"><span data-stu-id="c1f18-114">Please give us at least 24 hours to complete a solution.</span></span>

> [!IMPORTANT]
> <span data-ttu-id="c1f18-115">Ако сайт, документ (библиотека) или списък е изтрит и все още се показва в резултатите от търсенето, потребителите трябва да получите **грешка 404 файл не е намерен** , когато се опитвате да получите достъп до него.</span><span class="sxs-lookup"><span data-stu-id="c1f18-115">If a site, document (library), or a list was deleted and still shows in the search results, users should receive an **Error 404 File Not Found** when trying to access it.</span></span> <span data-ttu-id="c1f18-116">Този проблем трябва да се регистрира като поддръжка случай за по-нататъшно разследване.</span><span class="sxs-lookup"><span data-stu-id="c1f18-116">This issue should be logged as a support case for further investigation.</span></span> 



