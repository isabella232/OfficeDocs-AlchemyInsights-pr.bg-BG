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
# <a name="api-permissions-and-consent"></a><span data-ttu-id="3547c-102">Разрешения и съгласие с API</span><span class="sxs-lookup"><span data-stu-id="3547c-102">API permissions and consent</span></span>

<span data-ttu-id="3547c-103">Приложенията, които се интегрират с платформата за самоличност на Microsoft, следват модел на удостоверяване, който дава на потребителите и администраторите контрол върху това как могат да бъдат отваряни данни.</span><span class="sxs-lookup"><span data-stu-id="3547c-103">Applications that integrate with Microsoft identity platform follow an authorization model that gives users and administrators control over how data can be accessed.</span></span> <span data-ttu-id="3547c-104">Прилагането на модела на удостоверяване е актуализирано на крайната точка на платформата за самоличност на Microsoft.</span><span class="sxs-lookup"><span data-stu-id="3547c-104">The implementation of the authorization model has been updated on the Microsoft identity platform endpoint.</span></span> <span data-ttu-id="3547c-105">Той променя начина, по който приложението трябва да взаимодейства с платформата за самоличност на Microsoft.</span><span class="sxs-lookup"><span data-stu-id="3547c-105">It changes how an app must interact with the Microsoft identity platform.</span></span> <span data-ttu-id="3547c-106">[Разрешенията и съгласието в крайна точка на платформата за самоличност на Microsoft](https://docs.microsoft.com/azure/active-directory/develop/v2-permissions-and-consent) обхващат основните понятия на този модел на удостоверяване, включително обхвати, разрешения и съгласие.</span><span class="sxs-lookup"><span data-stu-id="3547c-106">[Permissions and consent in the Microsoft identity platform endpoint](https://docs.microsoft.com/azure/active-directory/develop/v2-permissions-and-consent) covers the basic concepts of this authorization model, including scopes, permissions, and consent.</span></span>

<span data-ttu-id="3547c-107">[Рамката за съгласие на Azure Active Directory (AZURE ad)](https://docs.microsoft.com/azure/active-directory/develop/consent-framework) улеснява създаването на уеб приложения и приложенията на родния клиент на множество клиенти.</span><span class="sxs-lookup"><span data-stu-id="3547c-107">The [Azure Active Directory (Azure AD) consent framework](https://docs.microsoft.com/azure/active-directory/develop/consent-framework) makes it easy to develop multi-tenant web and native client applications.</span></span> <span data-ttu-id="3547c-108">Тези приложения разрешават влизане чрез потребителски акаунти от клиент на Azure AD, който е различен от този, в който е регистрирано приложението.</span><span class="sxs-lookup"><span data-stu-id="3547c-108">These applications allow sign-in by user accounts from an Azure AD tenant that's different from the one where the application is registered.</span></span> <span data-ttu-id="3547c-109">Можете също да се наложи да получите достъп до уеб API, като например API за Microsoft Graph (за достъп до Azure AD, настройки и услуги в Microsoft 365) и други API за Microsoft Services, в допълнение към собствените си уеб API.</span><span class="sxs-lookup"><span data-stu-id="3547c-109">They may also need to access web APIs such as the Microsoft Graph API (to access Azure AD, Intune, and services in Microsoft 365) and other Microsoft services' APIs, in addition to your own web APIs.</span></span>

