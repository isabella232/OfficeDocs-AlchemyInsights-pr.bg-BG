---
title: ConsistencyGuid / sourceAnchor поведение
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 5/2/2018
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: 6a44f797-acc7-4cbe-aa5a-47e2581fabf5
ms.openlocfilehash: cb1b50792b07a1b3b69607bf2f6824141a15922f
ms.sourcegitcommit: 9d78905c512192ffc4675468abd2efc5f2e4baf4
ms.translationtype: MT
ms.contentlocale: bg-BG
ms.lasthandoff: 04/23/2019
ms.locfileid: "32408097"
---
# <a name="consistencyguid--sourceanchor-behavior"></a><span data-ttu-id="b25a6-102">ConsistencyGuid / sourceAnchor поведение</span><span class="sxs-lookup"><span data-stu-id="b25a6-102">ConsistencyGuid / sourceAnchor behavior</span></span>

<span data-ttu-id="b25a6-103">Лазурно АД свързване (версия 1.1.524.0 и след) сега улеснява използването на МСС-ConsistencyGuid като sourceAnchor атрибут.</span><span class="sxs-lookup"><span data-stu-id="b25a6-103">Azure AD Connect (version 1.1.524.0 and after) now facilitates the use of msDS-ConsistencyGuid as sourceAnchor attribute.</span></span> <span data-ttu-id="b25a6-104">Когато използвате тази функция, Azure АД се свържете автоматично конфигурира синхронизация правилата към:</span><span class="sxs-lookup"><span data-stu-id="b25a6-104">When using this feature, Azure AD Connect automatically configures the synchronization rules to:</span></span>
  
- <span data-ttu-id="b25a6-105">Използвайте МСС-ConsistencyGuid като атрибут на sourceAnchor за потребителски обекти.</span><span class="sxs-lookup"><span data-stu-id="b25a6-105">Use msDS-ConsistencyGuid as the sourceAnchor attribute for User objects.</span></span> <span data-ttu-id="b25a6-106">ObjectGUID се използва за други типове обекти.</span><span class="sxs-lookup"><span data-stu-id="b25a6-106">ObjectGUID is used for other object types.</span></span>
    
- <span data-ttu-id="b25a6-107">За всяка дадена локалния AD потребителски обект, чиято МСС-ConsistencyGuid атрибут не е населена, Azure АД се свържете пише своята objectGUID стойност обратно към атрибута на МСС-ConsistencyGuid в локалната Active Directory.</span><span class="sxs-lookup"><span data-stu-id="b25a6-107">For any given on-premises AD User object whose msDS-ConsistencyGuid attribute isn't populated, Azure AD Connect writes its objectGUID value back to the msDS-ConsistencyGuid attribute in on-premises Active Directory.</span></span> <span data-ttu-id="b25a6-108">След МСС-ConsistencyGuid атрибут е населена, тогава Azure АД свържете експортира обект лазурно АД.</span><span class="sxs-lookup"><span data-stu-id="b25a6-108">After the msDS-ConsistencyGuid attribute is populated, Azure AD Connect then exports the object to Azure AD.</span></span>
    
 <span data-ttu-id="b25a6-109">**Забележка:** Веднъж локална реклама обект се импортира в Azure АД свържете (тоест, внесени в пространството на конектора на Рекламата и проектира в Metaverse), не можете да променяте стойността си sourceAnchor вече.</span><span class="sxs-lookup"><span data-stu-id="b25a6-109">**Note:** Once an on-premises AD object is imported into Azure AD Connect (that is, imported into the AD Connector Space and projected into the Metaverse), you cannot change its sourceAnchor value anymore.</span></span> <span data-ttu-id="b25a6-110">За да зададете стойността на sourceAnchor за дадена локална реклама обект, конфигуриране му МСС-ConsistencyGuid атрибут, преди то се импортира в Azure АД се свържете.</span><span class="sxs-lookup"><span data-stu-id="b25a6-110">To specify the sourceAnchor value for a given on-premises AD object, configure its msDS-ConsistencyGuid attribute before it is imported into Azure AD Connect.</span></span> 
  
<span data-ttu-id="b25a6-111">За повече информация за SourceAnchor и ConsistencyGuid, се отнасят до следното: [Azure АД свържете: дизайн концепции](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-design-concepts)</span><span class="sxs-lookup"><span data-stu-id="b25a6-111">For more information on SourceAnchor and ConsistencyGuid, refer to the following: [Azure AD Connect: Design concepts](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-design-concepts)</span></span>
  

