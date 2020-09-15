---
title: Грешка AttributeValueMustBeUnique
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
ms.assetid: bf8ac830-6f0c-4616-827d-987616700e59
ms.openlocfilehash: 4627a7ae34b0dd9f16538ef75ac8792672dcc056
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: bg-BG
ms.lasthandoff: 09/14/2020
ms.locfileid: "47709140"
---
# <a name="error-attributevaluemustbeunique"></a>Грешка: AttributeValueMustBeUnique

Най-честата причина за грешката на AttributeValueMustBeUnique е два обекта с различен SourceAnchor (immutableId) имат еднаква стойност за атрибутите ProxyAddresses и/или UserPrincipalName. За да коригирате грешката на AttributeValueMustBeUnique:
  
1. Определете дублираната стойност на proxyAddresses, userPrincipalName или друг атрибут, което е причина за грешката. Също така Определете кои два (или повече) обекта са включени в конфликта. Докладът, генериран от Azure AD Connect Health за синхронизиране, може да ви помогне да идентифицирате двата обекта.
    
2. Определяне кой обект трябва да продължи да използва дублираната стойност и кой обект не трябва.
    
3. Отстранете дублираната стойност от обекта, който не трябва да има тази стойност. Имайте предвид, че трябва да направите промяната в директорията, от която е източникът на обекта. В някои случаи може да се наложи да изтриете един от конфликтните обекти.
    
4. Ако сте направили промяната в локалната реклама, оставете Azure AD Connect да синхронизира промяната за грешката, за да се поправи.
    

