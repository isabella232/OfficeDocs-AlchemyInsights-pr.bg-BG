---
title: Проверка на домейна ви
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "47"
- "48"
- "8"
ms.assetid: 81fd176b-3d67-4e52-9ab8-d36602412734
ms.openlocfilehash: 2c4d8e075d2cf7214b5ef005b856daf7fb0ed53c
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: bg-BG
ms.lasthandoff: 04/22/2020
ms.locfileid: "43710432"
---
# <a name="verify-your-domain"></a><span data-ttu-id="0392d-102">Проверка на домейна ви</span><span class="sxs-lookup"><span data-stu-id="0392d-102">Verify your domain</span></span>

 <span data-ttu-id="0392d-103">**Записът вероятно не се е актуализирал в интернет.**</span><span class="sxs-lookup"><span data-stu-id="0392d-103">**The record probably hasn't updated across the Internet.**</span></span>
  
<span data-ttu-id="0392d-104">Обикновено отнема само няколко минути, за да можем да видим новия запис, но понякога може да отнеме толкова време, колкото няколко часа.</span><span class="sxs-lookup"><span data-stu-id="0392d-104">It typically only takes a few minutes for us to be able to see the new record, but occasionally it can take as long as a few hours.</span></span> 
  
- <span data-ttu-id="0392d-105">Ако сте изчакали толкова дълго вече, проверете два пъти, че сте копирали и поставили точната стойност в tXT записа за потвърждение на вашия DNS хост.</span><span class="sxs-lookup"><span data-stu-id="0392d-105">If you've waited that long already, double-check that you've copied and pasted the exact value into the TXT verification record at your DNS host.</span></span> <span data-ttu-id="0392d-106">Един общ проблем не включва "MS =" част на записа.</span><span class="sxs-lookup"><span data-stu-id="0392d-106">One common issue is not including the "MS=" part of the record.</span></span> <span data-ttu-id="0392d-107">И на нас ни трябва!</span><span class="sxs-lookup"><span data-stu-id="0392d-107">We need that too!</span></span>

- <span data-ttu-id="0392d-108">В някои DNS хостове, трябва да направите допълнителна стъпка, за да запазите файла зона (където се съхранява DNS запис), така че да се актуализира в интернет.</span><span class="sxs-lookup"><span data-stu-id="0392d-108">At some DNS hosts, you have to take an extra step to save the zone file (where the DNS record is stored) so that it will update across the Internet.</span></span> <span data-ttu-id="0392d-109">Уверете се, че сте записали промените, така че Microsoft да може да вижда и проверява записа.</span><span class="sxs-lookup"><span data-stu-id="0392d-109">Make sure you've saved your changes so Microsoft can see and verify the record.</span></span>
