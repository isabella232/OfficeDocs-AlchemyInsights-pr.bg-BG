---
title: API Permissions and Consent
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 01/25/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004343"
- "7756"
ms.openlocfilehash: c45bab67d414c8f0f2ca1c5275084d4ecce538c5256154292302080ba5bd8175
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: bg-BG
ms.lasthandoff: 08/05/2021
ms.locfileid: "53932086"
---
# <a name="api-permissions-and-consent"></a>Разрешения и съгласие за API

Приложенията, които се интегрират с Платформа за самоличност на Microsoft следват модел на удостоверяване, който дава на потребителите и администраторите контрол върху това как могат да бъдат достъпни данните. Внедряването на модела на удостоверяване е актуализирано на Платформа за самоличност на Microsoft крайна точка. Той променя начина, по който дадено приложение трябва да взаимодейства с Платформа за самоличност на Microsoft. [Разрешенията и съгласието в крайната Платформа за самоличност на Microsoft обхваща](https://docs.microsoft.com/azure/active-directory/develop/v2-permissions-and-consent) основните понятия на този модел на удостоверяване, включително обхвати, разрешения и съгласие.

Рамката [Azure Active Directory за съгласие (Azure AD)](https://docs.microsoft.com/azure/active-directory/develop/consent-framework) улеснява разработването на уеб приложения за множество клиенти и основни клиентски приложения. Тези приложения позволяват влизане по потребителски акаунти от клиент на Azure AD, който е различен от този, в който е регистрирано приложението. Може също да се наложи да имат достъп до API за уеб, като например API на Microsoft Graph (за достъп до Azure AD, Intune и услуги в Microsoft 365) и други API на Услуги на Microsoft, в допълнение към вашите собствени API за уеб.

