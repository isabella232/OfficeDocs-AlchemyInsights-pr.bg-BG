---
title: Достъпът е отказан при преглеждане на работен поток
ms.author: pebaum
author: Techwriter40
ms.date: 11/27/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 47ceb983-f9a4-4c55-a40c-03d5c3d75dc9
ms.openlocfilehash: 4ca65583fbd98867026e9e3cc8f36fe38798aa85
ms.sourcegitcommit: a65d196d00adb70045af5caca9828fe44b951f61
ms.translationtype: MT
ms.contentlocale: bg-BG
ms.lasthandoff: 09/04/2019
ms.locfileid: "36747737"
---
# <a name="access-denied-when-viewing-a-workflow"></a><span data-ttu-id="8abc0-102">Достъпът е отказан при преглеждане на работен поток</span><span class="sxs-lookup"><span data-stu-id="8abc0-102">Access denied when viewing a Workflow</span></span>

<span data-ttu-id="8abc0-103">SharePoint 2013 работни потоци, които се опитват да изпратите имейл до група на SharePoint може да се провали с съобщение за грешка "достъпът отказан", ако членството на групата на SharePoint не е зададен на всички.</span><span class="sxs-lookup"><span data-stu-id="8abc0-103">SharePoint 2013 Workflows that attempt to send an email to a SharePoint group can fail with an "Access Denied" error message if the membership of the SharePoint group is not set to Everyone.</span></span>
  
 <span data-ttu-id="8abc0-104">**За да разрешите този проблем, изпълнете следните стъпки:**</span><span class="sxs-lookup"><span data-stu-id="8abc0-104">**To resolve this issue, do these steps:**</span></span>
  
 1. <span data-ttu-id="8abc0-105">Позволете на всички да виждат членовете на групата на SharePoint.</span><span class="sxs-lookup"><span data-stu-id="8abc0-105">Allow everybody to see the members of the SharePoint group.</span></span>
  
 2. <span data-ttu-id="8abc0-106">Премахнете групата на SharePoint от до или Як линия на имейла.</span><span class="sxs-lookup"><span data-stu-id="8abc0-106">Remove the SharePoint group from the To or CC line of the email.</span></span>
  
 3. <span data-ttu-id="8abc0-107">Изрично добавете потребителите към до или Як линия, ако членството видимост не може да се промени за група на SharePoint.</span><span class="sxs-lookup"><span data-stu-id="8abc0-107">Explicitly add the users to the To or CC line if the membership visibility cannot be changed for SharePoint group.</span></span>
  
<span data-ttu-id="8abc0-108">За да видите повече подробности, моля, вижте [http неразрешено към/_vti_bin/client.SVC/SP.Utilities.Utility.SendEmail](https://go.microsoft.com/fwlink/?linkid=2044694&amp;clcid=0x409).</span><span class="sxs-lookup"><span data-stu-id="8abc0-108">To view more details please refer to [HTTP Unauthorized to /_vti_bin/client.svc/sp.utilities.utility.SendEmail](https://go.microsoft.com/fwlink/?linkid=2044694&amp;clcid=0x409).</span></span>
  