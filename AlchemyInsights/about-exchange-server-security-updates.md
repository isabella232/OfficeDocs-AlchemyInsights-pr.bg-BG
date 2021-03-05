---
title: За актуализациите на защитата на Exchange Server
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 03/04/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9005482"
- "9005483"
- "9413"
- "9412"
ms.openlocfilehash: 87a5cf1ac4dfb96a5406f6b1431adb6ead074fd6
ms.sourcegitcommit: 6741a997fff871d263f92d3ff7fb61e7755956a9
ms.translationtype: MT
ms.contentlocale: bg-BG
ms.lasthandoff: 03/04/2021
ms.locfileid: "50480978"
---
# <a name="about-exchange-server-security-updates"></a><span data-ttu-id="58957-102">За актуализациите на защитата на Exchange Server</span><span class="sxs-lookup"><span data-stu-id="58957-102">About Exchange Server Security updates</span></span>

<span data-ttu-id="58957-103">Microsoft издаде поредица от критични актуализации на защитата за локален сървър на Exchange.</span><span class="sxs-lookup"><span data-stu-id="58957-103">Microsoft has released a series of critical security updates for Exchange Server on-premises.</span></span> <span data-ttu-id="58957-104">Засегнатите версии на сървъра са всяко ниво на актуализиране на Exchange Server 2010, 2013, 2016 и 2019.</span><span class="sxs-lookup"><span data-stu-id="58957-104">The affected server versions are any update levels of Exchange Server 2010, 2013, 2016 and 2019.</span></span> <span data-ttu-id="58957-105">Exchange Online не е повлиян, но ако имате някои локални сървъри на Exchange поради хибридна конфигурация, те са потенциално уязвими.</span><span class="sxs-lookup"><span data-stu-id="58957-105">Exchange Online is NOT impacted, but if you have some on-premises Exchange servers due to Hybrid configuration, they are potentially vulnerable.</span></span>

<span data-ttu-id="58957-106">За да актуализирате своите локални сървъри, ще трябва да се изпълняват поне следните версии на Exchange:</span><span class="sxs-lookup"><span data-stu-id="58957-106">To update your on-premises servers will have to be running at least the following versions of Exchange:</span></span>

- <span data-ttu-id="58957-107">Exchange 2010 Service Pack 3</span><span class="sxs-lookup"><span data-stu-id="58957-107">Exchange 2010 Service Pack 3</span></span>
- <span data-ttu-id="58957-108">Exchange Server 2013 CU 23</span><span class="sxs-lookup"><span data-stu-id="58957-108">Exchange Server 2013 CU 23</span></span>
- <span data-ttu-id="58957-109">Exchange Server 2016 CU 19 или CU 18</span><span class="sxs-lookup"><span data-stu-id="58957-109">Exchange Server 2016 CU 19 or CU 18</span></span>
- <span data-ttu-id="58957-110">Exchange Server 2019 CU 8 или CU 7</span><span class="sxs-lookup"><span data-stu-id="58957-110">Exchange Server 2019 CU 8 or CU 7</span></span>

<span data-ttu-id="58957-111">Вижте следното съобщение за местоположението на корекциите: [издадено: актуализации на защитата за 2021 на Exchange Server](https://techcommunity.microsoft.com/t5/exchange-team-blog/released-march-2021-exchange-server-security-updates/ba-p/2175901)</span><span class="sxs-lookup"><span data-stu-id="58957-111">Please see the following announcement for location of fixes: [Released: March 2021 Exchange Server Security Updates](https://techcommunity.microsoft.com/t5/exchange-team-blog/released-march-2021-exchange-server-security-updates/ba-p/2175901)</span></span>

<span data-ttu-id="58957-112">**Важни бележки:**</span><span class="sxs-lookup"><span data-stu-id="58957-112">**Important notes:**</span></span>

<span data-ttu-id="58957-113">Инсталирането на актуализациите няма да работи, ако вашите локални сървъри не изпълняват задължителни версии на Exchange, както е посочено в списъка по-горе.</span><span class="sxs-lookup"><span data-stu-id="58957-113">Installation of updates will not work if your on-premises servers are not running required Exchange versions, as per the above list.</span></span>

<span data-ttu-id="58957-114">Ако ръчно инсталиране на актуализации, моля, прочетете секцията "известни проблеми" за актуализиране на статиите от БЗ за важна информация.</span><span class="sxs-lookup"><span data-stu-id="58957-114">If installing updates manually, please read the "Known issues" section of update KB articles for important information.</span></span> <span data-ttu-id="58957-115">Актуализациите на защитата трябва да се стартират от подкана на "повишена CMD/PowerShell"!</span><span class="sxs-lookup"><span data-stu-id="58957-115">Security updates MUST be run from elevated CMD/PowerShell prompt!</span></span>
