---
title: Диаграма показва различен брой записи в мрежата
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/24/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "5611"
- "9002930"
ms.openlocfilehash: 3d0be28c783bb129d05484565c6c2a56ac5e0acf
ms.sourcegitcommit: b10cea11b4975354b91193327b58aa4740d34833
ms.translationtype: MT
ms.contentlocale: bg-BG
ms.lasthandoff: 07/28/2020
ms.locfileid: "45438757"
---
# <a name="chart-shows-different-number-of-records-in-grid"></a><span data-ttu-id="fe682-102">Диаграма показва различен брой записи в мрежата</span><span class="sxs-lookup"><span data-stu-id="fe682-102">Chart shows different number of records in grid</span></span>

<span data-ttu-id="fe682-103">**Симптом**</span><span class="sxs-lookup"><span data-stu-id="fe682-103">**Symptom**</span></span>

<span data-ttu-id="fe682-104">За диаграма на таблото страница, когато щракнете върху диаграма "..." и щракнете върху "Преглед на записи", можете да навигирате до мрежата страница, за да видите всички записи. Понякога броят на записите се променя.</span><span class="sxs-lookup"><span data-stu-id="fe682-104">For chart on dashboard page, when you click on chart "…" and click "View records", you navigate to grid page to see all the records.Sometimes, the number of records changes.</span></span>

<span data-ttu-id="fe682-105">**Причина**</span><span class="sxs-lookup"><span data-stu-id="fe682-105">**Cause**</span></span>

<span data-ttu-id="fe682-106">Това се дължи на разликата между изгледите между диаграмата на оригиналната страница на таблото и диаграмата на началната страница на мрежата.</span><span class="sxs-lookup"><span data-stu-id="fe682-106">This is due to the difference of views between the chart on the original dashboard page and the chart on the grid home page.</span></span>  

<span data-ttu-id="fe682-107">**Решение**</span><span class="sxs-lookup"><span data-stu-id="fe682-107">**Solution**</span></span>

1. <span data-ttu-id="fe682-108">Проверете изгледа от оригиналната страница и изгледа в мрежата, за да видите дали са различни.</span><span class="sxs-lookup"><span data-stu-id="fe682-108">Check the view from the original page and the view in the grid to see if they are different.</span></span>
2. <span data-ttu-id="fe682-109">Променете изгледа в мрежата, за да съответства на изгледа в оригиналната страница.</span><span class="sxs-lookup"><span data-stu-id="fe682-109">Change the view in grid to match the view in the original page.</span></span>
3. <span data-ttu-id="fe682-110">Ако не може да бъде намерен правилния изглед, обикновено това означава, че изгледът не е разрешен в разработчик на приложения.</span><span class="sxs-lookup"><span data-stu-id="fe682-110">If the correct view cannot be found, usually it means the view is not enabled in app designer.</span></span>
4. <span data-ttu-id="fe682-111">Отидете на разработчик на приложения на конкретното приложение, изберете обекта и неговите изгледи, проверете изгледа, който искате да активирате, запишете, публикувате и затворите.</span><span class="sxs-lookup"><span data-stu-id="fe682-111">Go to app designer of the specific app, choose the entity and its views, check the view you want to enable, save, publish and close.</span></span>
5. <span data-ttu-id="fe682-112">Обновете страницата.</span><span class="sxs-lookup"><span data-stu-id="fe682-112">Refresh the page.</span></span>