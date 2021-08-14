---
title: Бизнес правила на Dynamics 365 Forms – бизнес правило, което не се използва за формуляр
ms.author: pebaum
author: pebaum
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1926"
- "6200018"
ms.openlocfilehash: 8425918950e1ef6c44f2866e6fa8987fe165536ae21e08ea6a1da880f761d512
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: bg-BG
ms.lasthandoff: 08/05/2021
ms.locfileid: "53947288"
---
# <a name="onchange-event-does-not-occur-if-the-field-is-changed-programmatically"></a>Събитието OnChange не възниква, ако полето се променя програмно

Събитието *OnChange* не възниква, ако полето се променя програмно с помощта на *атрибута.* [setValue](https://docs.microsoft.com/dynamics365/customer-engagement/developer/clientapi/reference/attributes/setvalue) метод. Ако искате манипулаторите на събития за *събитието OnChange* да се изпълняват, след като зададете стойността, трябва да използвате метода [fireOnchange на атрибута](https://docs.microsoft.com/dynamics365/customer-engagement/developer/clientapi/reference/attributes/fireonchange) *formContext.data.entity* във вашия код.

[https://docs.microsoft.com/dynamics365/customer-engagement/developer/clientapi/reference/events/attribute-onchange](https://docs.microsoft.com/dynamics365/customer-engagement/developer/clientapi/reference/events/attribute-onchange)
