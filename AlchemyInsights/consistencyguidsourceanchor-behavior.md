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
ms.openlocfilehash: 9b5765ff3c59b1312bead41a45a53478a96260df0567f006ab93c3ccfaf4be64
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: bg-BG
ms.lasthandoff: 08/05/2021
ms.locfileid: "54044329"
---
# <a name="consistencyguid--sourceanchor-behavior"></a>КонсистенцияGuid / sourceAnchor поведение

Azure AD Свързване (версия 1.1.524.0 и след) сега улеснява използването на атрибута msDS-ConsistencyGuid като източникAnchor. Когато използвате тази функция, Azure AD Свързване автоматично конфигурира правилата за синхронизиране на:
  
- Използвайте msDS-ConsistencyGuid като атрибут sourceAnchor за потребителски обекти. ObjectGUID се използва за други типове обекти.
    
- За всеки обект на потребител на локалния AD, чийто атрибут msDS-ConsistencyGuid не е попълнен, Azure AD Свързване записва стойността си objectGUID обратно в атрибута msDS-ConsistencyGuid в локалния Active Directory. След като атрибутът msDS-ConsistencyGuid е попълнен, Azure AD Свързване след това експортира обекта в Azure AD.
    
 **Забележка:** След като локалният AD обект бъде импортиран в Azure AD Свързване (т.е. импортиран в пространството на AD Connector и прожектиран в Метаверс), вече не можете да променяте стойността му източникAnchor. За да зададете стойността източникAnchor за даден локално ad обект, конфигурирайте неговия атрибут msDS-ConsistencyGuid, преди да бъде импортиран в Azure AD Свързване. 
  
За повече информация относно SourceAnchor и ConsistencyGuid вижте следното: [Azure AD Свързване: Концепции за проектиране](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-design-concepts)
  

