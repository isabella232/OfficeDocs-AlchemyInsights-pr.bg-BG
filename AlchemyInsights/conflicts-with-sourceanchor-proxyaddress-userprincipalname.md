---
title: Конфликти с SourceAnchor, ProxyAddress, UserPrincipalName
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/20/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "1699"
- "1300022"
ms.openlocfilehash: 877c954bea219cf8d885645cd25e41a5b7bab6fd
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: bg-BG
ms.lasthandoff: 09/14/2020
ms.locfileid: "47713443"
---
# <a name="conflicts-with-sourceanchor-proxyaddress-userprincipalname"></a><span data-ttu-id="ec27f-102">Конфликти с SourceAnchor, ProxyAddress, UserPrincipalName</span><span class="sxs-lookup"><span data-stu-id="ec27f-102">Conflicts with SourceAnchor, ProxyAddress, UserPrincipalName</span></span>

<span data-ttu-id="ec27f-103">Ако получавате грешки по време на синхронизация, като например "синхронизиран обект със същите ProxyAddress или UserPrincipalName съществува във вашия указател", вижте [диагностициране и възстановяване на дублирани грешки при синхронизиране на атрибут](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-health-diagnose-sync-errors).</span><span class="sxs-lookup"><span data-stu-id="ec27f-103">If you receive errors during a synchronization such as "A synchronized object with the same ProxyAddress or UserPrincipalName exists in your directory", see [Diagnose and remediate duplicated attribute sync errors](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-health-diagnose-sync-errors).</span></span>

<span data-ttu-id="ec27f-104">Освен това можете да разрешавате устойчивост на дублираните атрибути.</span><span class="sxs-lookup"><span data-stu-id="ec27f-104">Also, consider enabling duplicate attribute resiliency.</span></span> <span data-ttu-id="ec27f-105">За повече информация вижте [Синхронизиране на самоличност и издръжливост на дублирани атрибути](https://aka.ms/duplicateattributeresiliency).</span><span class="sxs-lookup"><span data-stu-id="ec27f-105">For more info, see [Identity synchronization and duplicate attribute resiliency](https://aka.ms/duplicateattributeresiliency).</span></span>