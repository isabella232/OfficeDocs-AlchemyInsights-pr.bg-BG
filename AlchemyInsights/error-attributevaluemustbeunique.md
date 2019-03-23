---
title: Грешка AttributeValueMustBeUnique
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 3/20/2018
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: bf8ac830-6f0c-4616-827d-987616700e59
ms.openlocfilehash: 7fc1190fb7b93dce945e366cf8b90112a97a2f3f
ms.sourcegitcommit: 03a156a9c9740521155a30775492c7dff0982588
ms.translationtype: MT
ms.contentlocale: bg-BG
ms.lasthandoff: 03/22/2019
ms.locfileid: "30766013"
---
# <a name="error-attributevaluemustbeunique"></a>Грешка: AttributeValueMustBeUnique

Най-честата причина за AttributeValueMustBeUnique грешката е две тела с различни SourceAnchor (immutableId) имат същата стойност за ProxyAddresses и/или UserPrincipalName атрибути. За да поправите грешка AttributeValueMustBeUnique:
  
1. Идентифицират дублирани proxyAddresses, userPrincipalName или други стойност на атрибут, който причинява грешката. Също така идентифицира които две (или повече) обекти са въвлечени в конфликта. Докладът, генерирани от Azure АД свържете здраве за синхронизация може да ви помогне да идентифицирате два обекта.
    
2. Идентифицира кой обект трябва да продължат да имат стойността на дублирани и кой обект не трябва.
    
3. Премахнете дублираните стойност от обекта, който не трябва да има тази стойност. Обърнете внимание, че трябва да направите промяната в директорията, където обектът е с произход от. В някои случаи може да се наложи да изтриете някой от обектите в конфликт.
    
4. Ако сте направили промяната в на помещения, реклама, нека Azure АД се свържете синхронизира промени за грешката да се оправят.
    

