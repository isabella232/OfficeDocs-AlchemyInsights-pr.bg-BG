---
title: Блок наследство
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3154"
- "9001194"
ms.openlocfilehash: e7bff5f9fcf6f2f2c77e93c2f27f585f2cc18bea
ms.sourcegitcommit: 98231a228ecb2bf14ec3b96d4dd4ccf2507617a3
ms.translationtype: MT
ms.contentlocale: bg-BG
ms.lasthandoff: 04/01/2020
ms.locfileid: "43079249"
---
# <a name="blocking-legacy-authentication"></a><span data-ttu-id="6d6f7-102">Блокиране на удостоверяване</span><span class="sxs-lookup"><span data-stu-id="6d6f7-102">Blocking legacy authentication</span></span>

<span data-ttu-id="6d6f7-103">Legacy удостоверяване е термин, който се отнася до заявка за удостоверяване, направена от:</span><span class="sxs-lookup"><span data-stu-id="6d6f7-103">Legacy authentication is a term that refers to an authentication request made by:</span></span>

- <span data-ttu-id="6d6f7-104">По-стари Office клиенти, които не използват съвременни удостоверяване (например клиент на Office 2010).</span><span class="sxs-lookup"><span data-stu-id="6d6f7-104">Older Office clients that do not use modern authentication (for example, Office 2010 client).</span></span>

- <span data-ttu-id="6d6f7-105">Всеки клиент, който използва стари поща протоколи като IMAP/SMTP/POP3.</span><span class="sxs-lookup"><span data-stu-id="6d6f7-105">Any client that uses legacy mail protocols such as IMAP/SMTP/POP3.</span></span>

<span data-ttu-id="6d6f7-106">За повече информация за блокиране на стари удостоверяване и разрешаване на съвременни удостоверяване вижте [Блокиране legacy удостоверяване](https://docs.microsoft.com/azure/active-directory/conditional-access/concept-conditional-access-block-legacy-authentication).</span><span class="sxs-lookup"><span data-stu-id="6d6f7-106">For more information on blocking legacy authentication and enabling modern authentication, refer to [Blocking legacy authentication](https://docs.microsoft.com/azure/active-directory/conditional-access/concept-conditional-access-block-legacy-authentication).</span></span>

<span data-ttu-id="6d6f7-107">Настройките по подразбиране за защита в Azure Active Directory (Azure AD) улесняват защитата и защитата на вашата организация.</span><span class="sxs-lookup"><span data-stu-id="6d6f7-107">Security defaults in Azure Active Directory (Azure AD) make it easier to be secure and help protect your organization.</span></span> <span data-ttu-id="6d6f7-108">Настройките по подразбиране за защитата съдържат предварително конфигурирани настройки за защита за често срещани атаки.</span><span class="sxs-lookup"><span data-stu-id="6d6f7-108">Security defaults contain preconfigured security settings for common attacks.</span></span>
<span data-ttu-id="6d6f7-109">За повече информация относно настройките по подразбиране за защитата вижте [Какво са настройките по подразбиране за защита?](https://docs.microsoft.com/azure/active-directory/fundamentals/concept-fundamentals-security-defaults).</span><span class="sxs-lookup"><span data-stu-id="6d6f7-109">For more information about security defaults, refer to [What are security defaults?](https://docs.microsoft.com/azure/active-directory/fundamentals/concept-fundamentals-security-defaults).</span></span> 

<span data-ttu-id="6d6f7-110">**Забележка:** Ако клиентът ви е създаден на или след 22 октомври 2019, е възможно да имате нов защитен по подразбиране поведение и вече има сигурност по подразбиране поддръжка в клиента.</span><span class="sxs-lookup"><span data-stu-id="6d6f7-110">**Note**:  If your tenant was created on or after October 22nd, 2019, it's possible you are experiencing the new secure-by-default behavior and already have security defaults enabled in your tenant.</span></span>  <span data-ttu-id="6d6f7-111">В стремежа си да защитим всички наши потребители, настройките за сигурност се реализират на всички нови наематели, създадени.</span><span class="sxs-lookup"><span data-stu-id="6d6f7-111">In an effort to protect all of our users, security defaults is being rolled out to all new tenants created.</span></span>
