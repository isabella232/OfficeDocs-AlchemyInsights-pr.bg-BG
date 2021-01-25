---
title: Проблеми при разработване на приложения с API
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
- "7755"
ms.openlocfilehash: 26d732819b64efa4fb84da44cc2a279368aa28b0
ms.sourcegitcommit: 605a73b159d30634b064c1b63b0e734ceb3fdec8
ms.translationtype: MT
ms.contentlocale: bg-BG
ms.lasthandoff: 01/25/2021
ms.locfileid: "49974264"
---
# <a name="issues-developing-applications-with-apis"></a><span data-ttu-id="56ee9-102">Проблеми при разработване на приложения с API</span><span class="sxs-lookup"><span data-stu-id="56ee9-102">Issues developing applications with APIs</span></span>

<span data-ttu-id="56ee9-103">За да започнете да използвате API на Azure Active Directory, вижте [справочника за ръководство за бърз старт в AZURE ad Graph](https://docs.microsoft.com/azure/active-directory/develop/microsoft-graph-intro) или вижте [документацията за справочника за API за интерактивна Azure ad Graph](https://docs.microsoft.com/previous-versions/azure/ad/graph/api/api-catalog).</span><span class="sxs-lookup"><span data-stu-id="56ee9-103">To begin using the Azure Active Directory Graph API, see the [Azure AD Graph API quickstart guide](https://docs.microsoft.com/azure/active-directory/develop/microsoft-graph-intro) , or view the [interactive Azure AD Graph API reference documentation](https://docs.microsoft.com/previous-versions/azure/ad/graph/api/api-catalog).</span></span>

<span data-ttu-id="56ee9-104">**Край на поддръжката за библиотеката за удостоверяване на Azure Active Directory (ADAL) и API за Azure AD Graph (пад Graph)**</span><span class="sxs-lookup"><span data-stu-id="56ee9-104">**End of support for Azure Active Directory Authentication Library (ADAL) and Azure AD Graph API (AAD Graph)**</span></span>

<span data-ttu-id="56ee9-105">**Започвайки от 30 юни 2020**, повече няма да добавяме нови функции към ADAL и Azure ad Graph.</span><span class="sxs-lookup"><span data-stu-id="56ee9-105">**Starting June 30th, 2020**, we will no longer add any new features to ADAL and Azure AD Graph.</span></span> <span data-ttu-id="56ee9-106">Ще продължим да предоставяме техническа поддръжка и актуализации на защитата, но повече няма да предоставяме актуализации на функции.</span><span class="sxs-lookup"><span data-stu-id="56ee9-106">We will continue to provide technical support and security updates but will no longer provide feature updates.</span></span>

<span data-ttu-id="56ee9-107">**Започвайки от 30 юни 2022**, ние ще прекратим ПОДДРЪЖКАТА за ADAL и Azure ad Graph и повече няма да предоставяме техническа поддръжка и актуализации на защитата.</span><span class="sxs-lookup"><span data-stu-id="56ee9-107">**Starting June 30th, 2022**, we will end support for ADAL and Azure AD Graph and will no longer provide technical support or security updates.</span></span>

<span data-ttu-id="56ee9-108">Приложенията, използващи ADAL за съществуващите версии на операционната система, ще продължат да работят след този час, но няма да получат техническа поддръжка или актуализация на защитата.</span><span class="sxs-lookup"><span data-stu-id="56ee9-108">Apps using ADAL on existing OS versions will continue to work after this time but will not get any technical support or security updates.</span></span>

<span data-ttu-id="56ee9-109">Приложенията, използващи Azure AD Graph след този час, вече не могат да получават отговори от крайна точка на Azure AD Graph.</span><span class="sxs-lookup"><span data-stu-id="56ee9-109">Apps using Azure AD Graph after this time may no longer receive responses from the Azure AD Graph endpoint.</span></span>

<span data-ttu-id="56ee9-110">**ADALна миграция**</span><span class="sxs-lookup"><span data-stu-id="56ee9-110">**ADAL Migration**</span></span>

<span data-ttu-id="56ee9-111">Препоръчваме ви да актуализирате до [библиотеката за удостоверяване на Microsoft (MSAL)](https://docs.microsoft.com/azure/active-directory/develop/v2-overview), която има най-новите функции и актуализации на защитата.</span><span class="sxs-lookup"><span data-stu-id="56ee9-111">We recommend updating to the [Microsoft Authentication Library (MSAL)](https://docs.microsoft.com/azure/active-directory/develop/v2-overview), which has the latest features and security updates.</span></span>

<span data-ttu-id="56ee9-112">Ако използвате Microsoft Apps, Знайте, че Microsoft е в процес на мигриране на приложенията си към MSAL до крайния срок за поддръжка, за да се гарантира, че ще извлече полза от текущите подобрения в защитата и функциите на MSAL.</span><span class="sxs-lookup"><span data-stu-id="56ee9-112">If you're using Microsoft apps, know that Microsoft is in the process of migrating its applications to MSAL by the end-of-support deadline, ensuring they'll benefit from MSAL's ongoing security and feature improvements.</span></span>

1. <span data-ttu-id="56ee9-113">[Прочетете ЧЗВ за ADAL](https://docs.microsoft.com/azure/active-directory/develop/msal-migration#frequently-asked-questions-faq).</span><span class="sxs-lookup"><span data-stu-id="56ee9-113">[Read the ADAL FAQ](https://docs.microsoft.com/azure/active-directory/develop/msal-migration#frequently-asked-questions-faq).</span></span>
1. <span data-ttu-id="56ee9-114">[Научете как да мигрирате приложения на база платформа](https://docs.microsoft.com/azure/active-directory/develop/msal-migration#frequently-asked-questions-faq).</span><span class="sxs-lookup"><span data-stu-id="56ee9-114">[Learn about how to migrate apps on a per-platform basis](https://docs.microsoft.com/azure/active-directory/develop/msal-migration#frequently-asked-questions-faq).</span></span>
1. <span data-ttu-id="56ee9-115">Ако имате нужда от помощ, за да разберете кой от вашите приложения използва ADAL, ви препоръчваме да прегледате всички изходния код на вашите приложения и ако е приложимо, да достигнете до всякакви доставчици на ISV или приложения.</span><span class="sxs-lookup"><span data-stu-id="56ee9-115">If you need help understanding which of your apps use ADAL, we recommend you review all of your apps' source code, and if applicable, reach out to any ISVs or app providers.</span></span> <span data-ttu-id="56ee9-116">Поддръжката на Microsoft може да ви предостави и списък с всички приложения, които не са на Microsoft ADAL, във вашия клиент.</span><span class="sxs-lookup"><span data-stu-id="56ee9-116">Microsoft support can also provide you with a list of all non-Microsoft ADAL apps in your tenant.</span></span>

<span data-ttu-id="56ee9-117">**Преминаване към графиката в пад**</span><span class="sxs-lookup"><span data-stu-id="56ee9-117">**AAD Graph Migration**</span></span>

<span data-ttu-id="56ee9-118">За приложенията, които използват Azure AD Graph, следвайте нашите указания за мигриране на [приложенията на AZURE ad Graph към Microsoft Graph](https://docs.microsoft.com/graph/migrate-azure-ad-graph-overview?view=graph-rest-1.0&preserve-view=true).</span><span class="sxs-lookup"><span data-stu-id="56ee9-118">For applications that are using Azure AD Graph, follow our guidance to migrate [Azure AD Graph apps to Microsoft Graph](https://docs.microsoft.com/graph/migrate-azure-ad-graph-overview?view=graph-rest-1.0&preserve-view=true).</span></span>

1. <span data-ttu-id="56ee9-119">[Нашият контролен списък за мигриране предоставя първи стъпки](https://docs.microsoft.com/graph/migrate-azure-ad-graph-planning-checklist).</span><span class="sxs-lookup"><span data-stu-id="56ee9-119">[Our migration checklist provides a getting started point](https://docs.microsoft.com/graph/migrate-azure-ad-graph-planning-checklist).</span></span> 
1. <span data-ttu-id="56ee9-120">Вашият портал за регистрация на Azure App показва кои приложения използват пад Graph.</span><span class="sxs-lookup"><span data-stu-id="56ee9-120">Your Azure app registration portal shows which applications are using AAD Graph.</span></span> <span data-ttu-id="56ee9-121">Препоръчваме ви да прегледате всички изходни кодове на вашите приложения и ако е приложимо, да се свържете с всички доставчици на ISV или приложения.</span><span class="sxs-lookup"><span data-stu-id="56ee9-121">We recommend you review all of your apps' source code, and if applicable, reach out to any ISVs or app providers.</span></span> <span data-ttu-id="56ee9-122">Поддръжката на Microsoft може да ви предостави и списък на всички употреби на използването на пад във вашия клиент.</span><span class="sxs-lookup"><span data-stu-id="56ee9-122">Microsoft support can also provide you with a list of all AAD Graph usage in your tenant.</span></span>
1. <span data-ttu-id="56ee9-123">За да получите достъп до данните в Microsoft Graph, потребителят или администраторът трябва да му предостави правилните разрешения чрез процеса на одобрение.</span><span class="sxs-lookup"><span data-stu-id="56ee9-123">For your app to access data in Microsoft Graph, the user or administrator must grant it the correct permissions via a consent process.</span></span> <span data-ttu-id="56ee9-124">[Справочникът за разрешения на Microsoft Graph](https://docs.microsoft.com/graph/permissions-reference?context=graph%2Fapi%2Fbeta&view=graph-rest-beta&preserve-view=true) изброява разрешенията, свързани с всеки основен набор от API на Microsoft Graph.</span><span class="sxs-lookup"><span data-stu-id="56ee9-124">The [Microsoft Graph permissions reference](https://docs.microsoft.com/graph/permissions-reference?context=graph%2Fapi%2Fbeta&view=graph-rest-beta&preserve-view=true) lists the permissions associated with each major set of Microsoft Graph APIs.</span></span> <span data-ttu-id="56ee9-125">Освен това се предоставят насоки как да използвате разрешенията.</span><span class="sxs-lookup"><span data-stu-id="56ee9-125">It also provides guidance about how to use the permissions.</span></span>
