---
title: UPN синхронизация с увреждания
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 3/20/2018
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom: Adm_O365
ms.assetid: 2a3489fe-c2a8-4e43-96c2-be4b3c5e978c
ms.openlocfilehash: 027782bb2a6b892df6201f3c3bf55151ef7b9db7
ms.sourcegitcommit: 0ae6cbb8cf2836da98300767ed81b411d6551bee
ms.translationtype: MT
ms.contentlocale: bg-BG
ms.lasthandoff: 01/30/2019
ms.locfileid: "29657960"
---
# <a name="upn-sync-disabled"></a><span data-ttu-id="8080e-102">UPN синхронизация с увреждания</span><span class="sxs-lookup"><span data-stu-id="8080e-102">UPN sync disabled</span></span>

<span data-ttu-id="8080e-103">Ако сте започнали syncing към лазурно АД преди 30 март 2016, изпълнете следните Azure АД PowerShell cmdlet да разрешите UPN мек мач за вашата организация само:</span><span class="sxs-lookup"><span data-stu-id="8080e-103">If you started syncing to Azure AD before March 30, 2016, run the following Azure AD PowerShell cmdlet to enable UPN soft match for your organization only:</span></span>
  
 <span data-ttu-id="8080e-104">**Комплект-MsolDirSyncFeature-функция EnableSoftMatchOnUpn-давам възможност на $True**</span><span class="sxs-lookup"><span data-stu-id="8080e-104">**Set-MsolDirSyncFeature -Feature EnableSoftMatchOnUpn -Enable $True**</span></span>
  
<span data-ttu-id="8080e-105">UPN мек мач е включено автоматично за организации, които започнали syncing към лазурните реклама на или след 30 март 2016 г.</span><span class="sxs-lookup"><span data-stu-id="8080e-105">UPN soft match is automatically turned on for organizations that started syncing to Azure AD on or after March 30, 2016.</span></span>
  
<span data-ttu-id="8080e-106">За да научите повече за активирането на мек мач на UPN и други функции за синхронизиране, моля вижте [Azure АД свържете синхронизация услуга функции](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnectsyncservice-features).</span><span class="sxs-lookup"><span data-stu-id="8080e-106">To learn more about enabling soft match on UPN and other sync features, please see [Azure AD Connect sync service features](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnectsyncservice-features).</span></span>
  

