---
title: BlockLegacyAuth
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3154"
- "9001194"
ms.openlocfilehash: 06ded694893c020f862864215700853b19d35f08
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: bg-BG
ms.lasthandoff: 04/15/2021
ms.locfileid: "51820167"
---
# <a name="blocking-legacy-authentication"></a><span data-ttu-id="567b9-102">Блокиране на наследено удостоверяване</span><span class="sxs-lookup"><span data-stu-id="567b9-102">Blocking legacy authentication</span></span>

<span data-ttu-id="567b9-103">Наследеното удостоверяване е израз, който препраща към искане за удостоверяване, направено от:</span><span class="sxs-lookup"><span data-stu-id="567b9-103">Legacy authentication is a term that refers to an authentication request made by:</span></span>

- <span data-ttu-id="567b9-104">По-стари клиенти на Office, които не използват модерно удостоверяване (например клиент на Office 2010).</span><span class="sxs-lookup"><span data-stu-id="567b9-104">Older Office clients that do not use modern authentication (for example, Office 2010 client).</span></span>

- <span data-ttu-id="567b9-105">Всеки клиент, който използва стари пощенски протоколи, като например IMAP/SMTP/POP3.</span><span class="sxs-lookup"><span data-stu-id="567b9-105">Any client that uses legacy mail protocols such as IMAP/SMTP/POP3.</span></span>

<span data-ttu-id="567b9-106">За повече информация относно блокирането на наследено удостоверяване и разрешаването на модерно удостоверяване вижте [Блокиране на наследено удостоверяване](https://docs.microsoft.com/azure/active-directory/conditional-access/concept-conditional-access-block-legacy-authentication).</span><span class="sxs-lookup"><span data-stu-id="567b9-106">For more information on blocking legacy authentication and enabling modern authentication, refer to [Blocking legacy authentication](https://docs.microsoft.com/azure/active-directory/conditional-access/concept-conditional-access-block-legacy-authentication).</span></span>

<span data-ttu-id="567b9-107">Настройките по подразбиране за защита в Azure Active Directory (Azure AD) улесняват защитата и защитават вашата организация.</span><span class="sxs-lookup"><span data-stu-id="567b9-107">Security defaults in Azure Active Directory (Azure AD) make it easier to be secure and help protect your organization.</span></span> <span data-ttu-id="567b9-108">Настройките за защита по подразбиране съдържат предварително конфигурирани настройки за защита за често срещани атаки.</span><span class="sxs-lookup"><span data-stu-id="567b9-108">Security defaults contain preconfigured security settings for common attacks.</span></span>
<span data-ttu-id="567b9-109">За повече информация относно настройките за защита по подразбиране вижте [Какво са настройките по подразбиране за защита?](https://docs.microsoft.com/azure/active-directory/fundamentals/concept-fundamentals-security-defaults).</span><span class="sxs-lookup"><span data-stu-id="567b9-109">For more information about security defaults, refer to [What are security defaults?](https://docs.microsoft.com/azure/active-directory/fundamentals/concept-fundamentals-security-defaults).</span></span> 

<span data-ttu-id="567b9-110">**Забележка:** Ако вашият клиент е създаден на или след 22 октомври 2019 г., е възможно да се сблъскате с новото поведение "защитен по подразбиране" и вече имате активирани настройки по подразбиране на защитата във вашия клиент.</span><span class="sxs-lookup"><span data-stu-id="567b9-110">**Note**:  If your tenant was created on or after October 22nd, 2019, it's possible you are experiencing the new secure-by-default behavior and already have security defaults enabled in your tenant.</span></span>  <span data-ttu-id="567b9-111">В опит да защитим всички наши потребители, по подразбиране защитата се създава за всички нови клиенти, създадени.</span><span class="sxs-lookup"><span data-stu-id="567b9-111">In an effort to protect all of our users, security defaults is being rolled out to all new tenants created.</span></span>
