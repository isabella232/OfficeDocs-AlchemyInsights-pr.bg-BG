---
title: КонсистенцияGuid / sourceAnchor поведение
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
ms.assetid: 6a44f797-acc7-4cbe-aa5a-47e2581fabf5
ms.openlocfilehash: eafe1ec9636cddc9d73a88beb7ae3ad9f6fad660
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: bg-BG
ms.lasthandoff: 04/15/2021
ms.locfileid: "51816981"
---
# <a name="consistencyguid--sourceanchor-behavior"></a><span data-ttu-id="b1ea7-102">КонсистенцияGuid / sourceAnchor поведение</span><span class="sxs-lookup"><span data-stu-id="b1ea7-102">ConsistencyGuid / sourceAnchor behavior</span></span>

<span data-ttu-id="b1ea7-103">Azure AD Connect (версия 1.1.524.0 и след) сега улеснява използването на атрибута msDS-ConsistencyGuid като източникAnchor.</span><span class="sxs-lookup"><span data-stu-id="b1ea7-103">Azure AD Connect (version 1.1.524.0 and after) now facilitates the use of msDS-ConsistencyGuid as sourceAnchor attribute.</span></span> <span data-ttu-id="b1ea7-104">Когато използвате тази функция, Azure AD Connect автоматично конфигурира правилата за синхронизиране на:</span><span class="sxs-lookup"><span data-stu-id="b1ea7-104">When using this feature, Azure AD Connect automatically configures the synchronization rules to:</span></span>
  
- <span data-ttu-id="b1ea7-105">Използвайте msDS-ConsistencyGuid като атрибут sourceAnchor за потребителски обекти.</span><span class="sxs-lookup"><span data-stu-id="b1ea7-105">Use msDS-ConsistencyGuid as the sourceAnchor attribute for User objects.</span></span> <span data-ttu-id="b1ea7-106">ObjectGUID се използва за други типове обекти.</span><span class="sxs-lookup"><span data-stu-id="b1ea7-106">ObjectGUID is used for other object types.</span></span>
    
- <span data-ttu-id="b1ea7-107">За всеки обект на локалния ПОТРЕБИТЕЛ НА AD, чийто атрибут msDS-ConsistencyGuid не е попълнен, Azure AD Connect записва стойността си objectGUID обратно в атрибута msDS-ConsistencyGuid в локалния Active Directory.</span><span class="sxs-lookup"><span data-stu-id="b1ea7-107">For any given on-premises AD User object whose msDS-ConsistencyGuid attribute isn't populated, Azure AD Connect writes its objectGUID value back to the msDS-ConsistencyGuid attribute in on-premises Active Directory.</span></span> <span data-ttu-id="b1ea7-108">След като атрибутът msDS-ConsistencyGuid е попълнен, Azure AD Connect след това експортира обекта в Azure AD.</span><span class="sxs-lookup"><span data-stu-id="b1ea7-108">After the msDS-ConsistencyGuid attribute is populated, Azure AD Connect then exports the object to Azure AD.</span></span>
    
 <span data-ttu-id="b1ea7-109">**Забележка:** След като локалният AD обект бъде импортиран в Azure AD Connect (т.е. импортиран в пространството за КОНЕКТОР НА AD и прожектиран в метаверзата), вече не можете да променяте стойността му източникAnchor.</span><span class="sxs-lookup"><span data-stu-id="b1ea7-109">**Note:** Once an on-premises AD object is imported into Azure AD Connect (that is, imported into the AD Connector Space and projected into the Metaverse), you cannot change its sourceAnchor value anymore.</span></span> <span data-ttu-id="b1ea7-110">За да зададете стойността източникAnchor за даден локално AD обект, конфигурирайте атрибута msDS-ConsistencyGuid, преди да бъде импортиран в Azure AD Connect.</span><span class="sxs-lookup"><span data-stu-id="b1ea7-110">To specify the sourceAnchor value for a given on-premises AD object, configure its msDS-ConsistencyGuid attribute before it is imported into Azure AD Connect.</span></span> 
  
<span data-ttu-id="b1ea7-111">За повече информация относно SourceAnchor и ConsistencyGuid вижте следното: [Azure AD Connect: Концепции за проектиране](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-design-concepts)</span><span class="sxs-lookup"><span data-stu-id="b1ea7-111">For more information on SourceAnchor and ConsistencyGuid, refer to the following: [Azure AD Connect: Design concepts](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-design-concepts)</span></span>
  

