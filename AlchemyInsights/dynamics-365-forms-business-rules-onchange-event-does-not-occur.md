---
title: Dynamics 365 образува бизнес правила - бизнес правило не стрелба за формуляр
ms.author: pebaum
author: pebaum
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1926"
- "6200018"
ms.openlocfilehash: 4ade8d2f68b465298e2d6efff3eef4f04f25c3bf
ms.sourcegitcommit: a413a0e27ef4ab8c484fa9fccff8bbef381c8b96
ms.translationtype: MT
ms.contentlocale: bg-BG
ms.lasthandoff: 07/16/2019
ms.locfileid: "35746943"
---
# <a name="onchange-event-does-not-occur-if-the-field-is-changed-programmatically"></a>OnChange събитие не се случи, ако програмно промяна на полето

Събитието *OnChange* не възниква ако полето е променен програмно използване *атрибут.* [setValue](https://docs.microsoft.com/en-us/dynamics365/customer-engagement/developer/clientapi/reference/attributes/setvalue) метод. Ако искате манипулатори на събитие за *OnChange* събитие, за да стартирате, след като зададете стойност, трябва да използвате *formContext.data.entity атрибут.* [fireOnchange](https://docs.microsoft.com/en-us/dynamics365/customer-engagement/developer/clientapi/reference/attributes/fireonchange) метод в кода си.

[https://docs.microsoft.com/dynamics365/customer-engagement/developer/clientapi/reference/events/attribute-onchange](https://docs.microsoft.com/en-us/dynamics365/customer-engagement/developer/clientapi/reference/events/attribute-onchange)
