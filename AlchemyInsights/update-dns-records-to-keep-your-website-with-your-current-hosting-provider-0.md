---
title: Актуализиране на DNS записи, за да запазите вашия уеб сайт при вашия текущ доставчик на хостинг
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "42"
- "43"
- "100002"
ms.assetid: 48251355-7383-4fdc-a1e1-9dc2c85a8d29
ms.openlocfilehash: 1d8654bc2dfb9063d0203992d624285eb646027d
ms.sourcegitcommit: 78939b01579b626b147d356045a37aec1170c948
ms.translationtype: MT
ms.contentlocale: bg-BG
ms.lasthandoff: 09/15/2020
ms.locfileid: "47815774"
---
# <a name="update-dns-records-to-keep-your-website-with-your-current-hosting-provider"></a><span data-ttu-id="0bc1f-102">Актуализиране на DNS записи, за да запазите вашия уеб сайт при вашия текущ доставчик на хостинг</span><span class="sxs-lookup"><span data-stu-id="0bc1f-102">Update DNS records to keep your website with your current hosting provider</span></span>

1. <span data-ttu-id="0bc1f-103">В центъра за администриране на Microsoft 365 отидете на страницата **Настройка**на  >  [домейни](https://admin.microsoft.com/Adminportal#/Domains) и в списъка с домейни изберете домейна, който използвате за своя уеб сайт.</span><span class="sxs-lookup"><span data-stu-id="0bc1f-103">In the Microsoft 365 admin center, go to the **Setup** > [Domains](https://admin.microsoft.com/Adminportal#/Domains) page, and in the list of domains, select the domain you're using for your website.</span></span>

2. <span data-ttu-id="0bc1f-104">Изберете **+ нов запис по избор** и въведете следната информация:</span><span class="sxs-lookup"><span data-stu-id="0bc1f-104">Select **+ New custom record** and enter the following:</span></span>

  - <span data-ttu-id="0bc1f-105">За **тип на DNS** въведете: **a (адрес)**</span><span class="sxs-lookup"><span data-stu-id="0bc1f-105">For **DNS type** enter: **A (Address)**</span></span>

  - <span data-ttu-id="0bc1f-106">За **име на хост или псевдоним**въведете следното: **@**</span><span class="sxs-lookup"><span data-stu-id="0bc1f-106">For **Host name or Alias**, type the following: **@**</span></span>

  - <span data-ttu-id="0bc1f-107">За **IP адрес**въведете статичен IP адрес за вашия уеб сайт, където се хоства в момента (например: 172.16.140.1).</span><span class="sxs-lookup"><span data-stu-id="0bc1f-107">For **IP Address**, type the static IP address for your website where it's currently hosted (for example, 172.16.140.1).</span></span>

    <span data-ttu-id="0bc1f-108">Това трябва да бъде  *статичен*  IP адрес за уеб сайта, а не  *динамичен*  IP адрес.</span><span class="sxs-lookup"><span data-stu-id="0bc1f-108">This must be a  *static*  IP address for the website, not a  *dynamic*  IP address.</span></span> <span data-ttu-id="0bc1f-109">Проверете със сайта, където е хостван Вашият уеб сайт, за да сте сигурни, че можете да получите статичен IP адрес за вашия публичен уеб сайт.</span><span class="sxs-lookup"><span data-stu-id="0bc1f-109">Check with site where your website is hosted to make sure you can get a static IP address for your public website.</span></span>

3. <span data-ttu-id="0bc1f-110">Изберете **Запиши**.</span><span class="sxs-lookup"><span data-stu-id="0bc1f-110">Select **Save**.</span></span>

<span data-ttu-id="0bc1f-111">Освен това можете да създадете CNAME запис, за да помогнете на потребителите да намират своя уеб сайт.</span><span class="sxs-lookup"><span data-stu-id="0bc1f-111">In addition, you can create a CNAME record to help customers find your website.</span></span>
  
1. <span data-ttu-id="0bc1f-112">Изберете **+ нов запис по избор** и въведете следната информация:</span><span class="sxs-lookup"><span data-stu-id="0bc1f-112">Select **+ New custom record** and enter the following:</span></span>

  - <span data-ttu-id="0bc1f-113">За **тип на DNS** въведете: **CNAME (Alias)**</span><span class="sxs-lookup"><span data-stu-id="0bc1f-113">For **DNS type** enter: **CNAME (Alias)**</span></span>

  - <span data-ttu-id="0bc1f-114">За **име на хост или псевдоним**въведете следното: **www**</span><span class="sxs-lookup"><span data-stu-id="0bc1f-114">For **Host name or Alias**, type the following: **www**</span></span>

  - <span data-ttu-id="0bc1f-115">За **сочи към адрес**въведете напълно квалифицирано име на домейн (FQDN) за вашия уеб сайт (например contoso.com).</span><span class="sxs-lookup"><span data-stu-id="0bc1f-115">For **Points to address**, type the fully qualified domain name (FQDN) for your website (for example, contoso.com).</span></span>

2. <span data-ttu-id="0bc1f-116">Изберете **Запиши**.</span><span class="sxs-lookup"><span data-stu-id="0bc1f-116">Select **Save**.</span></span>
