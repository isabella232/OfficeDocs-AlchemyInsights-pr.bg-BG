---
title: Съвместимост с Последователиguid/източник
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
ms.openlocfilehash: f0ff94a8e46f1fb4e0ac8653c51f8f651e29498b
ms.sourcegitcommit: b43f77221f47b50c41197a448a9c26c423ce1ad5
ms.translationtype: MT
ms.contentlocale: bg-BG
ms.lasthandoff: 11/15/2019
ms.locfileid: "36516959"
---
# <a name="consistencyguid--sourceanchor-behavior"></a><span data-ttu-id="9000a-102">Съвместимост с Последователиguid/източник</span><span class="sxs-lookup"><span data-stu-id="9000a-102">ConsistencyGuid / sourceAnchor behavior</span></span>

<span data-ttu-id="9000a-103">Azure AD свързване (версия 1.1.524.0 и след) сега улеснява използването на МСС Последователстенguid като sourceAnchor атрибут.</span><span class="sxs-lookup"><span data-stu-id="9000a-103">Azure AD Connect (version 1.1.524.0 and after) now facilitates the use of msDS-ConsistencyGuid as sourceAnchor attribute.</span></span> <span data-ttu-id="9000a-104">Когато използвате тази функция, Azure AD Connect автоматично конфигурира правилата за синхронизация на:</span><span class="sxs-lookup"><span data-stu-id="9000a-104">When using this feature, Azure AD Connect automatically configures the synchronization rules to:</span></span>
  
- <span data-ttu-id="9000a-105">Използване на МСС съгласуваност Иguid като sourceAnchor атрибут за обекти на потребителя.</span><span class="sxs-lookup"><span data-stu-id="9000a-105">Use msDS-ConsistencyGuid as the sourceAnchor attribute for User objects.</span></span> <span data-ttu-id="9000a-106">Обектguid се използва за други типове обекти.</span><span class="sxs-lookup"><span data-stu-id="9000a-106">ObjectGUID is used for other object types.</span></span>
    
- <span data-ttu-id="9000a-107">За всеки даден локален AD потребителски обект, чиято МСС съгласуваност Encyguid атрибут не се попълва, Azure AD свързване записва Обектаguid стойност обратно МСС съгласуваност Encyguid атрибут в локалната Active Directory.</span><span class="sxs-lookup"><span data-stu-id="9000a-107">For any given on-premises AD User object whose msDS-ConsistencyGuid attribute isn't populated, Azure AD Connect writes its objectGUID value back to the msDS-ConsistencyGuid attribute in on-premises Active Directory.</span></span> <span data-ttu-id="9000a-108">След като МСС съгласуваност Encyguid атрибут се попълва, Azure AD свързване след експортира обекта Azure AD.</span><span class="sxs-lookup"><span data-stu-id="9000a-108">After the msDS-ConsistencyGuid attribute is populated, Azure AD Connect then exports the object to Azure AD.</span></span>
    
 <span data-ttu-id="9000a-109">**Забележка:** След като локалния AD обект се импортира в Azure AD свързване (т. е. импортирани в AD конектор пространство и планирани в Метастих), не можете да променяте стойността му вече.</span><span class="sxs-lookup"><span data-stu-id="9000a-109">**Note:** Once an on-premises AD object is imported into Azure AD Connect (that is, imported into the AD Connector Space and projected into the Metaverse), you cannot change its sourceAnchor value anymore.</span></span> <span data-ttu-id="9000a-110">За да укажете стойността sourceAnchor за даден локален AD обект, конфигурирайте МСС съгласуваност Encyguid атрибут, преди да се импортира в Azure AD свързване.</span><span class="sxs-lookup"><span data-stu-id="9000a-110">To specify the sourceAnchor value for a given on-premises AD object, configure its msDS-ConsistencyGuid attribute before it is imported into Azure AD Connect.</span></span> 
  
<span data-ttu-id="9000a-111">За повече информация относно източник на котва и съвместимост, вижте следното: [AZURE ad свързване: дизайн концепции](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-design-concepts)</span><span class="sxs-lookup"><span data-stu-id="9000a-111">For more information on SourceAnchor and ConsistencyGuid, refer to the following: [Azure AD Connect: Design concepts](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-design-concepts)</span></span>
  

