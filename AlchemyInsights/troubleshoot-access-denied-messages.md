---
title: Отстраняване на неизправности при съобщения за отказан достъп
ms.author: kaarins
author: kaarins
ms.date: 6/29/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.assetid: d678b57a-53ad-4414-9423-d8726a0c532f
ms.openlocfilehash: 3973f5bf584343d3353e7389f22bc727827b5c35
ms.sourcegitcommit: d6ea5e9458a2b8ceaab3ac4bd483e1130b9a398a
ms.translationtype: MT
ms.contentlocale: bg-BG
ms.lasthandoff: 01/15/2019
ms.locfileid: "28276257"
---
# <a name="troubleshoot-access-denied-messages"></a><span data-ttu-id="68f95-102">Отстраняване на неизправности при съобщения за отказан достъп</span><span class="sxs-lookup"><span data-stu-id="68f95-102">Troubleshoot Access Denied messages</span></span>

<span data-ttu-id="68f95-p101">Ако някой имам "Достъп отказ" съобщение в споделена папка, администраторът на колекцията сайтове може да позволи на "ограничен достъп потребител разрешение lockdown режим." За да изключите това:</span><span class="sxs-lookup"><span data-stu-id="68f95-p101">If someone got an "Access Denied" message to a shared folder, the site collection administrator might have enabled "Limited-access user permission lockdown mode." To turn this off:</span></span> 
  
1. <span data-ttu-id="68f95-105">Прегледайте сайта, щракнете върху иконата настройки и след това щракнете върху **Настройки на сайта**.</span><span class="sxs-lookup"><span data-stu-id="68f95-105">Browse to the site, click the Settings icon, and then click **Site Settings**.</span></span>
    
2. <span data-ttu-id="68f95-106">Под **Администриране на колекцията сайтове**щракнете върху **функции на колекцията сайтове**.</span><span class="sxs-lookup"><span data-stu-id="68f95-106">Under **Site Collection Administration**, click **Site collection features**.</span></span>
    
3. <span data-ttu-id="68f95-107">Щракнете върху **Дезактивирай**до **ограничен достъп потребител разрешение lockdown режим**.</span><span class="sxs-lookup"><span data-stu-id="68f95-107">Next to **Limited-access user permission lockdown mode**, click **Deactivate**.</span></span>
    
<span data-ttu-id="68f95-p102">Съобщение за отказан достъп може да се появи за споделени папки, ако сайтът е сайт за публикуване. За информация вижте [Достъп отказ при достъп до споделена папка](https://go.microsoft.com/fwlink/?linkid=2004317).</span><span class="sxs-lookup"><span data-stu-id="68f95-p102">An Access Denied message can also occur for shared folders if the site is a publishing site. For info, see [Access Denied when accessing a shared folder](https://go.microsoft.com/fwlink/?linkid=2004317).</span></span>
  
<span data-ttu-id="68f95-p103">Ако някой имам "Достъп отказ" съобщение, когато се опитвате да видите искания за достъп, потребителят трябва да се добави като администратор на колекция или член на групата на собствениците на сайта. За повече информация вижте [Отказан достъп до списъка на искания за достъп](https://go.microsoft.com/fwlink/?linkid=2004220).</span><span class="sxs-lookup"><span data-stu-id="68f95-p103">If a someone got an "Access Denied" message when trying to view access requests, the user needs to be added as either a site collection administrator or a member of the Owners group for the site. For more info, see [Access Denied to Access Requests list](https://go.microsoft.com/fwlink/?linkid=2004220).</span></span>
  
<span data-ttu-id="68f95-112">Ако потребител имам "Достъп отказ" съобщение, след като са били премахнати от Active Directory локално и след това се добавя обратно, вижте [Отказан достъп, когато даден потребителски акаунт се синхронизира към Office 365](https://go.microsoft.com/fwlink/?linkid=2004318).</span><span class="sxs-lookup"><span data-stu-id="68f95-112">If a user got an "Access Denied" message after they were removed from Active Directory on-premises and then added back, see [Access Denied when a user account is synced to Office 365](https://go.microsoft.com/fwlink/?linkid=2004318).</span></span>
  

