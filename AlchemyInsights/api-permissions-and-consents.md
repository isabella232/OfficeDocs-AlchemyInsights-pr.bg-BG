---
title: Разрешения и съгласие с API
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
ms.openlocfilehash: c99e5e2e8fb9bcc88e5221890ed9c28ed9e7d0c8
ms.sourcegitcommit: 605a73b159d30634b064c1b63b0e734ceb3fdec8
ms.translationtype: MT
ms.contentlocale: bg-BG
ms.lasthandoff: 01/25/2021
ms.locfileid: "49974260"
---
# <a name="api-permissions-and-consent"></a>Разрешения и съгласие с API

Приложенията, които се интегрират с платформата за самоличност на Microsoft, следват модел на удостоверяване, който дава на потребителите и администраторите контрол върху това как могат да бъдат отваряни данни. Прилагането на модела на удостоверяване е актуализирано на крайната точка на платформата за самоличност на Microsoft. Той променя начина, по който приложението трябва да взаимодейства с платформата за самоличност на Microsoft. [Разрешенията и съгласието в крайна точка на платформата за самоличност на Microsoft](https://docs.microsoft.com/azure/active-directory/develop/v2-permissions-and-consent) обхващат основните понятия на този модел на удостоверяване, включително обхвати, разрешения и съгласие.

[Рамката за съгласие на Azure Active Directory (AZURE ad)](https://docs.microsoft.com/azure/active-directory/develop/consent-framework) улеснява създаването на уеб приложения и приложенията на родния клиент на множество клиенти. Тези приложения разрешават влизане чрез потребителски акаунти от клиент на Azure AD, който е различен от този, в който е регистрирано приложението. Можете също да се наложи да получите достъп до уеб API, като например API за Microsoft Graph (за достъп до Azure AD, настройки и услуги в Microsoft 365) и други API за Microsoft Services, в допълнение към собствените си уеб API.

