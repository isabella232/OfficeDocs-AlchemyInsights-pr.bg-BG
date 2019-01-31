---
title: Условен достъп с Intune
ms.author: pebaum
author: pebaum
ms.date: 10/11/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.assetid: aecba7c5-e86d-4ec8-9d44-679f5a3d659d
ms.openlocfilehash: 3b50bc96a879017b62e42e1849f72e68408a0d9d
ms.sourcegitcommit: 0ae6cbb8cf2836da98300767ed81b411d6551bee
ms.translationtype: MT
ms.contentlocale: bg-BG
ms.lasthandoff: 01/30/2019
ms.locfileid: "29662316"
---
# <a name="conditional-access-with-intune"></a>Условен достъп с Intune

Използване на **Условен достъп** с Intune изисква три стъпки: 
  
- Създаване на **Условен достъп политика** , която дефинира какви ресурси са защитени, както и какви условия трябва да бъдат изпълнени за достъп до тези ресурси. Например устройството трябва да бъде съвместим преди достъп до корпоративни имейл. 
    
- Създаване на **Спазване на политиката** да дефинирате настройки, които трябва да бъдат изпълнени, преди устройството се счита съвместим. Например устройство трябва да има ПИН на най-малко 6 цифри преди се счита съвместим. 
    
- Гарантира **Съответствие политики** и **Условен достъп политики** са насочени към желаните групи от потребители. Това може да наложи създаването на специфични групи от потребители в Azure Active Directory. 
    
Прочетете още:
  
- [Условен достъп най-добрите практики](https://docs.microsoft.com/azure/active-directory/conditional-access/best-practices)
    
- [Запознаване с условен достъп](https://docs.microsoft.com/azure/active-directory/active-directory-conditional-access-azure-portal-get-started)
    

