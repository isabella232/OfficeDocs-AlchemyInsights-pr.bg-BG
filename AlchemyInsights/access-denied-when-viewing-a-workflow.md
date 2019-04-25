---
title: Достъпът е отказан при разглеждане на работен поток
ms.author: kirks
author: Techwriter40
ms.date: 11/27/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 47ceb983-f9a4-4c55-a40c-03d5c3d75dc9
ms.openlocfilehash: 43369c600687d6ac253f70a8535dc2bd0d41687e
ms.sourcegitcommit: 9d78905c512192ffc4675468abd2efc5f2e4baf4
ms.translationtype: MT
ms.contentlocale: bg-BG
ms.lasthandoff: 04/23/2019
ms.locfileid: "32389876"
---
# <a name="access-denied-when-viewing-a-workflow"></a><span data-ttu-id="b2a13-102">Достъпът е отказан при разглеждане на работен поток</span><span class="sxs-lookup"><span data-stu-id="b2a13-102">Access denied when viewing a Workflow</span></span>

<span data-ttu-id="b2a13-103">SharePoint 2013 работни потоци, които се опитват да изпратите имейл до SharePoint група може да се провали с "Достъп отказ" грешка съобщение, ако съставът на групата на SharePoint не е за всеки.</span><span class="sxs-lookup"><span data-stu-id="b2a13-103">SharePoint 2013 Workflows that attempt to send an email to a SharePoint group can fail with an "Access Denied" error message if the membership of the SharePoint group is not set to Everyone.</span></span>
  
 <span data-ttu-id="b2a13-104">**За да разрешите този проблем, направете следните стъпки:**</span><span class="sxs-lookup"><span data-stu-id="b2a13-104">**To resolve this issue, do these steps:**</span></span>
  
 1. <span data-ttu-id="b2a13-105">Позволи всички да видите членовете на групата на SharePoint.</span><span class="sxs-lookup"><span data-stu-id="b2a13-105">Allow everybody to see the members of the SharePoint group.</span></span> 
  
 2. <span data-ttu-id="b2a13-106">Премахнете групата на SharePoint от полето до или Як на писмото.</span><span class="sxs-lookup"><span data-stu-id="b2a13-106">Remove the SharePoint group from the To or CC line of the email.</span></span> 
  
 3. <span data-ttu-id="b2a13-107">Изрично да добавите потребители към полето до или Як линия ако видимостта на членство не може да бъде променено за SharePoint група.</span><span class="sxs-lookup"><span data-stu-id="b2a13-107">Explicitly add the users to the To or CC line if the membership visibility cannot be changed for SharePoint group.</span></span> 
  
<span data-ttu-id="b2a13-108">За да видите повече подробности моля вижте [HTTP неразрешените до /_vti_bin/client.svc/sp.utilities.utility.SendEmail ](https://go.microsoft.com/fwlink/?linkid=2044694&amp;clcid=0x409).</span><span class="sxs-lookup"><span data-stu-id="b2a13-108">To view more details please refer to [HTTP Unauthorized to /_vti_bin/client.svc/sp.utilities.utility.SendEmail ](https://go.microsoft.com/fwlink/?linkid=2044694&amp;clcid=0x409).</span></span>
  

