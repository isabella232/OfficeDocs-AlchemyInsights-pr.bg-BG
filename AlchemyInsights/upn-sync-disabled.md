---
title: UPN синхронизирането е забранено
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: 2a3489fe-c2a8-4e43-96c2-be4b3c5e978c
ms.openlocfilehash: 2b1ba772459091ce1a796884997fe2516d0407eb
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: bg-BG
ms.lasthandoff: 04/15/2021
ms.locfileid: "51782140"
---
# <a name="upn-sync-disabled"></a><span data-ttu-id="d644a-102">UPN синхронизирането е забранено</span><span class="sxs-lookup"><span data-stu-id="d644a-102">UPN sync disabled</span></span>

<span data-ttu-id="d644a-103">Ако сте започнали да синхронизирате с Azure AD преди 30 март 2016 г., изпълнете следната кратка команда Azure AD PowerShell, за да разрешите UPN софтуерно съвпадение само за вашата организация:</span><span class="sxs-lookup"><span data-stu-id="d644a-103">If you started syncing to Azure AD before March 30, 2016, run the following Azure AD PowerShell cmdlet to enable UPN soft match for your organization only:</span></span>
  
 <span data-ttu-id="d644a-104">**Set-MsolDirSyncFeature -Feature EnableSoftMatchOnUpn -Enable $True**</span><span class="sxs-lookup"><span data-stu-id="d644a-104">**Set-MsolDirSyncFeature -Feature EnableSoftMatchOnUpn -Enable $True**</span></span>
  
<span data-ttu-id="d644a-105">UpN soft match се включва автоматично за организации, които са започнали синхронизиране с Azure AD на или след 30 март 2016 г.</span><span class="sxs-lookup"><span data-stu-id="d644a-105">UPN soft match is automatically turned on for organizations that started syncing to Azure AD on or after March 30, 2016.</span></span>
  
<span data-ttu-id="d644a-106">За да научите повече за разрешаването на софтуерно съвпадение в UPN и други функции за синхронизиране, вижте Функции на услугата [за синхронизиране на Azure AD Connect](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnectsyncservice-features).</span><span class="sxs-lookup"><span data-stu-id="d644a-106">To learn more about enabling soft match on UPN and other sync features, please see [Azure AD Connect sync service features](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnectsyncservice-features).</span></span>
  

