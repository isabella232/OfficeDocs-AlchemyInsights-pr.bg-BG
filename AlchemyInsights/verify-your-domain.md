---
title: Проверка на вашия домейн
ms.author: pebaum
author: pebaum
manager: mnirkhe
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
ms.openlocfilehash: d30f9b51c0164acd126f214a581ad6cec5eec04e
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: bg-BG
ms.lasthandoff: 09/14/2020
ms.locfileid: "47734295"
---
# <a name="verify-your-domain"></a><span data-ttu-id="f1bca-102">Проверка на вашия домейн</span><span class="sxs-lookup"><span data-stu-id="f1bca-102">Verify your domain</span></span>

 <span data-ttu-id="f1bca-103">**Записът вероятно не е актуализиран по интернет.**</span><span class="sxs-lookup"><span data-stu-id="f1bca-103">**The record probably hasn't updated across the Internet.**</span></span>
  
<span data-ttu-id="f1bca-104">За нас обикновено са необходими само няколко минути, за да можем да видим новия запис, но понякога може да отнеме няколко часа.</span><span class="sxs-lookup"><span data-stu-id="f1bca-104">It typically only takes a few minutes for us to be able to see the new record, but occasionally it can take as long as a few hours.</span></span> 
  
- <span data-ttu-id="f1bca-105">Ако сте чакали толкова дълго, проверете отново, че сте копирали и поставили точните стойности в TXT проверката на вашия DNS хост.</span><span class="sxs-lookup"><span data-stu-id="f1bca-105">If you've waited that long already, double-check that you've copied and pasted the exact value into the TXT verification record at your DNS host.</span></span> <span data-ttu-id="f1bca-106">Един често срещан проблем не включва частта "MS =" на записа.</span><span class="sxs-lookup"><span data-stu-id="f1bca-106">One common issue is not including the "MS=" part of the record.</span></span> <span data-ttu-id="f1bca-107">Ние също имаме нужда от това!</span><span class="sxs-lookup"><span data-stu-id="f1bca-107">We need that too!</span></span>

- <span data-ttu-id="f1bca-108">При някои DNS хостове трябва да предприемете допълнителна стъпка, за да запишете файла на зоната (където се съхранява DNS записът), така че да се актуализира по интернет.</span><span class="sxs-lookup"><span data-stu-id="f1bca-108">At some DNS hosts, you have to take an extra step to save the zone file (where the DNS record is stored) so that it will update across the Internet.</span></span> <span data-ttu-id="f1bca-109">Уверете се, че сте записали промените, така че Microsoft да може да вижда и проверява записа.</span><span class="sxs-lookup"><span data-stu-id="f1bca-109">Make sure you've saved your changes so Microsoft can see and verify the record.</span></span>
