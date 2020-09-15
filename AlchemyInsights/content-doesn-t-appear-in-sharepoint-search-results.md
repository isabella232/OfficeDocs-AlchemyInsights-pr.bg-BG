---
title: Съдържание не се появява в резултатите от търсенето в SharePoint
ms.author: tlarsen
author: tklarsen
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "750"
- "5300017"
ms.assetid: 693db84f-2737-4c21-b027-4ab3d121b4a8
ms.openlocfilehash: a57711434d653f5d5667776916c9251bba2370e6
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: bg-BG
ms.lasthandoff: 09/14/2020
ms.locfileid: "47713119"
---
# <a name="content-doesnt-appear-in-sharepoint-search-results"></a><span data-ttu-id="6ece4-102">Съдържание не се появява в резултатите от търсенето в SharePoint</span><span class="sxs-lookup"><span data-stu-id="6ece4-102">Content doesn't appear in SharePoint search results</span></span>

<span data-ttu-id="6ece4-103">Следвайте тези стъпки за отстраняване на неизправности, когато очакваното съдържание не се появява в резултатите от търсенето:</span><span class="sxs-lookup"><span data-stu-id="6ece4-103">Follow these troubleshooting steps when expected content doesn't appear in search results:</span></span>
  
1. <span data-ttu-id="6ece4-104">Проверете дали **сайтът** , съдържащ очакваното съдържание, е настроен да позволява съдържание, което да се показва в резултатите от търсенето.</span><span class="sxs-lookup"><span data-stu-id="6ece4-104">Check that the **site** that contains the expected content is set to allow content to appear in search results.</span></span> <span data-ttu-id="6ece4-105">Следвайте стъпките в [Показване на съдържание на сайт в резултатите от търсенето](https://docs.microsoft.com/sharepoint/make-site-content-searchable#show-content-on-a-site-in-search-results).</span><span class="sxs-lookup"><span data-stu-id="6ece4-105">Follow the steps in [Show content on a site in search results](https://docs.microsoft.com/sharepoint/make-site-content-searchable#show-content-on-a-site-in-search-results).</span></span>

2. <span data-ttu-id="6ece4-106">Проверете дали **списъкът** или **библиотеката** , съдържащи очакваното съдържание, са зададени така, че да позволява съдържание да се показва в резултатите от търсенето.</span><span class="sxs-lookup"><span data-stu-id="6ece4-106">Check that the **list** or **library** that contains the expected content is set to allow content to appear in search results.</span></span> <span data-ttu-id="6ece4-107">Следвайте стъпките в [Показване на съдържание от списъци или библиотеки в резултатите от търсенето](https://docs.microsoft.com/sharepoint/make-site-content-searchable#show-content-from-lists-or-libraries-in-search-results).</span><span class="sxs-lookup"><span data-stu-id="6ece4-107">Follow the steps in [Show content from lists or libraries in search results](https://docs.microsoft.com/sharepoint/make-site-content-searchable#show-content-from-lists-or-libraries-in-search-results).</span></span>

3. <span data-ttu-id="6ece4-108">Уверете се, че оформлението на страницата, документа или страницата по избор се публикува като **главна версия.**</span><span class="sxs-lookup"><span data-stu-id="6ece4-108">Verify that the page, document, or custom page layout is published as a **Major version.**</span></span> <span data-ttu-id="6ece4-109">Следвайте стъпка 3 в [търсенето не връща всички резултати в SharePoint online](https://go.microsoft.com/fwlink/?linkid=874525).</span><span class="sxs-lookup"><span data-stu-id="6ece4-109">Follow step 3 in [Search doesn't return all results in SharePoint Online](https://go.microsoft.com/fwlink/?linkid=874525).</span></span>

4. <span data-ttu-id="6ece4-110">Проверете дали потребителят има **разрешения** да преглежда съдържанието.</span><span class="sxs-lookup"><span data-stu-id="6ece4-110">Verify that the user has **permissions** to view the content.</span></span> <span data-ttu-id="6ece4-111">Следвайте стъпките в [запознаване с нивата на разрешение в SharePoint](https://docs.microsoft.com/sharepoint/understanding-permission-levels).</span><span class="sxs-lookup"><span data-stu-id="6ece4-111">Follow the steps in [Understanding permission levels in SharePoint](https://docs.microsoft.com/sharepoint/understanding-permission-levels).</span></span>
    
5. <span data-ttu-id="6ece4-112">Ако схемата на търсене е променена, като сте добавили ново контролирано свойство чрез редактиране на контролирано свойство или чрез премахване на контролирано свойство, е необходимо да поискате обхождане и повторно индексиране.</span><span class="sxs-lookup"><span data-stu-id="6ece4-112">If the search schema has been changed by adding a new managed property, by editing a managed property, or by removing a managed property then requesting a crawl and re-index will be required.</span></span> <span data-ttu-id="6ece4-113">**Повторно индексиране** на съдържанието, като следвате стъпките в [ръчна заявка обхождане и повторно индексиране на сайт, библиотека или списък](https://docs.microsoft.com/sharepoint/crawl-site-content).</span><span class="sxs-lookup"><span data-stu-id="6ece4-113">**Re-index** the content by following the steps in [Manually request crawling and re-indexing of a site, a library or a list](https://docs.microsoft.com/sharepoint/crawl-site-content).</span></span> <span data-ttu-id="6ece4-114">Това може да отнеме известно време, изчакайте 24 часа, преди да проверите резултатите отново.</span><span class="sxs-lookup"><span data-stu-id="6ece4-114">This might take a while, wait 24 hours before checking the results again.</span></span>

<span data-ttu-id="6ece4-115">За повече информация вижте [Разрешаване на съдържание на сайт, за да може да се търси](https://docs.microsoft.com/sharepoint/make-site-content-searchable).</span><span class="sxs-lookup"><span data-stu-id="6ece4-115">For more information, see [Enable content on a site to be searchable](https://docs.microsoft.com/sharepoint/make-site-content-searchable).</span></span> 
  
