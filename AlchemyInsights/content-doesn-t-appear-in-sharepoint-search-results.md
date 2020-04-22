---
title: Съдържанието не се показва в резултатите от търсенето на SharePoint
ms.author: tlarsen
author: tklarsen
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "750"
- "5300017"
ms.assetid: 693db84f-2737-4c21-b027-4ab3d121b4a8
ms.openlocfilehash: a21e0047b41390f740f9e13d31cba32b13990151
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: bg-BG
ms.lasthandoff: 04/22/2020
ms.locfileid: "43705650"
---
# <a name="content-doesnt-appear-in-sharepoint-search-results"></a><span data-ttu-id="ec311-102">Съдържанието не се показва в резултатите от търсенето на SharePoint</span><span class="sxs-lookup"><span data-stu-id="ec311-102">Content doesn't appear in SharePoint search results</span></span>

<span data-ttu-id="ec311-103">Следвайте тези стъпки за отстраняване на неизправности, когато очакваното съдържание не се показва в резултатите от търсенето:</span><span class="sxs-lookup"><span data-stu-id="ec311-103">Follow these troubleshooting steps when expected content doesn't appear in search results:</span></span>
  
1. <span data-ttu-id="ec311-104">Проверете дали **сайтът,** който съдържа очакваното съдържание, е настроен да позволява съдържанието да се показва в резултатите от търсенето.</span><span class="sxs-lookup"><span data-stu-id="ec311-104">Check that the **site** that contains the expected content is set to allow content to appear in search results.</span></span> <span data-ttu-id="ec311-105">Следвайте стъпките в [Показване на съдържание на сайт в резултатите от търсенето](https://docs.microsoft.com/sharepoint/make-site-content-searchable#show-content-on-a-site-in-search-results).</span><span class="sxs-lookup"><span data-stu-id="ec311-105">Follow the steps in [Show content on a site in search results](https://docs.microsoft.com/sharepoint/make-site-content-searchable#show-content-on-a-site-in-search-results).</span></span>

2. <span data-ttu-id="ec311-106">Проверете дали **списъкът** или **библиотеката,** които съдържат очакваното съдържание, е настроен да разрешава показването на съдържание в резултатите от търсенето.</span><span class="sxs-lookup"><span data-stu-id="ec311-106">Check that the **list** or **library** that contains the expected content is set to allow content to appear in search results.</span></span> <span data-ttu-id="ec311-107">Следвайте стъпките в [Показване на съдържание от списъци или библиотеки в резултатите от търсенето](https://docs.microsoft.com/sharepoint/make-site-content-searchable#show-content-from-lists-or-libraries-in-search-results).</span><span class="sxs-lookup"><span data-stu-id="ec311-107">Follow the steps in [Show content from lists or libraries in search results](https://docs.microsoft.com/sharepoint/make-site-content-searchable#show-content-from-lists-or-libraries-in-search-results).</span></span>

3. <span data-ttu-id="ec311-108">Проверете дали оформлението на страницата, документа или персонализираното оформление на страницата е публикувано като **основна версия.**</span><span class="sxs-lookup"><span data-stu-id="ec311-108">Verify that the page, document, or custom page layout is published as a **Major version.**</span></span> <span data-ttu-id="ec311-109">Следвайте стъпка 3 в [търсене не връща всички резултати в SharePoint Online](https://go.microsoft.com/fwlink/?linkid=874525).</span><span class="sxs-lookup"><span data-stu-id="ec311-109">Follow step 3 in [Search doesn't return all results in SharePoint Online](https://go.microsoft.com/fwlink/?linkid=874525).</span></span>

4. <span data-ttu-id="ec311-110">Проверете дали потребителят има **разрешения** да преглежда съдържанието.</span><span class="sxs-lookup"><span data-stu-id="ec311-110">Verify that the user has **permissions** to view the content.</span></span> <span data-ttu-id="ec311-111">Следвайте стъпките в [Разбиране на нивата на разрешение в SharePoint](https://docs.microsoft.com/sharepoint/understanding-permission-levels).</span><span class="sxs-lookup"><span data-stu-id="ec311-111">Follow the steps in [Understanding permission levels in SharePoint](https://docs.microsoft.com/sharepoint/understanding-permission-levels).</span></span>
    
5. <span data-ttu-id="ec311-112">Ако схемата на търсене е променена чрез добавяне на ново контролирано свойство, чрез редактиране на контролирано свойство или чрез премахване на контролирано свойство, тогава ще се изисква обхождане и повторно индексиране.</span><span class="sxs-lookup"><span data-stu-id="ec311-112">If the search schema has been changed by adding a new managed property, by editing a managed property, or by removing a managed property then requesting a crawl and re-index will be required.</span></span> <span data-ttu-id="ec311-113">**Индексирайте повторно** съдържанието, като следвате стъпките в [Ръчно поискате обхождане и повторно индексиране на сайт, библиотека или списък](https://docs.microsoft.com/sharepoint/crawl-site-content).</span><span class="sxs-lookup"><span data-stu-id="ec311-113">**Re-index** the content by following the steps in [Manually request crawling and re-indexing of a site, a library or a list](https://docs.microsoft.com/sharepoint/crawl-site-content).</span></span> <span data-ttu-id="ec311-114">Това може да отнеме известно време, изчакайте 24 часа, преди да проверите резултатите отново.</span><span class="sxs-lookup"><span data-stu-id="ec311-114">This might take a while, wait 24 hours before checking the results again.</span></span>

<span data-ttu-id="ec311-115">За повече информация вижте [Разрешаване на съдържание на сайт, за да може да се търси](https://docs.microsoft.com/sharepoint/make-site-content-searchable).</span><span class="sxs-lookup"><span data-stu-id="ec311-115">For more information, see [Enable content on a site to be searchable](https://docs.microsoft.com/sharepoint/make-site-content-searchable).</span></span> 
  
