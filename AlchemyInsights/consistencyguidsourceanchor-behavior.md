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
# <a name="consistencyguid--sourceanchor-behavior"></a>Съвместимост с Последователиguid/източник

Azure AD свързване (версия 1.1.524.0 и след) сега улеснява използването на МСС Последователстенguid като sourceAnchor атрибут. Когато използвате тази функция, Azure AD Connect автоматично конфигурира правилата за синхронизация на:
  
- Използване на МСС съгласуваност Иguid като sourceAnchor атрибут за обекти на потребителя. Обектguid се използва за други типове обекти.
    
- За всеки даден локален AD потребителски обект, чиято МСС съгласуваност Encyguid атрибут не се попълва, Azure AD свързване записва Обектаguid стойност обратно МСС съгласуваност Encyguid атрибут в локалната Active Directory. След като МСС съгласуваност Encyguid атрибут се попълва, Azure AD свързване след експортира обекта Azure AD.
    
 **Забележка:** След като локалния AD обект се импортира в Azure AD свързване (т. е. импортирани в AD конектор пространство и планирани в Метастих), не можете да променяте стойността му вече. За да укажете стойността sourceAnchor за даден локален AD обект, конфигурирайте МСС съгласуваност Encyguid атрибут, преди да се импортира в Azure AD свързване. 
  
За повече информация относно източник на котва и съвместимост, вижте следното: [AZURE ad свързване: дизайн концепции](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-design-concepts)
  

