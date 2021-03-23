---
title: Отстраняване на грешки при удостоверяване на Azure AD и упълномощаване (AADSTS)
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 03/19/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9800"
- "9005744"
ms.openlocfilehash: 14555dfcb1406fd3a3977012393714a713ff80dc
ms.sourcegitcommit: c08bed4071baa3bb5879496df3ed44fb828c8367
ms.translationtype: MT
ms.contentlocale: bg-BG
ms.lasthandoff: 03/19/2021
ms.locfileid: "51034971"
---
# <a name="troubleshoot-azure-ad-authentication-and-authorization-aadsts-error-codes"></a>Отстраняване на грешки при удостоверяване на Azure AD и упълномощаване (AADSTS)

За да разрешите кодовете на грешка за удостоверяване на пад и упълномощаване (AADSTS), изпълнете следните Препоръчителни стъпки:

1. **Обработване на кодове на грешка в приложението**

- **OAuth 2.0 Spec**, https://tools.ietf.org/html/rfc6749#section-5.2 предоставя насоки как да се обработват грешки по време на удостоверяване, като се използва грешката част от отговора на грешката.

    - **грешка**: низ на код на грешка, който може да се използва за класифицирането на типове грешки, които възникват, и трябва да се използва за реагиране на грешки.
    - Полето за **грешка** има няколко възможни стойности – прегледайте връзките с документацията за протокола и OAuth 2,0 спецификациите за повече информация за конкретни грешки и как да ги реагирате.

- Ето примерен отговор на грешка:
```
{
  "error": "invalid_scope",
  "error_description": "AADSTS70011: The provided value for the input parameter 'scope' is not 
valid. The scope https://example.contoso.com/activity.read is not valid.\r\nTrace ID: 255d1aef- 8c98-452f-ac51-23d051240864\r\nCorrelation ID: fb3d2015-bc17-4bb9-bb85-30c5cf1aaaa7\r\nTimestamp: 2016-01-09 02:02:12Z",
  "error_codes": [
    70011
  ],
  "timestamp": "2016-01-09 02:02:12Z",
  "trace_id": "255d1aef-8c98-452f-ac51-23d051240864",
  "correlation_id": "fb3d2015-bc17-4bb9-bb85-30c5cf1aaaa7", 
  "error_uri":"https://login.microsoftonline.com/error?code=70011"
}
```
2. **Справка за актуална информация за код на грешка**

- Кодовете на грешки и съобщенията подлежат на промяна. За най-актуална информация вижте страницата, https://login.microsoftonline.com/error за да намерите описания на грешки, корекции на AADSTS и някои предложени заобиколни решения.
- Можете също да потърсите и отстраните [кодове за грешка на AADSTS](https://docs.microsoft.com/azure/active-directory/develop/reference-aadsts-error-codes#aadsts-error-codes) , описани в кодовете на грешки при удостоверяване на статия [Azure ad и упълномощаване](https://docs.microsoft.com/azure/active-directory/develop/reference-aadsts-error-codes#handling-error-codes-in-your-application).

3. **Получаване на помощ**

- [Опции за поддръжка и помощ за разработчиците](https://docs.microsoft.com/azure/active-directory/develop/developer-support-help-options) – ако ви е нужен отговор на въпрос или помощ при решаването на проблем, който не е обхванат от нашата документация, може би е време да се свържете с експертите за помощ. Тази статия предоставя няколко предложения за получаване на отговори на вашите въпроси при разработване на приложения, които се интегрират с платформата за самоличност на Microsoft.








