---
title: Dynamics 365 формуляри бизнес правила-правило за бизнес не стрелба за формуляр
ms.author: pebaum
author: pebaum
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1926"
- "6200018"
ms.openlocfilehash: 3cdd2175083e864b3bffc57a70bb6c6220843fad
ms.sourcegitcommit: b43f77221f47b50c41197a448a9c26c423ce1ad5
ms.translationtype: MT
ms.contentlocale: bg-BG
ms.lasthandoff: 11/15/2019
ms.locfileid: "37769328"
---
# <a name="onchange-event-does-not-occur-if-the-field-is-changed-programmatically"></a><span data-ttu-id="be056-102">OnChange събитие не възниква, ако полето се променя програмно</span><span class="sxs-lookup"><span data-stu-id="be056-102">OnChange event does not occur if the field is changed programmatically</span></span>

<span data-ttu-id="be056-103">Събитие *onChange* не възниква, ако полето се променя програмно с помощта на *атрибута.* [SetValue](https://docs.microsoft.com/dynamics365/customer-engagement/developer/clientapi/reference/attributes/setvalue) метод.</span><span class="sxs-lookup"><span data-stu-id="be056-103">The *OnChange* event does not occur if the field is changed programmatically using the *attribute.*[setValue](https://docs.microsoft.com/dynamics365/customer-engagement/developer/clientapi/reference/attributes/setvalue) method.</span></span> <span data-ttu-id="be056-104">Ако искате манипулатори за събития *onChange* да се стартира, след като зададете стойността, трябва да използвате *formконтекстно. data. обект атрибут* [fireonchange](https://docs.microsoft.com/dynamics365/customer-engagement/developer/clientapi/reference/attributes/fireonchange) в кода.</span><span class="sxs-lookup"><span data-stu-id="be056-104">If you want event handlers for the *OnChange* event to run after you set the value you must use the *formContext.data.entity attribute* [fireOnchange](https://docs.microsoft.com/dynamics365/customer-engagement/developer/clientapi/reference/attributes/fireonchange) method in your code.</span></span>

[https://docs.microsoft.com/dynamics365/customer-engagement/developer/clientapi/reference/events/attribute-onchange](https://docs.microsoft.com/dynamics365/customer-engagement/developer/clientapi/reference/events/attribute-onchange)
