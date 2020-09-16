---
title: ConsistencyGuid/sourceAnchor поведение
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: 6a44f797-acc7-4cbe-aa5a-47e2581fabf5
ms.openlocfilehash: adac469328485696d1ee1532aa3d6828af0642eb
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: bg-BG
ms.lasthandoff: 09/14/2020
ms.locfileid: "47756272"
---
# <a name="consistencyguid--sourceanchor-behavior"></a><span data-ttu-id="9c48b-102">ConsistencyGuid/sourceAnchor поведение</span><span class="sxs-lookup"><span data-stu-id="9c48b-102">ConsistencyGuid / sourceAnchor behavior</span></span>

<span data-ttu-id="9c48b-103">Azure AD Connect (версия 1.1.524.0 и After) сега улеснява използването на МСС – ConsistencyGuid като sourceAnchor атрибут.</span><span class="sxs-lookup"><span data-stu-id="9c48b-103">Azure AD Connect (version 1.1.524.0 and after) now facilitates the use of msDS-ConsistencyGuid as sourceAnchor attribute.</span></span> <span data-ttu-id="9c48b-104">При използването на тази функция Azure AD Connect автоматично конфигурира правилата за синхронизиране с:</span><span class="sxs-lookup"><span data-stu-id="9c48b-104">When using this feature, Azure AD Connect automatically configures the synchronization rules to:</span></span>
  
- <span data-ttu-id="9c48b-105">Използвайте МСС – ConsistencyGuid като атрибут sourceAnchor за потребителските обекти.</span><span class="sxs-lookup"><span data-stu-id="9c48b-105">Use msDS-ConsistencyGuid as the sourceAnchor attribute for User objects.</span></span> <span data-ttu-id="9c48b-106">ObjectGUID се използва за други типове обекти.</span><span class="sxs-lookup"><span data-stu-id="9c48b-106">ObjectGUID is used for other object types.</span></span>
    
- <span data-ttu-id="9c48b-107">За всеки даден локален РЕКЛАМен потребителски обект, чийто атрибут на ConsistencyGuid не е попълнен, Azure AD Connect записва своята objectGUID стойност обратно към МСС – ConsistencyGuid атрибут в локален Active Directory.</span><span class="sxs-lookup"><span data-stu-id="9c48b-107">For any given on-premises AD User object whose msDS-ConsistencyGuid attribute isn't populated, Azure AD Connect writes its objectGUID value back to the msDS-ConsistencyGuid attribute in on-premises Active Directory.</span></span> <span data-ttu-id="9c48b-108">След като МСС – ConsistencyGuid атрибутът е населен, Azure AD Connect и експортира обекта в Azure AD.</span><span class="sxs-lookup"><span data-stu-id="9c48b-108">After the msDS-ConsistencyGuid attribute is populated, Azure AD Connect then exports the object to Azure AD.</span></span>
    
 <span data-ttu-id="9c48b-109">**Забележка:** След като локален РЕКЛАМен обект бъде импортиран в Azure AD Connect (който е внесен в РЕКЛАМното поле за конектор и е прожектиран в Metaverse), повече не можете да променяте стойността на sourceAnchor.</span><span class="sxs-lookup"><span data-stu-id="9c48b-109">**Note:** Once an on-premises AD object is imported into Azure AD Connect (that is, imported into the AD Connector Space and projected into the Metaverse), you cannot change its sourceAnchor value anymore.</span></span> <span data-ttu-id="9c48b-110">За да зададете стойността на sourceAnchor за даден локален РЕКЛАМен обект, конфигурирайте неговия ConsistencyGuid атрибут за msDS, преди да бъде импортиран в Azure AD Connect.</span><span class="sxs-lookup"><span data-stu-id="9c48b-110">To specify the sourceAnchor value for a given on-premises AD object, configure its msDS-ConsistencyGuid attribute before it is imported into Azure AD Connect.</span></span> 
  
<span data-ttu-id="9c48b-111">За повече информация относно SourceAnchor и ConsistencyGuid вижте следното: [AZURE ad Connect: концепции за проектиране](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-design-concepts)</span><span class="sxs-lookup"><span data-stu-id="9c48b-111">For more information on SourceAnchor and ConsistencyGuid, refer to the following: [Azure AD Connect: Design concepts](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-design-concepts)</span></span>
  

