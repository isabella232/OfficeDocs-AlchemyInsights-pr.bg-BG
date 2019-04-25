---
title: UPN синхронизация с увреждания
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 3/20/2018
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: 2a3489fe-c2a8-4e43-96c2-be4b3c5e978c
ms.openlocfilehash: 2a03ac64d92c07b523b015850251b33c58bb76f8
ms.sourcegitcommit: 9d78905c512192ffc4675468abd2efc5f2e4baf4
ms.translationtype: MT
ms.contentlocale: bg-BG
ms.lasthandoff: 04/23/2019
ms.locfileid: "32423532"
---
# <a name="upn-sync-disabled"></a><span data-ttu-id="8bc7d-102">UPN синхронизация с увреждания</span><span class="sxs-lookup"><span data-stu-id="8bc7d-102">UPN sync disabled</span></span>

<span data-ttu-id="8bc7d-103">Ако сте започнали syncing към лазурно АД преди 30 март 2016, изпълнете следните Azure АД PowerShell cmdlet да разрешите UPN мек мач за вашата организация само:</span><span class="sxs-lookup"><span data-stu-id="8bc7d-103">If you started syncing to Azure AD before March 30, 2016, run the following Azure AD PowerShell cmdlet to enable UPN soft match for your organization only:</span></span>
  
 <span data-ttu-id="8bc7d-104">**Комплект-MsolDirSyncFeature-функция EnableSoftMatchOnUpn-давам възможност на $True**</span><span class="sxs-lookup"><span data-stu-id="8bc7d-104">**Set-MsolDirSyncFeature -Feature EnableSoftMatchOnUpn -Enable $True**</span></span>
  
<span data-ttu-id="8bc7d-105">UPN мек мач е включено автоматично за организации, които започнали syncing към лазурните реклама на или след 30 март 2016 г.</span><span class="sxs-lookup"><span data-stu-id="8bc7d-105">UPN soft match is automatically turned on for organizations that started syncing to Azure AD on or after March 30, 2016.</span></span>
  
<span data-ttu-id="8bc7d-106">За да научите повече за активирането на мек мач на UPN и други функции за синхронизиране, моля вижте [Azure АД свържете синхронизация услуга функции](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnectsyncservice-features).</span><span class="sxs-lookup"><span data-stu-id="8bc7d-106">To learn more about enabling soft match on UPN and other sync features, please see [Azure AD Connect sync service features](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnectsyncservice-features).</span></span>
  

