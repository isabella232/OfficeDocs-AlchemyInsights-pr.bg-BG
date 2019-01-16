---
title: ConsistencyGuid / sourceAnchor поведение
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 5/2/2018
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom: Adm_O365
ms.assetid: 6a44f797-acc7-4cbe-aa5a-47e2581fabf5
ms.openlocfilehash: 80516ed9e15040475a8b65a1af98a1b561704d49
ms.sourcegitcommit: d6ea5e9458a2b8ceaab3ac4bd483e1130b9a398a
ms.translationtype: MT
ms.contentlocale: bg-BG
ms.lasthandoff: 01/15/2019
ms.locfileid: "28275839"
---
# <a name="consistencyguid--sourceanchor-behavior"></a>ConsistencyGuid / sourceAnchor поведение

Лазурно АД свързване (версия 1.1.524.0 и след) сега улеснява използването на МСС-ConsistencyGuid като sourceAnchor атрибут. Когато използвате тази функция, Azure АД се свържете автоматично конфигурира синхронизация правилата към:
  
- Използвайте МСС-ConsistencyGuid като атрибут на sourceAnchor за потребителски обекти. ObjectGUID се използва за други типове обекти.
    
- За всяка дадена локалния AD потребителски обект, чиято МСС-ConsistencyGuid атрибут не е населена, Azure АД се свържете пише своята objectGUID стойност обратно към атрибута на МСС-ConsistencyGuid в локалната Active Directory. След МСС-ConsistencyGuid атрибут е населена, тогава Azure АД свържете експортира обект лазурно АД.
    
 **Забележка:** Веднъж локална реклама обект се импортира в Azure АД свържете (тоест, внесени в пространството на конектора на Рекламата и проектира в Metaverse), не можете да променяте стойността си sourceAnchor вече. За да зададете стойността на sourceAnchor за дадена локална реклама обект, конфигуриране му МСС-ConsistencyGuid атрибут, преди то се импортира в Azure АД се свържете. 
  
За повече информация за SourceAnchor и ConsistencyGuid, се отнасят до следното: [Azure АД свържете: дизайн концепции](https://docs.microsoft.com/en-us/azure/active-directory/connect/active-directory-aadconnect-design-concepts)
  

