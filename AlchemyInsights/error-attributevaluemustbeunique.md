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
ms.openlocfilehash: 37d6764d19d9cfbb0899a5ab85a4b1530896568adc364122075b7d6f2a32970a
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: bg-BG
ms.lasthandoff: 08/05/2021
ms.locfileid: "54002109"
---
# <a name="error-attributevaluemustbeunique"></a>Грешка: AttributeValueMustBeUnique

Най-често срещаната причина за грешката AttributeValueMustBeUnique е два обекта с различен SourceAnchor (immutableId) имат една и съща стойност за атрибутите ProxyAddresses и/или UserPrincipalName. За да коригирате грешката AttributeValueMustBeUnique:
  
1. Идентифицирайте дублирания прокси Адрес, userPrincipalName или друга стойност на атрибута, която е причина за грешката. Също така определете кои два (или повече) обекта са включени в конфликта. Отчетът, генериран от Azure AD Свързване изцели за синхронизиране, може да ви помогне да идентифицирате двата обекта.
    
2. Определете кой обект трябва да продължи да има дублираната стойност и кой обект не трябва.
    
3. Премахнете дублираната стойност от обекта, който не би трябвало да има тази стойност. Обърнете внимание, че трябва да направите промяната в указателя, откъдето е източникът на обекта. В някои случаи може да се наложи да изтриете един от обектите в конфликт.
    
4. Ако сте направили промяната в локалната AD, оставете Azure AD Свързване да синхронизира промяната, за да се коригира грешката.
    

