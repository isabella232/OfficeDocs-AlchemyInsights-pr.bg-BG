---
title: Проблеми със съгласието на администратор
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 01/18/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004354"
- "7786"
ms.openlocfilehash: 6154b4b9cce51be3271cb25132f409319d8da14b
ms.sourcegitcommit: 113b802081101de70810fc73938ea92f7518d8c6
ms.translationtype: MT
ms.contentlocale: bg-BG
ms.lasthandoff: 01/18/2021
ms.locfileid: "49900778"
---
# <a name="admin-consent-issues"></a>Проблеми със съгласието на администратор

1. Разрешете [работния поток "съгласие на администратор](https://docs.microsoft.com/azure/active-directory/manage-apps/configure-admin-consent-workflow) ", за да позволите на потребителите да изискват одобрение от администратор директно от екрана за съгласие.

1. Ако вие или потребителите на вашето приложение виждате неочаквани грешки по време на процеса на одобрение, вижте тази статия за стъпките за отстраняване на неизправности: [неочаквана грешка при извършване на съгласие за приложение](https://docs.microsoft.com/azure/active-directory/manage-apps/application-sign-in-unexpected-user-consent-error).

1. Научете повече за [съгласието на администратора в платформата за самоличност на Microsoft](https://docs.microsoft.com/azure/active-directory/develop/v2-admin-consent), как работи [подканата за съгласие](https://docs.microsoft.com/azure/active-directory/develop/v2-admin-consent) и как да се [направи оценка на искане за съгласие от администратор на клиент](https://docs.microsoft.com/azure/active-directory/manage-apps/manage-consent-requests#evaluating-a-request-for-tenant-wide-admin-consent).

1. Приложенията, които се интегрират с платформата за самоличност на Microsoft, следват модел на удостоверяване, който дава на потребителите и администраторите контрол върху това как могат да бъдат отваряни данни. Прилагането на модела на удостоверяване е актуализирано на крайната точка на платформата за самоличност на Microsoft и това променя начина, по който приложението трябва да взаимодейства с платформата за самоличност на Microsoft. Вижте [разрешения и съгласие в крайната точка на платформата за самоличност на Microsoft](https://docs.microsoft.com/azure/active-directory/manage-apps/manage-consent-requests#evaluating-a-request-for-tenant-wide-admin-consent) за общ преглед на този модел на удостоверяване, включително обхвати, разрешения и съгласие.