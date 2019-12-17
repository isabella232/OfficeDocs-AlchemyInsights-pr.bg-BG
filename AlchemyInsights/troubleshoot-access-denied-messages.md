---
title: Отстраняване на съобщения за отказан достъп
ms.author: pebaum
author: pebaum
ms.date: 6/29/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: d678b57a-53ad-4414-9423-d8726a0c532f
ms.openlocfilehash: 05d12aee49b449e8a29e84021b41298fb9983859
ms.sourcegitcommit: 0f0186044a3597e42ad14c32ca58e7224344dcfa
ms.translationtype: MT
ms.contentlocale: bg-BG
ms.lasthandoff: 12/15/2019
ms.locfileid: "40050694"
---
# <a name="troubleshoot-access-denied-messages"></a><span data-ttu-id="ebaa5-102">Отстраняване на съобщения за отказан достъп</span><span class="sxs-lookup"><span data-stu-id="ebaa5-102">Troubleshoot Access Denied messages</span></span>

<span data-ttu-id="ebaa5-103">Ако някой има съобщение "отказан достъп" до споделена папка в SharePoint, администраторът на колекцията от сайтове може да е разрешил "ограничен достъп потребител разрешение режим заключване".</span><span class="sxs-lookup"><span data-stu-id="ebaa5-103">If someone got an "Access Denied" message to a shared folder in SharePoint, the site collection administrator might have enabled "Limited-access user permission lockdown mode."</span></span> <span data-ttu-id="ebaa5-104">За да изключите това:</span><span class="sxs-lookup"><span data-stu-id="ebaa5-104">To turn this off:</span></span> 
  
1. <span data-ttu-id="ebaa5-105">Прегледайте сайта, щракнете върху иконата настройки и след това щракнете върху **Настройки на сайта**.</span><span class="sxs-lookup"><span data-stu-id="ebaa5-105">Browse to the site, click the Settings icon, and then click **Site Settings**.</span></span>
    
2. <span data-ttu-id="ebaa5-106">Под **администриране на колекция от сайтове**щракнете върху **функции на колекцията от сайтове**.</span><span class="sxs-lookup"><span data-stu-id="ebaa5-106">Under **Site Collection Administration**, click **Site collection features**.</span></span>
    
3. <span data-ttu-id="ebaa5-107">До **режим на заключване на потребителското разрешение с ограничен достъп**щракнете върху **дезактивиране**.</span><span class="sxs-lookup"><span data-stu-id="ebaa5-107">Next to **Limited-access user permission lockdown mode**, click **Deactivate**.</span></span>
    
<span data-ttu-id="ebaa5-108">Съобщение за отказан достъп може да се появи за споделени папки, ако сайтът е сайт за публикуване.</span><span class="sxs-lookup"><span data-stu-id="ebaa5-108">An Access Denied message can also occur for shared folders if the site is a publishing site.</span></span> <span data-ttu-id="ebaa5-109">За информация вижте [достъп отказан при достъп до споделена папка](https://go.microsoft.com/fwlink/?linkid=2004317).</span><span class="sxs-lookup"><span data-stu-id="ebaa5-109">For info, see [Access Denied when accessing a shared folder](https://go.microsoft.com/fwlink/?linkid=2004317).</span></span>
  
<span data-ttu-id="ebaa5-110">Ако някой има съобщение "достъпът е отказан" при опит за преглед на искания за достъп, потребителят трябва да бъде добавен или като администратор на колекция от сайтове или член на групата на собствениците на сайта.</span><span class="sxs-lookup"><span data-stu-id="ebaa5-110">If a someone got an "Access Denied" message when trying to view access requests, the user needs to be added as either a site collection administrator or a member of the Owners group for the site.</span></span> <span data-ttu-id="ebaa5-111">За повече информация вижте [списъка с отказан достъп до искания за достъп](https://go.microsoft.com/fwlink/?linkid=2004220).</span><span class="sxs-lookup"><span data-stu-id="ebaa5-111">For more info, see [Access Denied to Access Requests list](https://go.microsoft.com/fwlink/?linkid=2004220).</span></span>
  
<span data-ttu-id="ebaa5-112">Ако потребителят има съобщение "достъпът отказан", след като са били премахнати от Active Directory локално и след това добавени обратно, вижте [достъп отказан при потребителски акаунт се синхронизира с Office 365](https://go.microsoft.com/fwlink/?linkid=2004318).</span><span class="sxs-lookup"><span data-stu-id="ebaa5-112">If a user got an "Access Denied" message after they were removed from Active Directory on-premises and then added back, see [Access Denied when a user account is synced to Office 365](https://go.microsoft.com/fwlink/?linkid=2004318).</span></span>
  

