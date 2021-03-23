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
# <a name="troubleshoot-azure-ad-authentication-and-authorization-aadsts-error-codes"></a><span data-ttu-id="ac502-102">Отстраняване на грешки при удостоверяване на Azure AD и упълномощаване (AADSTS)</span><span class="sxs-lookup"><span data-stu-id="ac502-102">Troubleshoot Azure AD Authentication and Authorization (AADSTS) error codes</span></span>

<span data-ttu-id="ac502-103">За да разрешите кодовете на грешка за удостоверяване на пад и упълномощаване (AADSTS), изпълнете следните Препоръчителни стъпки:</span><span class="sxs-lookup"><span data-stu-id="ac502-103">To resolve AAD authentication and authorization error codes (AADSTS), perform the following recommended steps:</span></span>

1. <span data-ttu-id="ac502-104">**Обработване на кодове на грешка в приложението**</span><span class="sxs-lookup"><span data-stu-id="ac502-104">**Handling error codes in your application**</span></span>

- <span data-ttu-id="ac502-105">**OAuth 2.0 Spec**, https://tools.ietf.org/html/rfc6749#section-5.2 предоставя насоки как да се обработват грешки по време на удостоверяване, като се използва грешката част от отговора на грешката.</span><span class="sxs-lookup"><span data-stu-id="ac502-105">The **OAuth2.0 spec**, https://tools.ietf.org/html/rfc6749#section-5.2, provides guidance on how to handle errors during authentication using the error portion of the error response.</span></span>

    - <span data-ttu-id="ac502-106">**грешка**: низ на код на грешка, който може да се използва за класифицирането на типове грешки, които възникват, и трябва да се използва за реагиране на грешки.</span><span class="sxs-lookup"><span data-stu-id="ac502-106">**error**: An error code string that can be used to classify types of errors that occur, and should be used to react to errors.</span></span>
    - <span data-ttu-id="ac502-107">Полето за **грешка** има няколко възможни стойности – прегледайте връзките с документацията за протокола и OAuth 2,0 спецификациите за повече информация за конкретни грешки и как да ги реагирате.</span><span class="sxs-lookup"><span data-stu-id="ac502-107">The **error** field has several possible values - review the protocol documentation links and OAuth 2.0 specs for more information about specific errors and how to react to them.</span></span>

- <span data-ttu-id="ac502-108">Ето примерен отговор на грешка:</span><span class="sxs-lookup"><span data-stu-id="ac502-108">Here is a sample error response:</span></span>
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
2. <span data-ttu-id="ac502-109">**Справка за актуална информация за код на грешка**</span><span class="sxs-lookup"><span data-stu-id="ac502-109">**Lookup current error code information**</span></span>

- <span data-ttu-id="ac502-110">Кодовете на грешки и съобщенията подлежат на промяна.</span><span class="sxs-lookup"><span data-stu-id="ac502-110">Error codes and messages are subject to change.</span></span> <span data-ttu-id="ac502-111">За най-актуална информация вижте страницата, https://login.microsoftonline.com/error за да намерите описания на грешки, корекции на AADSTS и някои предложени заобиколни решения.</span><span class="sxs-lookup"><span data-stu-id="ac502-111">For the most current information, see the https://login.microsoftonline.com/error page to find AADSTS error descriptions, fixes, and some suggested workarounds.</span></span>
- <span data-ttu-id="ac502-112">Можете също да потърсите и отстраните [кодове за грешка на AADSTS](https://docs.microsoft.com/azure/active-directory/develop/reference-aadsts-error-codes#aadsts-error-codes) , описани в кодовете на грешки при удостоверяване на статия [Azure ad и упълномощаване](https://docs.microsoft.com/azure/active-directory/develop/reference-aadsts-error-codes#handling-error-codes-in-your-application).</span><span class="sxs-lookup"><span data-stu-id="ac502-112">You can also search for and troubleshoot [AADSTS error codes](https://docs.microsoft.com/azure/active-directory/develop/reference-aadsts-error-codes#aadsts-error-codes) listed in the article [Azure AD Authentication and authorization error codes](https://docs.microsoft.com/azure/active-directory/develop/reference-aadsts-error-codes#handling-error-codes-in-your-application).</span></span>

3. <span data-ttu-id="ac502-113">**Получаване на помощ**</span><span class="sxs-lookup"><span data-stu-id="ac502-113">**Get Help**</span></span>

- <span data-ttu-id="ac502-114">[Опции за поддръжка и помощ за разработчиците](https://docs.microsoft.com/azure/active-directory/develop/developer-support-help-options) – ако ви е нужен отговор на въпрос или помощ при решаването на проблем, който не е обхванат от нашата документация, може би е време да се свържете с експертите за помощ.</span><span class="sxs-lookup"><span data-stu-id="ac502-114">[Support and help options for developers](https://docs.microsoft.com/azure/active-directory/develop/developer-support-help-options) - If you need an answer to a question or help in solving a problem not covered in our documentation, it might be time to reach out to experts for help.</span></span> <span data-ttu-id="ac502-115">Тази статия предоставя няколко предложения за получаване на отговори на вашите въпроси при разработване на приложения, които се интегрират с платформата за самоличност на Microsoft.</span><span class="sxs-lookup"><span data-stu-id="ac502-115">This article provides several suggestions for getting answers to your questions as you develop apps that integrate with the Microsoft identity platform.</span></span>








