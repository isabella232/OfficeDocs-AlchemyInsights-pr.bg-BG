---
title: Проблеми с библиотеките за удостоверяване
ms.author: v-jmathew
author: v-jmathew
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004333"
- "7731"
ms.openlocfilehash: ab4ffbc78a7cadd8acee3c98eaa5f3323da9c7e3
ms.sourcegitcommit: 7e6d89f47eca1babf5aeba4995bceccd990c3963
ms.translationtype: MT
ms.contentlocale: bg-BG
ms.lasthandoff: 01/28/2021
ms.locfileid: "50063580"
---
# <a name="issues-with-authentication-libraries"></a><span data-ttu-id="7e85d-102">Проблеми с библиотеките за удостоверяване</span><span class="sxs-lookup"><span data-stu-id="7e85d-102">Issues with Authentication Libraries</span></span>

1. <span data-ttu-id="7e85d-103">[Библиотеките за удостоверяване на Microsoft Identity platforms](https://docs.microsoft.com/azure/active-directory/develop/reference-v2-libraries) изброява поддържани и съвместими с Microsoft библиотеки клиент и междинен източник.</span><span class="sxs-lookup"><span data-stu-id="7e85d-103">[Microsoft identity platform authentication libraries](https://docs.microsoft.com/azure/active-directory/develop/reference-v2-libraries) lists Microsoft-supported and compatible client and middleware libraries.</span></span>
2. <span data-ttu-id="7e85d-104">Библиотеката за удостоверяване на Microsoft (MSAL) поддържа няколко [потока на удостоверяване](https://docs.microsoft.com/azure/active-directory/develop/msal-authentication-flows) за използване в различни сценарии за приложения.</span><span class="sxs-lookup"><span data-stu-id="7e85d-104">The Microsoft Authentication Library (MSAL) supports several [authentication flows](https://docs.microsoft.com/azure/active-directory/develop/msal-authentication-flows) for use in different application scenarios.</span></span>
3. <span data-ttu-id="7e85d-105">За удостоверяване и получаване на маркери можете да инициализирате ново публично или поверително клиентско приложение в своя код.</span><span class="sxs-lookup"><span data-stu-id="7e85d-105">To authenticate and acquire tokens, you initialize a new public or confidential client application in your code.</span></span> <span data-ttu-id="7e85d-106">Можете да зададете няколко опции за конфигуриране, когато инициализирате приложението клиент в библиотеката за удостоверяване на Microsoft (MSAL).</span><span class="sxs-lookup"><span data-stu-id="7e85d-106">You can set several configuration options when you initialize the client app in the Microsoft Authentication Library (MSAL).</span></span> <span data-ttu-id="7e85d-107">За да научите повече, вижте [Опции за конфигуриране на приложения](https://docs.microsoft.com/azure/active-directory/develop/msal-client-application-configuration).</span><span class="sxs-lookup"><span data-stu-id="7e85d-107">To learn more, see [Application configuration options](https://docs.microsoft.com/azure/active-directory/develop/msal-client-application-configuration).</span></span>

<span data-ttu-id="7e85d-108">**Край на поддръжката за библиотеката за удостоверяване на Azure Active Directory (ADAL) и API за Azure AD Graph (пад Graph)**</span><span class="sxs-lookup"><span data-stu-id="7e85d-108">**End of support for Azure Active Directory Authentication Library (ADAL) and Azure AD Graph API (AAD Graph)**</span></span>

<span data-ttu-id="7e85d-109">**Започвайки от 30 юни 2020**, повече няма да добавяме нови функции към ADAL и Azure ad Graph.</span><span class="sxs-lookup"><span data-stu-id="7e85d-109">**Starting June 30th, 2020**, we will no longer add any new features to ADAL and Azure AD Graph.</span></span> <span data-ttu-id="7e85d-110">Ще продължим да предоставяме актуализации на техническата поддръжка и защитата, но повече няма да предоставяме актуализации на функции.</span><span class="sxs-lookup"><span data-stu-id="7e85d-110">We will continue to provide technical support and security updates but will no longer provide feature updates.</span></span>

<span data-ttu-id="7e85d-111">**Започвайки от 30 юни 2022**, ние ще прекратим ПОДДРЪЖКАТА за ADAL и Azure ad Graph и повече няма да предоставяме техническа поддръжка и актуализации на защитата.</span><span class="sxs-lookup"><span data-stu-id="7e85d-111">**Starting June 30th, 2022**, we will end support for ADAL and Azure AD Graph and will no longer provide technical support or security updates.</span></span>

<span data-ttu-id="7e85d-112">Приложенията, използващи ADAL за съществуващите версии на операционната система, ще продължат да работят след този час, но няма *да получат техническа поддръжка или актуализация на защитата*.</span><span class="sxs-lookup"><span data-stu-id="7e85d-112">Apps using ADAL on existing OS versions will continue to work after this time but will not *get any technical support or security updates*.</span></span>

<span data-ttu-id="7e85d-113">Приложенията, използващи Azure AD Graph след този час, вече не могат да получават отговори от крайна точка на Azure AD Graph.</span><span class="sxs-lookup"><span data-stu-id="7e85d-113">Apps using Azure AD Graph after this time may no longer receive responses from the Azure AD Graph endpoint.</span></span>

<span data-ttu-id="7e85d-114">**ADALна миграция**</span><span class="sxs-lookup"><span data-stu-id="7e85d-114">**ADAL Migration**</span></span>

<span data-ttu-id="7e85d-115">Препоръчваме да актуализирате до [Библиотеката за удостоверяване на Microsoft (MSAL)](https://docs.microsoft.com/azure/active-directory/develop/v2-overview), в която има най-новите функции и актуализации на защитата.</span><span class="sxs-lookup"><span data-stu-id="7e85d-115">We recommend updating to the [Microsoft Authentication Library (MSAL)](https://docs.microsoft.com/azure/active-directory/develop/v2-overview), which has the latest features and security updates.</span></span>

<span data-ttu-id="7e85d-116">Ако използвате Microsoft Apps, Знайте, че Microsoft е в процес на мигриране на приложенията си към MSAL до крайния срок за поддръжка, за да се гарантира, че ще извлече полза от текущите подобрения в защитата и функциите на MSAL.</span><span class="sxs-lookup"><span data-stu-id="7e85d-116">If you are using Microsoft apps, know that Microsoft is in the process of migrating its applications to MSAL by the end-of-support deadline, ensuring they will benefit from MSAL's ongoing security and feature improvements.</span></span>

<span data-ttu-id="7e85d-117">За повече информация вижте:</span><span class="sxs-lookup"><span data-stu-id="7e85d-117">For more information, see:</span></span>

1. [<span data-ttu-id="7e85d-118">Прочетете ЧЗВ за ADAL</span><span class="sxs-lookup"><span data-stu-id="7e85d-118">Read the ADAL FAQ</span></span>](https://docs.microsoft.com/azure/active-directory/develop/msal-migration#frequently-asked-questions-faq)
2. [<span data-ttu-id="7e85d-119">Научете как да мигрирате приложения на базата на платформа</span><span class="sxs-lookup"><span data-stu-id="7e85d-119">Learn about how to migrate apps on a per-platform basis</span></span>](https://docs.microsoft.com/azure/active-directory/develop/msal-migration#frequently-asked-questions-faq)
3. <span data-ttu-id="7e85d-120">Ако имате нужда от помощ, за да разберете кой от вашите приложения използва ADAL, ви препоръчваме да прегледате всички изходния код на вашите приложения и ако е приложимо, да достигнете до всякакви доставчици на ISV или приложения.</span><span class="sxs-lookup"><span data-stu-id="7e85d-120">If you need help understanding which of your apps use ADAL, we recommend you review all of your apps' source code, and if applicable, reach out to any ISVs or app providers.</span></span> <span data-ttu-id="7e85d-121">Поддръжката на Microsoft също може да ви предостави списък с всички приложения на ADAL, които не са на Microsoft, във вашия клиент.</span><span class="sxs-lookup"><span data-stu-id="7e85d-121">Microsoft support can also provide you with a list of all non-Microsoft ADAL apps in your tenant.</span></span>

<span data-ttu-id="7e85d-122">**Мигриране на AAD Graph**</span><span class="sxs-lookup"><span data-stu-id="7e85d-122">**AAD Graph Migration**</span></span>

<span data-ttu-id="7e85d-123">За приложенията, които използват Azure AD Graph, следвайте нашите указания за [мигриране на приложенията на AZURE ad Graph към Microsoft Graph](https://docs.microsoft.com/graph/migrate-azure-ad-graph-overview).</span><span class="sxs-lookup"><span data-stu-id="7e85d-123">For applications that are using Azure AD Graph, follow our guidance to [migrate Azure AD Graph apps to Microsoft Graph](https://docs.microsoft.com/graph/migrate-azure-ad-graph-overview).</span></span>

1. [<span data-ttu-id="7e85d-124">Нашият контролен списък за мигриране предоставя първи стъпки.</span><span class="sxs-lookup"><span data-stu-id="7e85d-124">Our migration checklist provides a getting started point.</span></span>](https://docs.microsoft.com/graph/migrate-azure-ad-graph-planning-checklist)
2. <span data-ttu-id="7e85d-125">Вашият портал за регистрация на приложения на Azure показва кои приложения използват AAD Graph.</span><span class="sxs-lookup"><span data-stu-id="7e85d-125">Your Azure app registration portal shows which applications are using AAD Graph.</span></span> <span data-ttu-id="7e85d-126">Препоръчваме ви да прегледате изходния код на всички приложения и ако е приложимо, да се свържете с доставчици на интернет или приложения.</span><span class="sxs-lookup"><span data-stu-id="7e85d-126">We recommend you review all of your apps' source code, and if applicable, reach out to any ISVs or app providers.</span></span> <span data-ttu-id="7e85d-127">Поддръжката на Microsoft може да ви предостави и списък на всички употреби на използването на пад във вашия клиент.</span><span class="sxs-lookup"><span data-stu-id="7e85d-127">Microsoft support can also provide you with a list of all AAD Graph usage in your tenant.</span></span>
3. <span data-ttu-id="7e85d-128">За да получите достъп до данните в Microsoft Graph, потребителят или администраторът трябва да му предостави правилните разрешения чрез процеса на одобрение.</span><span class="sxs-lookup"><span data-stu-id="7e85d-128">For your app to access data in Microsoft Graph, the user or administrator must grant it the correct permissions via a consent process.</span></span> <span data-ttu-id="7e85d-129">[Справочникът за разрешения на Microsoft Graph](https://docs.microsoft.com/graph/permissions-reference) изброява разрешенията, свързани с всеки основен набор от API на Microsoft Graph.</span><span class="sxs-lookup"><span data-stu-id="7e85d-129">The [Microsoft Graph permissions reference](https://docs.microsoft.com/graph/permissions-reference) lists the permissions associated with each major set of Microsoft Graph APIs.</span></span> <span data-ttu-id="7e85d-130">Освен това се предоставят насоки как да използвате разрешенията.</span><span class="sxs-lookup"><span data-stu-id="7e85d-130">It also provides guidance about how to use the permissions.</span></span>
