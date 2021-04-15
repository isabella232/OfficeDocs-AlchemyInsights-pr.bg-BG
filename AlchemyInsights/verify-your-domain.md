---
title: Проверка на вашия домейн
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "47"
- "48"
- "8"
ms.assetid: 81fd176b-3d67-4e52-9ab8-d36602412734
ms.openlocfilehash: 4a34de7fa2aaaae365cf4562d31590d4b5fb7544
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: bg-BG
ms.lasthandoff: 04/15/2021
ms.locfileid: "51770980"
---
# <a name="verify-your-domain"></a><span data-ttu-id="db5c3-102">Проверка на вашия домейн</span><span class="sxs-lookup"><span data-stu-id="db5c3-102">Verify your domain</span></span>

 <span data-ttu-id="db5c3-103">**Вероятно записът не е актуализиран в интернет.**</span><span class="sxs-lookup"><span data-stu-id="db5c3-103">**The record probably hasn't updated across the Internet.**</span></span>
  
<span data-ttu-id="db5c3-104">Обикновено ни отнема само няколко минути, за да можем да видим новия запис, но понякога може да отнеме няколко часа.</span><span class="sxs-lookup"><span data-stu-id="db5c3-104">It typically only takes a few minutes for us to be able to see the new record, but occasionally it can take as long as a few hours.</span></span> 
  
- <span data-ttu-id="db5c3-105">Ако вече сте чакали толкова дълго време, проверете двукратно дали сте копирали и сте заместили точната стойност в записа за проверка txt във вашия DNS хост.</span><span class="sxs-lookup"><span data-stu-id="db5c3-105">If you've waited that long already, double-check that you've copied and pasted the exact value into the TXT verification record at your DNS host.</span></span> <span data-ttu-id="db5c3-106">Един често срещан проблем не включва частта "MS=" на записа.</span><span class="sxs-lookup"><span data-stu-id="db5c3-106">One common issue is not including the "MS=" part of the record.</span></span> <span data-ttu-id="db5c3-107">И това ни трябва!</span><span class="sxs-lookup"><span data-stu-id="db5c3-107">We need that too!</span></span>

- <span data-ttu-id="db5c3-108">При някои DNS хостове трябва да предприемете допълнителна стъпка, за да запишете файла на зоната (където се съхранява DNS записът), така че да се актуализира в интернет.</span><span class="sxs-lookup"><span data-stu-id="db5c3-108">At some DNS hosts, you have to take an extra step to save the zone file (where the DNS record is stored) so that it will update across the Internet.</span></span> <span data-ttu-id="db5c3-109">Уверете се, че сте записали промените, така че Microsoft да може да вижда и проверява записа.</span><span class="sxs-lookup"><span data-stu-id="db5c3-109">Make sure you've saved your changes so Microsoft can see and verify the record.</span></span>
