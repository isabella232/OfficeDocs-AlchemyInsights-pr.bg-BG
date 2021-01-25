---
title: Съпоставяне на атрибутите на потребителите
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 01/22/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "7851"
- "9004348"
ms.openlocfilehash: 8bbf554c533d960a304901d7cbb492b87e9bec71
ms.sourcegitcommit: 953a8567ebcd9835f8c5c49472b223107c92549b
ms.translationtype: MT
ms.contentlocale: bg-BG
ms.lasthandoff: 01/22/2021
ms.locfileid: "49949649"
---
# <a name="user-provisioning-attribute-mapping"></a>Съпоставяне на атрибутите на потребителите

1. За да отстраните известни проблеми със съпоставянето на атрибута, вижте [съпоставяния на атрибути](https://docs.microsoft.com/azure/active-directory/app-provisioning/known-issues#attribute-mappings). 
2. Microsoft Azure Active Directory (AD) предоставя поддръжка за осигуряването на потребители за приложения на други разработчици, като например Salesforce, G Suite и други. Ако разрешите осигуряването на потребителя за приложение за SaaS от друг разработчик, порталът на Azure управлява стойностите на атрибута си чрез нанасяне на атрибут. За да научите как да персонализирате атрибутите по подразбиране, вижте [Персонализиране на атрибута за осигуряване на потребители – съпоставяния за SaaS приложения в Azure Active Directory](https://docs.microsoft.com/azure/active-directory/app-provisioning/customize-application-attributes).
    - За да научите повече за осигуряването на потребителите в SaaS App, вижте [Какво представлява автоматизираното приложение за SaaS потребители в AZURE ad?](https://docs.microsoft.com/azure/active-directory/app-provisioning/user-provisioning) 
3. При персонализиране на атрибута за съпоставяне на потребителски провизии е възможно да откриете, че атрибутът, който искате да съпоставите, не се показва в списъка на атрибута източник. [Свойството синхронизиране на атрибут от локален указател на Active Directory в AZURE ad за осигуряване на](https://docs.microsoft.com/azure/active-directory/app-provisioning/user-provisioning-sync-attributes-for-mapping) статия за приложения ви показва как да добавите липсващия атрибут, като го синхронизирате от локалната си реклама в Azure ad.
