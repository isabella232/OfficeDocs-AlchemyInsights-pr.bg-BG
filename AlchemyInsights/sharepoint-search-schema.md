---
title: Управление на схемата на търсене в SharePoint Online
ms.author: efrene
author: efrene
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: fe00f4c0-44d5-49d4-9db0-a62698bcd1d1
ms.openlocfilehash: 704fb3b682d23220d61192e383d7d80f59f27933
ms.sourcegitcommit: 1d98db8acb9959aba3b5e308a567ade6b62da56c
ms.translationtype: MT
ms.contentlocale: bg-BG
ms.lasthandoff: 08/22/2019
ms.locfileid: "36502796"
---
# <a name="manage-search-schema-in-sharepoint-online"></a><span data-ttu-id="5738f-102">Управление на схемата на търсене в SharePoint Online</span><span class="sxs-lookup"><span data-stu-id="5738f-102">Manage search schema in SharePoint Online</span></span>

<span data-ttu-id="5738f-103">Схемата на търсене контролира какво потребителите могат да търсят, как потребителите могат да го търсят и как можете да представите резултатите за вашето търсене сайтове.</span><span class="sxs-lookup"><span data-stu-id="5738f-103">The search schema controls what users can search for, how users can search it, and how you can present the results on your search websites.</span></span> 

<span data-ttu-id="5738f-104">Вижте [управление на схемата на търсене в SharePoint Online](https://docs.microsoft.com/sharepoint/manage-search-schema) за да научите как да:</span><span class="sxs-lookup"><span data-stu-id="5738f-104">See [Manage the Search Schema in SharePoint Online](https://docs.microsoft.com/sharepoint/manage-search-schema) to learn how to:</span></span> 
- <span data-ttu-id="5738f-105">Промяна на схемата на търсене.</span><span class="sxs-lookup"><span data-stu-id="5738f-105">Change the search schema.</span></span>
- <span data-ttu-id="5738f-106">Създаване на контролирани свойства.</span><span class="sxs-lookup"><span data-stu-id="5738f-106">Create managed properties.</span></span>
- <span data-ttu-id="5738f-107">Карта обходени карта обходени свойства с контролирани свойства.</span><span class="sxs-lookup"><span data-stu-id="5738f-107">Map crawled map crawled properties to managed properties.</span></span>

<span data-ttu-id="5738f-108">Отбележете следното по отношение на управлението на вашето търсене схема:</span><span class="sxs-lookup"><span data-stu-id="5738f-108">Note the following in regards to managing your Search Schema:</span></span>

- <span data-ttu-id="5738f-109">Ако получите предупреждение посочва **приложението е пауза** когато схема промяна, това е само временно като има сервизно обслужване настъпили.</span><span class="sxs-lookup"><span data-stu-id="5738f-109">If you receive a warning stating **the application is paused** when making a schema change, this is only temporary as there is service maintenance occurring.</span></span> 

    <span data-ttu-id="5738f-110">Ако са минали повече от 24 часа и все още имате предупреждението, моля влезте подкрепа случай.</span><span class="sxs-lookup"><span data-stu-id="5738f-110">If more than 24 hours have passed and you still experience the warning, please log a support case.</span></span>
- <span data-ttu-id="5738f-111">Когато промените контролираните свойства или добавите нови, промените влязат в сила само след като съдържанието е било повторно обходени.</span><span class="sxs-lookup"><span data-stu-id="5738f-111">When you change managed properties or add new ones, the changes take effect only after the content has been re-crawled.</span></span> <span data-ttu-id="5738f-112">В SharePoint Online индексиране се случва автоматично на базата на графика на определени обхождане.</span><span class="sxs-lookup"><span data-stu-id="5738f-112">In SharePoint Online, crawling happens automatically based on the defined crawl schedule.</span></span>
- <span data-ttu-id="5738f-113">За да се уверите, че вашите промени са обходени, можете да специално [искане повторно индексиране на списъка или библиотеката](https://docs.microsoft.com/sharepoint/manage-search-schema#request-re-indexing-of-a-document-library-or-list)</span><span class="sxs-lookup"><span data-stu-id="5738f-113">To make sure that your changes are crawled, you can specifically [request a re-indexing of the list or library](https://docs.microsoft.com/sharepoint/manage-search-schema#request-re-indexing-of-a-document-library-or-list)</span></span> 

<span data-ttu-id="5738f-114">За пълен преглед на схемата на търсене вижте [Въвеждане на схемата за търсене](https://blogs.technet.microsoft.com/tothesharepoint/2012/11/25/introducing-search-schema-for-sharepoint-2013/)</span><span class="sxs-lookup"><span data-stu-id="5738f-114">For a complete overview of the Search Schema, see [Introducing Search Schema](https://blogs.technet.microsoft.com/tothesharepoint/2012/11/25/introducing-search-schema-for-sharepoint-2013/)</span></span> 


