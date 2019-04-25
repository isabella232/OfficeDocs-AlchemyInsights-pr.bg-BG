---
title: Актуализиране на DNS записи да си сайт с настоящия си хостинг доставчик
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 5/2/2018
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: 48251355-7383-4fdc-a1e1-9dc2c85a8d29
ms.openlocfilehash: f2cdb319e56b82c09b7a9856c81a45e69dee6759
ms.sourcegitcommit: 9d78905c512192ffc4675468abd2efc5f2e4baf4
ms.translationtype: MT
ms.contentlocale: bg-BG
ms.lasthandoff: 04/23/2019
ms.locfileid: "32423712"
---
# <a name="update-dns-records-to-keep-your-website-with-your-current-hosting-provider"></a><span data-ttu-id="77b71-102">Актуализиране на DNS записи да си сайт с настоящия си хостинг доставчик</span><span class="sxs-lookup"><span data-stu-id="77b71-102">Update DNS records to keep your website with your current hosting provider</span></span>

1. <span data-ttu-id="77b71-103">Страницата на [домейни](https://portal.office.com/adminportal/home#/Domains) изберете в списъка на домейни, домейн, което използвате за вашия уеб сайт и след това изберете **DNS настройките** в прозореца управление на.</span><span class="sxs-lookup"><span data-stu-id="77b71-103">On the [Domains](https://portal.office.com/adminportal/home#/Domains) page, in the list of domains, select the domain you're using for your website, and then select **DNS settings** in the management pane.</span></span> 
    
2. <span data-ttu-id="77b71-104">Изберете **+ нов потребителски запис** и въведете следното:</span><span class="sxs-lookup"><span data-stu-id="77b71-104">Select **+ New custom record** and enter the following:</span></span> 
    
  - <span data-ttu-id="77b71-105">За **DNS тип** въведете: **(адрес)**</span><span class="sxs-lookup"><span data-stu-id="77b71-105">For **DNS type** enter: **A (Address)**</span></span>
    
  - <span data-ttu-id="77b71-106">За **име на хост или псевдоним**въведете следното:**@**</span><span class="sxs-lookup"><span data-stu-id="77b71-106">For **Host name or Alias**, type the following: **@**</span></span>
    
  - <span data-ttu-id="77b71-107">За **IP адрес**въведете статичен IP адрес за вашия сайт, където той в момента е домакин (например 172.16.140.1).</span><span class="sxs-lookup"><span data-stu-id="77b71-107">For **IP Address**, type the static IP address for your website where it's currently hosted (for example, 172.16.140.1).</span></span> 
    
    <span data-ttu-id="77b71-108">Това трябва да бъде *статичен* IP адрес на сайта, не *динамичен* IP адрес.</span><span class="sxs-lookup"><span data-stu-id="77b71-108">This must be a  *static*  IP address for the website, not a  *dynamic*  IP address.</span></span> <span data-ttu-id="77b71-109">Проверете сайта, където е домакин вашия сайт да се уверите, можете да получите на статичен IP адрес за вашия публичен уеб сайт.</span><span class="sxs-lookup"><span data-stu-id="77b71-109">Check with site where your website is hosted to make sure you can get a static IP address for your public website.</span></span> 
    
3. <span data-ttu-id="77b71-110">Изберете **Запиши**.</span><span class="sxs-lookup"><span data-stu-id="77b71-110">Select **Save**.</span></span> 
    
<span data-ttu-id="77b71-111">В допълнение можете да създадете CNAME запис да помогне на клиентите намерите вашия уебсайт.</span><span class="sxs-lookup"><span data-stu-id="77b71-111">In addition, you can create a CNAME record to help customers find your website.</span></span>
  
1. <span data-ttu-id="77b71-112">Изберете **+ нов потребителски запис** и въведете следното:</span><span class="sxs-lookup"><span data-stu-id="77b71-112">Select **+ New custom record** and enter the following:</span></span> 
    
  - <span data-ttu-id="77b71-113">За **DNS тип** въведете: **CNAME (псевдоним)**</span><span class="sxs-lookup"><span data-stu-id="77b71-113">For **DNS type** enter: **CNAME (Alias)**</span></span>
    
  - <span data-ttu-id="77b71-114">За **име на хост или псевдоним**, въведете следното: **www**</span><span class="sxs-lookup"><span data-stu-id="77b71-114">For **Host name or Alias**, type the following: **www**</span></span>
    
  - <span data-ttu-id="77b71-115">За **пункта до адрес**въведете пълното домейн име (FQDN) за вашия уеб сайт (например contoso.com).</span><span class="sxs-lookup"><span data-stu-id="77b71-115">For **Points to address**, type the fully qualified domain name (FQDN) for your website (for example, contoso.com).</span></span> 
    
2. <span data-ttu-id="77b71-116">Изберете **Запиши**.</span><span class="sxs-lookup"><span data-stu-id="77b71-116">Select **Save**.</span></span> 
    

