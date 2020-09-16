---
title: Проблеми с производителността – SharePoint или OneDrive
ms.author: pebaum
author: pebaum
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1133"
- "2397"
- "2418"
- "5200018"
ms.assetid: 9225ec0f-771f-4d7a-8157-e188953107aa
ms.openlocfilehash: 28867b71df5353dcee5cc3361742f10357a0efe1
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: bg-BG
ms.lasthandoff: 09/15/2020
ms.locfileid: "47771890"
---
# <a name="sharepoint-or-onedrive-slow-inaccessible-or-unavailable-for-multiple-users"></a><span data-ttu-id="81bf9-102">SharePoint или OneDrive – бавен, недостъпен или недостъпен за множество потребители</span><span class="sxs-lookup"><span data-stu-id="81bf9-102">SharePoint or OneDrive slow, inaccessible, or unavailable for multiple users</span></span>

<span data-ttu-id="81bf9-103">SharePoint или OneDrive може да е бавен, недостъпен или недостъпен или може да показва услугата недостъпни или 503 грешки по няколко причини:</span><span class="sxs-lookup"><span data-stu-id="81bf9-103">SharePoint or OneDrive may be slow, inaccessible, or unavailable, or may display service unavailable or 503 errors, for several reasons:</span></span>
  
- <span data-ttu-id="81bf9-104">Ако вашият сайт на SharePoint или OneDrive е бавен или забавен за много потребители, е възможно да има проблем с временните услуги, в който потребителите да получават периодични закъснения или грешки при навигация при достъп до сайтове на SharePoint или съдържание на OneDrive.</span><span class="sxs-lookup"><span data-stu-id="81bf9-104">If your SharePoint or OneDrive site is slow or delayed for multiple users, there may be a temporary service issue where users experience intermittent delays or navigation errors when accessing SharePoint sites or OneDrive content.</span></span> <span data-ttu-id="81bf9-105">Проверете [таблото за изправност на услугите](https://admin.microsoft.com/AdminPortal/Home#/servicehealth) , за да видите дали вашата организация е засегната.</span><span class="sxs-lookup"><span data-stu-id="81bf9-105">Check the [Service health dashboard](https://admin.microsoft.com/AdminPortal/Home#/servicehealth) to see if your organization is impacted.</span></span>
  
- <span data-ttu-id="81bf9-106">Потребителят може да получи съобщение за грешка, че *сървърът на 503 е зает* при опит за навигиране до сайтове на SharePoint или OneDrive.</span><span class="sxs-lookup"><span data-stu-id="81bf9-106">Users may receive a *503 server is busy* error when attempting to navigate to SharePoint or OneDrive sites.</span></span> <span data-ttu-id="81bf9-107">Тази грешка може да се дължи на ограничаване в рамките на услугата на SharePoint.</span><span class="sxs-lookup"><span data-stu-id="81bf9-107">This error can be caused by throttling within the SharePoint service.</span></span> <span data-ttu-id="81bf9-108">SharePoint Online използва регулиране, за да поддържа оптимална производителност и надеждност на услугата SharePoint Online.</span><span class="sxs-lookup"><span data-stu-id="81bf9-108">SharePoint Online uses throttling to maintain optimal performance and reliability of the SharePoint Online service.</span></span> <span data-ttu-id="81bf9-109">Регулирането ограничава броя на действията на потребителите или едновременните повиквания (по скрипт или код), за да се предотврати прекомерната употреба на ресурси.</span><span class="sxs-lookup"><span data-stu-id="81bf9-109">Throttling limits the number of user actions or concurrent calls (by script or code) to prevent overuse of resources.</span></span> <span data-ttu-id="81bf9-110">За повече информация относно ограничаването на скоростта вижте [избягване на ограничаването или блокирането в SharePoint online](https://docs.microsoft.com/sharepoint/dev/general-development/how-to-avoid-getting-throttled-or-blocked-in-sharepoint-online).</span><span class="sxs-lookup"><span data-stu-id="81bf9-110">For more information on throttling see, [Avoid getting throttled or blocked in SharePoint Online](https://docs.microsoft.com/sharepoint/dev/general-development/how-to-avoid-getting-throttled-or-blocked-in-sharepoint-online).</span></span>

- <span data-ttu-id="81bf9-111">Ако имате ниска производителност с **класически** или **модерен** сайт на SharePoint или страница, използвайте инструмента за [диагностика](https://aka.ms/perftool) на страници, за да анализирате страниците.</span><span class="sxs-lookup"><span data-stu-id="81bf9-111">If you experience slow performance with a **classic** or **modern** SharePoint site or page, utilize the [Page Diagnostic tool](https://aka.ms/perftool) to analyze the pages.</span></span>
  
- <span data-ttu-id="81bf9-112">Ако все още имате общи бавни резултати, прегледайте ресурсите в долната част на тази статия: [Въведение в настройката на производителността за SharePoint online](https://go.microsoft.com/fwlink/?linkid=2024334)</span><span class="sxs-lookup"><span data-stu-id="81bf9-112">If you still experience general slow performance, please review the resources at the bottom of this article: [Introduction to performance tuning for SharePoint Online](https://go.microsoft.com/fwlink/?linkid=2024334)</span></span>
  