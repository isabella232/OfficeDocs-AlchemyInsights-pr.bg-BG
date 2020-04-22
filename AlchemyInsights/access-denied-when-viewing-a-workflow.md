---
title: Достъпът е отказан при преглед на работен поток
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 47ceb983-f9a4-4c55-a40c-03d5c3d75dc9
ms.openlocfilehash: c576bf88225582f2577e0b59506a7482cf9f38d5
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: bg-BG
ms.lasthandoff: 04/22/2020
ms.locfileid: "43687319"
---
# <a name="access-denied-when-viewing-a-workflow"></a><span data-ttu-id="13e27-102">Достъпът е отказан при преглед на работен поток</span><span class="sxs-lookup"><span data-stu-id="13e27-102">Access denied when viewing a Workflow</span></span>

<span data-ttu-id="13e27-103">SharePoint 2013 работни потоци, които се опитват да изпратите имейл до група на SharePoint може да се провали с съобщение за грешка "Достъпът е отказан", ако членството на групата на SharePoint не е зададена на всеки.</span><span class="sxs-lookup"><span data-stu-id="13e27-103">SharePoint 2013 Workflows that attempt to send an email to a SharePoint group can fail with an "Access Denied" error message if the membership of the SharePoint group is not set to Everyone.</span></span>
  
 <span data-ttu-id="13e27-104">**За да разрешите този проблем, направете следните стъпки:**</span><span class="sxs-lookup"><span data-stu-id="13e27-104">**To resolve this issue, do these steps:**</span></span>
  
 1. <span data-ttu-id="13e27-105">Позволявана на всички да виждат членовете на групата на SharePoint.</span><span class="sxs-lookup"><span data-stu-id="13e27-105">Allow everybody to see the members of the SharePoint group.</span></span>
  
 2. <span data-ttu-id="13e27-106">Премахнете групата на SharePoint от реда до или як на имейла.</span><span class="sxs-lookup"><span data-stu-id="13e27-106">Remove the SharePoint group from the To or CC line of the email.</span></span>
  
 3. <span data-ttu-id="13e27-107">Изрично добавете потребителите към или як ред, ако не може да се промени членството за SharePoint група.</span><span class="sxs-lookup"><span data-stu-id="13e27-107">Explicitly add the users to the To or CC line if the membership visibility cannot be changed for SharePoint group.</span></span>
  
<span data-ttu-id="13e27-108">За да видите повече подробности, моля, вижте [HTTP Неоторизиран достъп до /_vti_bin/client.svc/sp.utilities.utility.SendEmail](https://go.microsoft.com/fwlink/?linkid=2044694&amp;clcid=0x409).</span><span class="sxs-lookup"><span data-stu-id="13e27-108">To view more details please refer to [HTTP Unauthorized to /_vti_bin/client.svc/sp.utilities.utility.SendEmail](https://go.microsoft.com/fwlink/?linkid=2044694&amp;clcid=0x409).</span></span>
  