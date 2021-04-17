---
title: Актуализирайте DNS записите, за да поддържате уеб сайта си с вашия текущ доставчик на хостинг
ms.author: pebaum
author: pebaum
manager: scotv
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
ms.openlocfilehash: 89bce2aa5931c0c20706efabd42d2351be43938b
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: bg-BG
ms.lasthandoff: 04/15/2021
ms.locfileid: "51827496"
---
# <a name="update-dns-records-to-keep-your-website-with-your-current-hosting-provider"></a><span data-ttu-id="07e7e-102">Актуализирайте DNS записите, за да поддържате уеб сайта си с вашия текущ доставчик на хостинг</span><span class="sxs-lookup"><span data-stu-id="07e7e-102">Update DNS records to keep your website with your current hosting provider</span></span>

1. <span data-ttu-id="07e7e-103">В центъра за администриране на Microsoft 365 отидете на страницата Домейни за настройка и в списъка с домейни изберете домейна,   >  [](https://admin.microsoft.com/Adminportal#/Domains) който използвате за вашия уеб сайт.</span><span class="sxs-lookup"><span data-stu-id="07e7e-103">In the Microsoft 365 admin center, go to the **Setup** > [Domains](https://admin.microsoft.com/Adminportal#/Domains) page, and in the list of domains, select the domain you're using for your website.</span></span>

2. <span data-ttu-id="07e7e-104">Изберете **+ Нов потребителски запис** и въведете следното:</span><span class="sxs-lookup"><span data-stu-id="07e7e-104">Select **+ New custom record** and enter the following:</span></span>

  - <span data-ttu-id="07e7e-105">За **въвеждане на DNS** тип: A **(Адрес)**</span><span class="sxs-lookup"><span data-stu-id="07e7e-105">For **DNS type** enter: **A (Address)**</span></span>

  - <span data-ttu-id="07e7e-106">За **Име на хост или Псевдоним** въведете следното: **@**</span><span class="sxs-lookup"><span data-stu-id="07e7e-106">For **Host name or Alias**, type the following: **@**</span></span>

  - <span data-ttu-id="07e7e-107">За **IP адрес** въведете статичния IP адрес за вашия уеб сайт, където се хоства в момента (например 172.16.140.1).</span><span class="sxs-lookup"><span data-stu-id="07e7e-107">For **IP Address**, type the static IP address for your website where it's currently hosted (for example, 172.16.140.1).</span></span>

    <span data-ttu-id="07e7e-108">Това трябва да е  *статичен*  IP адрес за уеб сайта, а не  *динамичен*  IP адрес.</span><span class="sxs-lookup"><span data-stu-id="07e7e-108">This must be a  *static*  IP address for the website, not a  *dynamic*  IP address.</span></span> <span data-ttu-id="07e7e-109">Консултирайте се със сайта, където се хоства уеб сайтът ви, за да се уверите, че можете да получите статичен IP адрес за вашия публичен уеб сайт.</span><span class="sxs-lookup"><span data-stu-id="07e7e-109">Check with site where your website is hosted to make sure you can get a static IP address for your public website.</span></span>

3. <span data-ttu-id="07e7e-110">Изберете **Запиши**.</span><span class="sxs-lookup"><span data-stu-id="07e7e-110">Select **Save**.</span></span>

<span data-ttu-id="07e7e-111">Освен това можете да създадете CNAME запис, който да помогне на клиентите да намерят вашия уеб сайт.</span><span class="sxs-lookup"><span data-stu-id="07e7e-111">In addition, you can create a CNAME record to help customers find your website.</span></span>
  
1. <span data-ttu-id="07e7e-112">Изберете **+ Нов потребителски запис** и въведете следното:</span><span class="sxs-lookup"><span data-stu-id="07e7e-112">Select **+ New custom record** and enter the following:</span></span>

  - <span data-ttu-id="07e7e-113">За **въвеждане на DNS** тип: **CNAME (Псевдоним)**</span><span class="sxs-lookup"><span data-stu-id="07e7e-113">For **DNS type** enter: **CNAME (Alias)**</span></span>

  - <span data-ttu-id="07e7e-114">За **Име на хост или Псевдоним** въведете следното: **www**</span><span class="sxs-lookup"><span data-stu-id="07e7e-114">For **Host name or Alias**, type the following: **www**</span></span>

  - <span data-ttu-id="07e7e-115">За **Адрес на точки** въведете пълното име на домейн (FQDN) за вашия уеб сайт (например contoso.com).</span><span class="sxs-lookup"><span data-stu-id="07e7e-115">For **Points to address**, type the fully qualified domain name (FQDN) for your website (for example, contoso.com).</span></span>

2. <span data-ttu-id="07e7e-116">Изберете **Запиши**.</span><span class="sxs-lookup"><span data-stu-id="07e7e-116">Select **Save**.</span></span>
