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
# <a name="consistencyguid--sourceanchor-behavior"></a>КонсистенцияGuid / sourceAnchor поведение

Azure AD Connect (версия 1.1.524.0 и след) сега улеснява използването на атрибута msDS-ConsistencyGuid като източникAnchor. Когато използвате тази функция, Azure AD Connect автоматично конфигурира правилата за синхронизиране на:
  
- Използвайте msDS-ConsistencyGuid като атрибут sourceAnchor за потребителски обекти. ObjectGUID се използва за други типове обекти.
    
- За всеки обект на локалния ПОТРЕБИТЕЛ НА AD, чийто атрибут msDS-ConsistencyGuid не е попълнен, Azure AD Connect записва стойността си objectGUID обратно в атрибута msDS-ConsistencyGuid в локалния Active Directory. След като атрибутът msDS-ConsistencyGuid е попълнен, Azure AD Connect след това експортира обекта в Azure AD.
    
 **Забележка:** След като локалният AD обект бъде импортиран в Azure AD Connect (т.е. импортиран в пространството за КОНЕКТОР НА AD и прожектиран в метаверзата), вече не можете да променяте стойността му източникAnchor. За да зададете стойността източникAnchor за даден локално AD обект, конфигурирайте атрибута msDS-ConsistencyGuid, преди да бъде импортиран в Azure AD Connect. 
  
За повече информация относно SourceAnchor и ConsistencyGuid вижте следното: [Azure AD Connect: Концепции за проектиране](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-design-concepts)
  

