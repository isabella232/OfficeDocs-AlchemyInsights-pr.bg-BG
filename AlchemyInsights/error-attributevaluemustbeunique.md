---
title: Атрибут за грешкаValueMustBeUnique
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
ms.assetid: bf8ac830-6f0c-4616-827d-987616700e59
ms.openlocfilehash: 35eb88624a5535e136ac1d01faf8e905bf00eb45
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: bg-BG
ms.lasthandoff: 04/15/2021
ms.locfileid: "51813749"
---
# <a name="error-attributevaluemustbeunique"></a>Грешка: AttributeValueMustBeUnique

Най-често срещаната причина за грешката AttributeValueMustBeUnique е два обекта с различен SourceAnchor (immutableId) имат една и съща стойност за атрибутите ProxyAddresses и/или UserPrincipalName. За да коригирате грешката AttributeValueMustBeUnique:
  
1. Идентифицирайте дублирания прокси Адрес, userPrincipalName или друга стойност на атрибута, която е причина за грешката. Също така определете кои два (или повече) обекта са включени в конфликта. Отчетът, генериран от Azure AD Connect Health за синхронизиране, може да ви помогне да идентифицирате двата обекта.
    
2. Определете кой обект трябва да продължи да има дублираната стойност и кой обект не трябва.
    
3. Премахнете дублираната стойност от обекта, който не би трябвало да има тази стойност. Обърнете внимание, че трябва да направите промяната в указателя, откъдето е източникът на обекта. В някои случаи може да се наложи да изтриете един от обектите в конфликт.
    
4. Ако сте направили промяната в локалната AD, оставете Azure AD Connect да синхронизира промяната, за да бъде коригирана грешката.
    

