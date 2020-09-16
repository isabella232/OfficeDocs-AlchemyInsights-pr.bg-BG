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
# <a name="consistencyguid--sourceanchor-behavior"></a>ConsistencyGuid/sourceAnchor поведение

Azure AD Connect (версия 1.1.524.0 и After) сега улеснява използването на МСС – ConsistencyGuid като sourceAnchor атрибут. При използването на тази функция Azure AD Connect автоматично конфигурира правилата за синхронизиране с:
  
- Използвайте МСС – ConsistencyGuid като атрибут sourceAnchor за потребителските обекти. ObjectGUID се използва за други типове обекти.
    
- За всеки даден локален РЕКЛАМен потребителски обект, чийто атрибут на ConsistencyGuid не е попълнен, Azure AD Connect записва своята objectGUID стойност обратно към МСС – ConsistencyGuid атрибут в локален Active Directory. След като МСС – ConsistencyGuid атрибутът е населен, Azure AD Connect и експортира обекта в Azure AD.
    
 **Забележка:** След като локален РЕКЛАМен обект бъде импортиран в Azure AD Connect (който е внесен в РЕКЛАМното поле за конектор и е прожектиран в Metaverse), повече не можете да променяте стойността на sourceAnchor. За да зададете стойността на sourceAnchor за даден локален РЕКЛАМен обект, конфигурирайте неговия ConsistencyGuid атрибут за msDS, преди да бъде импортиран в Azure AD Connect. 
  
За повече информация относно SourceAnchor и ConsistencyGuid вижте следното: [AZURE ad Connect: концепции за проектиране](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-design-concepts)
  

