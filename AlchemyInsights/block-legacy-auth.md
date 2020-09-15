---
title: BlockLegacyAuth
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3154"
- "9001194"
ms.openlocfilehash: baf3ee808cce1e4da362dd0841c0138d7d9268d1
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: bg-BG
ms.lasthandoff: 09/14/2020
ms.locfileid: "47685587"
---
# <a name="blocking-legacy-authentication"></a><span data-ttu-id="ed00c-102">Блокиране на наследено удостоверяване</span><span class="sxs-lookup"><span data-stu-id="ed00c-102">Blocking legacy authentication</span></span>

<span data-ttu-id="ed00c-103">Наследеното удостоверяване е израз, който препраща към искане за удостоверяване, направено от:</span><span class="sxs-lookup"><span data-stu-id="ed00c-103">Legacy authentication is a term that refers to an authentication request made by:</span></span>

- <span data-ttu-id="ed00c-104">По-стари клиенти на Office, които не използват модерно удостоверяване (например клиент на Office 2010).</span><span class="sxs-lookup"><span data-stu-id="ed00c-104">Older Office clients that do not use modern authentication (for example, Office 2010 client).</span></span>

- <span data-ttu-id="ed00c-105">Всеки клиент, който използва стари протоколи за поща, като IMAP/SMTP/POP3.</span><span class="sxs-lookup"><span data-stu-id="ed00c-105">Any client that uses legacy mail protocols such as IMAP/SMTP/POP3.</span></span>

<span data-ttu-id="ed00c-106">За повече информация относно блокирането на Legacy удостоверяване и разрешаването на модерното удостоверяване, вижте [блокиране на наследени удостоверяване](https://docs.microsoft.com/azure/active-directory/conditional-access/concept-conditional-access-block-legacy-authentication).</span><span class="sxs-lookup"><span data-stu-id="ed00c-106">For more information on blocking legacy authentication and enabling modern authentication, refer to [Blocking legacy authentication](https://docs.microsoft.com/azure/active-directory/conditional-access/concept-conditional-access-block-legacy-authentication).</span></span>

<span data-ttu-id="ed00c-107">Настройките по подразбиране за защита в Azure Active Directory (Azure AD) улесняват защитата и защитават вашата организация.</span><span class="sxs-lookup"><span data-stu-id="ed00c-107">Security defaults in Azure Active Directory (Azure AD) make it easier to be secure and help protect your organization.</span></span> <span data-ttu-id="ed00c-108">Настройките по подразбиране за защита съдържат предварително конфигурирани настройки за защита за често срещани атаки.</span><span class="sxs-lookup"><span data-stu-id="ed00c-108">Security defaults contain preconfigured security settings for common attacks.</span></span>
<span data-ttu-id="ed00c-109">За повече информация относно настройките по подразбиране за защита вижте [какви са настройките по подразбиране за защита?](https://docs.microsoft.com/azure/active-directory/fundamentals/concept-fundamentals-security-defaults).</span><span class="sxs-lookup"><span data-stu-id="ed00c-109">For more information about security defaults, refer to [What are security defaults?](https://docs.microsoft.com/azure/active-directory/fundamentals/concept-fundamentals-security-defaults).</span></span> 

<span data-ttu-id="ed00c-110">**Забележка**: Ако клиентът ви е създаден на или след 22 октомври 2019, е възможно да имате новото поведение по подразбиране, което вече е разрешено по подразбиране на защитата във вашия клиент.</span><span class="sxs-lookup"><span data-stu-id="ed00c-110">**Note**:  If your tenant was created on or after October 22nd, 2019, it's possible you are experiencing the new secure-by-default behavior and already have security defaults enabled in your tenant.</span></span>  <span data-ttu-id="ed00c-111">В усилията си за защита на всички наши потребители е създадена настройката за защита по подразбиране за всички създадени нови наематели.</span><span class="sxs-lookup"><span data-stu-id="ed00c-111">In an effort to protect all of our users, security defaults is being rolled out to all new tenants created.</span></span>
