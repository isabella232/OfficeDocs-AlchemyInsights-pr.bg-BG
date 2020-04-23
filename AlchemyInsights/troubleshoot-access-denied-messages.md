---
title: Отстраняване на отказан достъп съобщения
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: d678b57a-53ad-4414-9423-d8726a0c532f
ms.openlocfilehash: 1930edcfd14acc48ea77b66e2793654a3e6332cc
ms.sourcegitcommit: 631cbb5f03e5371f0995e976536d24e9d13746c3
ms.translationtype: MT
ms.contentlocale: bg-BG
ms.lasthandoff: 04/22/2020
ms.locfileid: "43759789"
---
# <a name="troubleshoot-access-denied-messages"></a><span data-ttu-id="5125c-102">Отстраняване на отказан достъп съобщения</span><span class="sxs-lookup"><span data-stu-id="5125c-102">Troubleshoot Access Denied messages</span></span>

<span data-ttu-id="5125c-103">Ако някой получи съобщение "Достъпът отказан" в споделена папка в SharePoint, администраторът на колекцията от сайтове може да е разрешил "Ограничен достъп потребител разрешение lockdown режим."</span><span class="sxs-lookup"><span data-stu-id="5125c-103">If someone got an "Access Denied" message to a shared folder in SharePoint, the site collection administrator might have enabled "Limited-access user permission lockdown mode."</span></span> <span data-ttu-id="5125c-104">За да изключите това:</span><span class="sxs-lookup"><span data-stu-id="5125c-104">To turn this off:</span></span> 
  
1. <span data-ttu-id="5125c-105">Намерете сайта, щракнете върху иконата настройки и след това щракнете върху **Настройки на сайта**.</span><span class="sxs-lookup"><span data-stu-id="5125c-105">Browse to the site, click the Settings icon, and then click **Site Settings**.</span></span>
    
2. <span data-ttu-id="5125c-106">Под **Администриране на колекция от сайтове**щракнете върху функции на **колекцията .**</span><span class="sxs-lookup"><span data-stu-id="5125c-106">Under **Site Collection Administration**, click **Site collection features**.</span></span>
    
3. <span data-ttu-id="5125c-107">До **ограничен достъп до режим на блокиране**на разрешенията за ограничен достъп щракнете върху **Дезактивиране**.</span><span class="sxs-lookup"><span data-stu-id="5125c-107">Next to **Limited-access user permission lockdown mode**, click **Deactivate**.</span></span>
    
<span data-ttu-id="5125c-108">Съобщение за отказан достъп може да възникне и за споделени папки, ако сайтът е сайт за публикуване.</span><span class="sxs-lookup"><span data-stu-id="5125c-108">An Access Denied message can also occur for shared folders if the site is a publishing site.</span></span> <span data-ttu-id="5125c-109">За информация вижте [Отказан достъп при достъп до споделена папка](https://go.microsoft.com/fwlink/?linkid=2004317).</span><span class="sxs-lookup"><span data-stu-id="5125c-109">For info, see [Access Denied when accessing a shared folder](https://go.microsoft.com/fwlink/?linkid=2004317).</span></span>
  
<span data-ttu-id="5125c-110">Ако някой получи съобщение "Достъпът отказан", когато се опитвате да видите заявки за достъп, потребителят трябва да се добави като администратор на колекция от сайтове или член на групата на собствениците на сайта.</span><span class="sxs-lookup"><span data-stu-id="5125c-110">If a someone got an "Access Denied" message when trying to view access requests, the user needs to be added as either a site collection administrator or a member of the Owners group for the site.</span></span> <span data-ttu-id="5125c-111">За повече информация вижте [Отказан достъп до списъка с искания за достъп](https://go.microsoft.com/fwlink/?linkid=2004220).</span><span class="sxs-lookup"><span data-stu-id="5125c-111">For more info, see [Access Denied to Access Requests list](https://go.microsoft.com/fwlink/?linkid=2004220).</span></span>
  
<span data-ttu-id="5125c-112">Ако потребител получи съобщение "Достъпът отказан", след като те са премахнати от локалния Active Directory и след това добавени обратно, вижте [Отказан достъп, когато потребителски акаунт се синхронизира с Microsoft 365](https://go.microsoft.com/fwlink/?linkid=2004318).</span><span class="sxs-lookup"><span data-stu-id="5125c-112">If a user got an "Access Denied" message after they were removed from Active Directory on-premises and then added back, see [Access Denied when a user account is synced to Microsoft 365](https://go.microsoft.com/fwlink/?linkid=2004318).</span></span>
  

