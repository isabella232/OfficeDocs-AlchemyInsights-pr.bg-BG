---
title: Стойността на атрибута на грешката трябва да бъде уникална
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: bf8ac830-6f0c-4616-827d-987616700e59
ms.openlocfilehash: fa1fdb35f1af250bc98aa61c0e5111f1f1b8aac4
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: bg-BG
ms.lasthandoff: 04/22/2020
ms.locfileid: "43703163"
---
# <a name="error-attributevaluemustbeunique"></a>Грешка: АтрибутстойностТрябвадабъдеуникален

Най-честата причина за грешка attributeValueMustBeUnique е два обекта с различни SourceAnchor (immutableId) имат същата стойност за атрибутите ProxyAddresses и/или UserPrincipalName. За да коригирате грешката AttributeValueMustBeUnique:
  
1. Проверете дублирани proxyAddresses, userPrincipalName или други атрибут стойност, която причинява грешката. Също така да се определи кои два (или повече) обекта са включени в конфликта. Отчет, генериран от Azure AD свързване на здравето за синхронизиране може да ви помогне да идентифицирате двата обекта.
    
2. Определете кой обект трябва да продължи да има дублирана стойност и кой обект не трябва.
    
3. Премахнете дублираната стойност от обекта, който не трябва да има тази стойност. Имайте предвид, че трябва да направите промяната в директорията, от която е сизточник на обекта. В някои случаи може да се наложи да изтриете един от обектите в конфликт.
    
4. Ако сте направили промяна та на помещения AD, нека Azure AD свързване синхронизиране на промяната за грешка, за да се фиксира.
    

