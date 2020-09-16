---
title: Управление на схемата на търсене в SharePoint online
ms.author: pebaum
author: pebaum
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: fe00f4c0-44d5-49d4-9db0-a62698bcd1d1
ms.openlocfilehash: f2d8d3e07fe32d21af484e4c59e0f5ac6fe8081c
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: bg-BG
ms.lasthandoff: 09/15/2020
ms.locfileid: "47770540"
---
# <a name="manage-search-schema-in-sharepoint-online"></a><span data-ttu-id="431d8-102">Управление на схемата на търсене в SharePoint online</span><span class="sxs-lookup"><span data-stu-id="431d8-102">Manage search schema in SharePoint Online</span></span>

<span data-ttu-id="431d8-103">Схемата на търсене управлява това, което потребителите могат да търсят, как потребителите могат да я търсят и как можете да представите резултатите на уеб сайтовете си за търсене.</span><span class="sxs-lookup"><span data-stu-id="431d8-103">The search schema controls what users can search for, how users can search it, and how you can present the results on your search websites.</span></span> 

<span data-ttu-id="431d8-104">Вижте [управление на схемата на търсене в SharePoint Online,](https://docs.microsoft.com/sharepoint/manage-search-schema) за да научите как да направите следното:</span><span class="sxs-lookup"><span data-stu-id="431d8-104">See [Manage the Search Schema in SharePoint Online](https://docs.microsoft.com/sharepoint/manage-search-schema) to learn how to:</span></span> 
- <span data-ttu-id="431d8-105">Промяна на схемата на търсене.</span><span class="sxs-lookup"><span data-stu-id="431d8-105">Change the search schema.</span></span>
- <span data-ttu-id="431d8-106">Създайте контролирани свойства.</span><span class="sxs-lookup"><span data-stu-id="431d8-106">Create managed properties.</span></span>
- <span data-ttu-id="431d8-107">Нанесена карта обходени свойства с контролирани свойства.</span><span class="sxs-lookup"><span data-stu-id="431d8-107">Map crawled map crawled properties to managed properties.</span></span>

<span data-ttu-id="431d8-108">Обърнете внимание на следното по отношение на управлението на вашата схема на търсене:</span><span class="sxs-lookup"><span data-stu-id="431d8-108">Note the following in regards to managing your Search Schema:</span></span>

- <span data-ttu-id="431d8-109">Ако получите предупреждение, че **приложението е на пауза** при промяна на схемата, това е само временно, тъй като има поддръжка за услуги.</span><span class="sxs-lookup"><span data-stu-id="431d8-109">If you receive a warning stating **the application is paused** when making a schema change, this is only temporary as there is service maintenance occurring.</span></span> 

    <span data-ttu-id="431d8-110">Ако са изминали повече от 24 часа и все още имате предупреждение, моля, влезте по казус за поддръжка.</span><span class="sxs-lookup"><span data-stu-id="431d8-110">If more than 24 hours have passed and you still experience the warning, please log a support case.</span></span>
- <span data-ttu-id="431d8-111">Когато промените контролирани свойства или добавите нови, промените ще влязат в сила само след като съдържанието е било повторно обходено.</span><span class="sxs-lookup"><span data-stu-id="431d8-111">When you change managed properties or add new ones, the changes take effect only after the content has been re-crawled.</span></span> <span data-ttu-id="431d8-112">В SharePoint online обхождането се извършва автоматично на базата на дефиниран график за обхождане.</span><span class="sxs-lookup"><span data-stu-id="431d8-112">In SharePoint Online, crawling happens automatically based on the defined crawl schedule.</span></span>
- <span data-ttu-id="431d8-113">За да се уверите, че вашите промени са обходени, можете конкретно да [поискате повторно индексиране на списъка или библиотеката](https://docs.microsoft.com/sharepoint/manage-search-schema#request-re-indexing-of-a-document-library-or-list)</span><span class="sxs-lookup"><span data-stu-id="431d8-113">To make sure that your changes are crawled, you can specifically [request a re-indexing of the list or library](https://docs.microsoft.com/sharepoint/manage-search-schema#request-re-indexing-of-a-document-library-or-list)</span></span> 

<span data-ttu-id="431d8-114">За пълен преглед на схемата на търсене вижте Въведение в [схемата на търсене](https://blogs.technet.microsoft.com/tothesharepoint/2012/11/25/introducing-search-schema-for-sharepoint-2013/)</span><span class="sxs-lookup"><span data-stu-id="431d8-114">For a complete overview of the Search Schema, see [Introducing Search Schema](https://blogs.technet.microsoft.com/tothesharepoint/2012/11/25/introducing-search-schema-for-sharepoint-2013/)</span></span> 


