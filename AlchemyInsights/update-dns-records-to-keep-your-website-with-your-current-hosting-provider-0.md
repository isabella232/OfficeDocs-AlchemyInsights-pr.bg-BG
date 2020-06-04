---
title: Актуализиране на DNS записи, за да запазите вашия уеб сайт с вашия текущ хостинг доставчик
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "42"
- "43"
- "100002"
ms.assetid: 48251355-7383-4fdc-a1e1-9dc2c85a8d29
ms.openlocfilehash: 7bd36c3954d12d3ee4ac624a2f827d8e5cd88082
ms.sourcegitcommit: bc7d6f4f3c9f7060d073f5130e1ec856e248d020
ms.translationtype: MT
ms.contentlocale: bg-BG
ms.lasthandoff: 06/02/2020
ms.locfileid: "36665749"
---
# <a name="update-dns-records-to-keep-your-website-with-your-current-hosting-provider"></a><span data-ttu-id="5ccb2-102">Актуализиране на DNS записи, за да запазите вашия уеб сайт с вашия текущ хостинг доставчик</span><span class="sxs-lookup"><span data-stu-id="5ccb2-102">Update DNS records to keep your website with your current hosting provider</span></span>

1. <span data-ttu-id="5ccb2-103">В центъра за администриране на Microsoft 365 отидете на **страницата за инсталиране**на  >  [домейни](https://portal.office.com/adminportal/home#/Domains) и в списъка с домейни изберете домейна, който използвате за вашия уеб сайт.</span><span class="sxs-lookup"><span data-stu-id="5ccb2-103">In the Microsoft 365 admin center, go to the **Setup** > [Domains](https://portal.office.com/adminportal/home#/Domains) page, and in the list of domains, select the domain you're using for your website.</span></span>

2. <span data-ttu-id="5ccb2-104">Изберете **+ Нов потребителски запис** и въведете следното:</span><span class="sxs-lookup"><span data-stu-id="5ccb2-104">Select **+ New custom record** and enter the following:</span></span>

  - <span data-ttu-id="5ccb2-105">За **DNS тип** въведете: A **(адрес)**</span><span class="sxs-lookup"><span data-stu-id="5ccb2-105">For **DNS type** enter: **A (Address)**</span></span>

  - <span data-ttu-id="5ccb2-106">За **име на хост или псевдоним**въведете следното:**@**</span><span class="sxs-lookup"><span data-stu-id="5ccb2-106">For **Host name or Alias**, type the following: **@**</span></span>

  - <span data-ttu-id="5ccb2-107">За **IP адрес**въведете статичния IP адрес за вашия уеб сайт, където се хоства (например 172.16.140.1).</span><span class="sxs-lookup"><span data-stu-id="5ccb2-107">For **IP Address**, type the static IP address for your website where it's currently hosted (for example, 172.16.140.1).</span></span>

    <span data-ttu-id="5ccb2-108">Това трябва да е *статичен* IP адрес за уеб сайта, а не *динамичен* IP адрес.</span><span class="sxs-lookup"><span data-stu-id="5ccb2-108">This must be a  *static*  IP address for the website, not a  *dynamic*  IP address.</span></span> <span data-ttu-id="5ccb2-109">Проверете на сайта, където се хоства уебсайтът Ви, за да сте сигурни, че можете да получите статичен IP адрес за публичния си уебсайт.</span><span class="sxs-lookup"><span data-stu-id="5ccb2-109">Check with site where your website is hosted to make sure you can get a static IP address for your public website.</span></span>

3. <span data-ttu-id="5ccb2-110">Изберете **Записване**.</span><span class="sxs-lookup"><span data-stu-id="5ccb2-110">Select **Save**.</span></span>

<span data-ttu-id="5ccb2-111">Освен това можете да създадете CNAME запис, който да помогне на клиентите да намерят уебсайта ви.</span><span class="sxs-lookup"><span data-stu-id="5ccb2-111">In addition, you can create a CNAME record to help customers find your website.</span></span>
  
1. <span data-ttu-id="5ccb2-112">Изберете **+ Нов потребителски запис** и въведете следното:</span><span class="sxs-lookup"><span data-stu-id="5ccb2-112">Select **+ New custom record** and enter the following:</span></span>

  - <span data-ttu-id="5ccb2-113">За **DNS тип** въведете: **CNAME (псевдоним)**</span><span class="sxs-lookup"><span data-stu-id="5ccb2-113">For **DNS type** enter: **CNAME (Alias)**</span></span>

  - <span data-ttu-id="5ccb2-114">За **име на хост или псевдоним**въведете следното: **www**</span><span class="sxs-lookup"><span data-stu-id="5ccb2-114">For **Host name or Alias**, type the following: **www**</span></span>

  - <span data-ttu-id="5ccb2-115">За **точки за адрес**въведете пълното име на домейн (FQDN) за вашия уебсайт (например contoso.com).</span><span class="sxs-lookup"><span data-stu-id="5ccb2-115">For **Points to address**, type the fully qualified domain name (FQDN) for your website (for example, contoso.com).</span></span>

2. <span data-ttu-id="5ccb2-116">Изберете **Записване**.</span><span class="sxs-lookup"><span data-stu-id="5ccb2-116">Select **Save**.</span></span>
