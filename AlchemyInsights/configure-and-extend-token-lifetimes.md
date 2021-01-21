---
title: Конфигуриране и удължаване на срока на валидност на знаците
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 01/20/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "7778"
- "9004351"
ms.openlocfilehash: 505e79ae9a163b89a6df2a7085480728bb0f1051
ms.sourcegitcommit: e378232f4c9ef4e962208100db752221e7bd2dd6
ms.translationtype: MT
ms.contentlocale: bg-BG
ms.lasthandoff: 01/20/2021
ms.locfileid: "49916688"
---
# <a name="configure-and-extend-token-lifetimes"></a><span data-ttu-id="49478-102">Конфигуриране и удължаване на срока на валидност на знаците</span><span class="sxs-lookup"><span data-stu-id="49478-102">Configure and extend token lifetimes</span></span>

<span data-ttu-id="49478-103">Можете да укажете живота на Access, SAML или ИД маркер, издаден от платформата за самоличност на Microsoft.</span><span class="sxs-lookup"><span data-stu-id="49478-103">You can specify the lifetime of an access, SAML, or ID token issued by Microsoft identity platform.</span></span> <span data-ttu-id="49478-104">Можете да зададете маркери за цял живот за всички приложения във вашата организация, за приложение за много клиенти (мултиорганизация) или за определен принципал на услуга във вашата организация.</span><span class="sxs-lookup"><span data-stu-id="49478-104">You can set token lifetimes for all apps in your organization, for a multi-tenant (multi-organization) application, or for a specific service principal in your organization.</span></span> <span data-ttu-id="49478-105">За повече информация прочетете [конфигурируеми животи за маркери](https://docs.microsoft.com/azure/active-directory/develop/active-directory-configurable-token-lifetimes).</span><span class="sxs-lookup"><span data-stu-id="49478-105">For more info, read [configurable token lifetimes](https://docs.microsoft.com/azure/active-directory/develop/active-directory-configurable-token-lifetimes).</span></span>

<span data-ttu-id="49478-106">За примери прочетете [примери за това как се конфигурират животи за маркери](https://docs.microsoft.com/azure/active-directory/develop/configure-token-lifetimes).</span><span class="sxs-lookup"><span data-stu-id="49478-106">For examples, read [examples of how to configure token lifetimes](https://docs.microsoft.com/azure/active-directory/develop/configure-token-lifetimes).</span></span>

<span data-ttu-id="49478-107">За да научите как да конфигурирате живота и съвместимостта на маркер в Azure Active Directory B2C (Azure AD B2C), вижте [Конфигуриране на маркери в Azure Active DIRECTORY B2C](https://docs.microsoft.com/azure/active-directory-b2c/configure-tokens?pivots=b2c-user-flow).</span><span class="sxs-lookup"><span data-stu-id="49478-107">To learn how to configure the lifetime and compatibility of a token in Azure Active Directory B2C (Azure AD B2C), see [Configure tokens in Azure Active Directory B2C](https://docs.microsoft.com/azure/active-directory-b2c/configure-tokens?pivots=b2c-user-flow).</span></span>

<span data-ttu-id="49478-108">Статията [Конфигурирай поведението на сесиите в Azure Active DIRECTORY B2C](https://docs.microsoft.com/azure/active-directory-b2c/session-behavior?pivots=b2c-user-flow) описва методите за еднократна идентификация (SSO), използвани в AZURE ad B2C, и ви помага да изберете най-подходящия метод за SSO при конфигуриране на правилата си.</span><span class="sxs-lookup"><span data-stu-id="49478-108">The article [Configure session behavior in Azure Active Directory B2C](https://docs.microsoft.com/azure/active-directory-b2c/session-behavior?pivots=b2c-user-flow) describes the single sign-on (SSO) methods used in Azure AD B2C and helps you choose the most appropriate SSO method when configuring your policy.</span></span>

<span data-ttu-id="49478-109">**Колко дълго ще трае маркерите? Колко време важат за тях?**</span><span class="sxs-lookup"><span data-stu-id="49478-109">**How long do tokens last? How long are they valid for?**</span></span>

<span data-ttu-id="49478-110">Продължителността на живота на знаците е 1 час, а продължителността на сесията е 24 часа.</span><span class="sxs-lookup"><span data-stu-id="49478-110">Token lifetimes are 1 hour and the session lifetime is 24 hours.</span></span> <span data-ttu-id="49478-111">Това означава, че ако не са правени искания за 24 часа, ще трябва да влезете отново, преди да поискате нов маркер.</span><span class="sxs-lookup"><span data-stu-id="49478-111">This means that if no requests have been made in 24 hours, you will need to log in again before requesting a new token.</span></span>

> [!NOTE]
> <span data-ttu-id="49478-112">След 30 май 2020, няма нов клиент, който да може да използва конфигурируеми правила за живот, за да конфигурира сесия и маркери за обновяване.</span><span class="sxs-lookup"><span data-stu-id="49478-112">After May 30, 2020, no new tenant will be able to use Configurable Token Lifetime policy to configure session and refresh tokens.</span></span> <span data-ttu-id="49478-113">Неодобрението ще се случи в рамките на няколко месеца след това, което означава, че ще спрем да почитаме съществуващи сеанси и обновете полицейски маркери.</span><span class="sxs-lookup"><span data-stu-id="49478-113">The deprecation will happen within several months after that, which means that we will stop honoring existing session and refresh tokens polices.</span></span> <span data-ttu-id="49478-114">Все още можете да конфигурирате маркер за достъп до животите след отказа.</span><span class="sxs-lookup"><span data-stu-id="49478-114">You can still configure access token lifetimes after the deprecation.</span></span>






