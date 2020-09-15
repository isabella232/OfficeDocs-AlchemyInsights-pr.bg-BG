---
title: Отстраняване на неизправности при отказан достъп
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: d678b57a-53ad-4414-9423-d8726a0c532f
ms.openlocfilehash: 3550081a12379f73725253214a2c2d44974ab740
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: bg-BG
ms.lasthandoff: 09/14/2020
ms.locfileid: "47690772"
---
# <a name="troubleshoot-access-denied-messages"></a><span data-ttu-id="86495-102">Отстраняване на неизправности при отказан достъп</span><span class="sxs-lookup"><span data-stu-id="86495-102">Troubleshoot Access Denied messages</span></span>

<span data-ttu-id="86495-103">Ако някой има съобщение "отказан достъп" в споделена папка в SharePoint, администраторът на колекцията от сайтове може да е активирал режима за заключване на потребители с ограничен достъп.</span><span class="sxs-lookup"><span data-stu-id="86495-103">If someone got an "Access Denied" message to a shared folder in SharePoint, the site collection administrator might have enabled "Limited-access user permission lockdown mode."</span></span> <span data-ttu-id="86495-104">За да изключите това:</span><span class="sxs-lookup"><span data-stu-id="86495-104">To turn this off:</span></span> 
  
1. <span data-ttu-id="86495-105">Отидете на сайта, щракнете върху иконата настройки и след това щракнете върху **Настройки на сайта**.</span><span class="sxs-lookup"><span data-stu-id="86495-105">Browse to the site, click the Settings icon, and then click **Site Settings**.</span></span>
    
2. <span data-ttu-id="86495-106">Под **администриране на колекция от сайтове**щракнете върху **функции на колекцията от сайтове**.</span><span class="sxs-lookup"><span data-stu-id="86495-106">Under **Site Collection Administration**, click **Site collection features**.</span></span>
    
3. <span data-ttu-id="86495-107">До **режима на заключване за потребители с ограничен достъп**щракнете върху **Дезактивирай**.</span><span class="sxs-lookup"><span data-stu-id="86495-107">Next to **Limited-access user permission lockdown mode**, click **Deactivate**.</span></span>
    
<span data-ttu-id="86495-108">Съобщение за отказан достъп може да възникне и за споделени папки, ако сайтът е сайт за публикуване.</span><span class="sxs-lookup"><span data-stu-id="86495-108">An Access Denied message can also occur for shared folders if the site is a publishing site.</span></span> <span data-ttu-id="86495-109">За информация вижте [отказан достъп при достъп до споделена папка](https://go.microsoft.com/fwlink/?linkid=2004317).</span><span class="sxs-lookup"><span data-stu-id="86495-109">For info, see [Access Denied when accessing a shared folder](https://go.microsoft.com/fwlink/?linkid=2004317).</span></span>
  
<span data-ttu-id="86495-110">Ако някой има съобщение "отказан достъп", когато се опитвате да видите исканията за достъп, потребителят трябва да бъде добавен или като администратор на колекцията от сайтове, или като член на групата "собственици" за сайта.</span><span class="sxs-lookup"><span data-stu-id="86495-110">If a someone got an "Access Denied" message when trying to view access requests, the user needs to be added as either a site collection administrator or a member of the Owners group for the site.</span></span> <span data-ttu-id="86495-111">За повече информация вижте [отказан достъп до списъка с искания за достъп](https://go.microsoft.com/fwlink/?linkid=2004220).</span><span class="sxs-lookup"><span data-stu-id="86495-111">For more info, see [Access Denied to Access Requests list](https://go.microsoft.com/fwlink/?linkid=2004220).</span></span>
  
<span data-ttu-id="86495-112">Ако потребител има съобщение "отказан достъп", след като са били премахнати от локален указател на Active Directory и след това сте добавили обратно, вижте [отказан достъп, когато потребителски акаунт е синхронизиран с Microsoft 365](https://go.microsoft.com/fwlink/?linkid=2004318).</span><span class="sxs-lookup"><span data-stu-id="86495-112">If a user got an "Access Denied" message after they were removed from Active Directory on-premises and then added back, see [Access Denied when a user account is synced to Microsoft 365](https://go.microsoft.com/fwlink/?linkid=2004318).</span></span>
  

