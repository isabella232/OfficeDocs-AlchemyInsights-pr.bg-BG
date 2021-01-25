---
title: Проблеми при разработване на приложения
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 01/25/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "7754"
- "9004342"
ms.openlocfilehash: 652fd6431201380e8e96619f63ecac15a6704d4f
ms.sourcegitcommit: 029c4697b77ce996d41ca74c4fa86de1bb84bd99
ms.translationtype: MT
ms.contentlocale: bg-BG
ms.lasthandoff: 01/25/2021
ms.locfileid: "49974188"
---
# <a name="issues-developing-applications"></a><span data-ttu-id="6da87-102">Проблеми при разработване на приложения</span><span class="sxs-lookup"><span data-stu-id="6da87-102">Issues developing applications</span></span>

<span data-ttu-id="6da87-103">За да отстраните най-често срещаните проблеми при създаването на приложения на Azure Active Directory (AD), вижте следните статии:</span><span class="sxs-lookup"><span data-stu-id="6da87-103">To troubleshoot the most common problems when building Azure Active Directory (AD) apps, see the following articles:</span></span>

- [<span data-ttu-id="6da87-104">Виждам неприятности при влизане в приложения, които използват само браузъра Chrome</span><span class="sxs-lookup"><span data-stu-id="6da87-104">I am seeing trouble signing in to application(s) using Chrome browser only</span></span>](https://docs.microsoft.com/office365/troubleshoot/miscellaneous/chrome-behavior-affects-applications) 
- [<span data-ttu-id="6da87-105">Не знам как да променя настройките по подразбиране на токена за моето приложение</span><span class="sxs-lookup"><span data-stu-id="6da87-105">I don't know how to change the token lifetime defaults for my application</span></span>](https://docs.microsoft.com/azure/active-directory/develop/registration-config-change-token-lifetime-how-to) 
- [<span data-ttu-id="6da87-106">Притеснен съм относно това как работи дадено съгласие за приложение</span><span class="sxs-lookup"><span data-stu-id="6da87-106">I am confused about how application consent works</span></span>](https://docs.microsoft.com/azure/active-directory/application-dev-consent-framework) 
- [<span data-ttu-id="6da87-107">Не знам как да давам разрешения за моето приложение</span><span class="sxs-lookup"><span data-stu-id="6da87-107">I don't know how to grant permissions to my application</span></span>](https://docs.microsoft.com/azure/active-directory/manage-apps/configure-user-consent) 
- [<span data-ttu-id="6da87-108">Не разбирам разликата между разрешения за делегиран и приложение</span><span class="sxs-lookup"><span data-stu-id="6da87-108">I don't understand the difference between delegated and application permissions</span></span>](https://docs.microsoft.com/azure/active-directory/develop/delegated-and-app-perms)

<span data-ttu-id="6da87-109">\***Край на поддръжката за библиотеката за удостоверяване на Azure Active Directory (ADAL) и API за AZURE ad Graph (пад Graph)** _</span><span class="sxs-lookup"><span data-stu-id="6da87-109">\***End of support for Azure Active Directory Authentication Library (ADAL) and Azure AD Graph API (AAD Graph)** _</span></span>

- <span data-ttu-id="6da87-110">Започвайки от 30 юни 2020, повече няма да добавяме нови функции към библиотеката за удостоверяване на Azure Active Directory (ADAL) и API на Azure AD Graph (пад Graph).</span><span class="sxs-lookup"><span data-stu-id="6da87-110">Starting June 30th, 2020, we will no longer add any new features to Azure Active Directory Authentication Library (ADAL) and Azure AD Graph API (AAD Graph).</span></span> <span data-ttu-id="6da87-111">Ще продължим да предоставяме техническа поддръжка и актуализации на защитата, но повече няма да предоставяме актуализации на функции.</span><span class="sxs-lookup"><span data-stu-id="6da87-111">We will continue to provide technical support and security updates but will no longer provide feature updates.</span></span>

- <span data-ttu-id="6da87-112">Започвайки от 30 юни 2022, ние ще сложим край на поддръжката за ADAL и пад Graph и повече няма да предоставяме техническа поддръжка и актуализации на защитата.</span><span class="sxs-lookup"><span data-stu-id="6da87-112">Starting June 30th, 2022, we will end support for ADAL and AAD Graph and will no longer provide technical support or security updates.</span></span> <span data-ttu-id="6da87-113">В резултат на това условие по-долу са посочени следните последствия:</span><span class="sxs-lookup"><span data-stu-id="6da87-113">As a result of this condition, the following are the implications:</span></span>

    - <span data-ttu-id="6da87-114">Приложенията, използващи ADAL за съществуващите версии на операционната система, ще продължат да работят след този час, но няма да получат техническа поддръжка или актуализация на защитата.</span><span class="sxs-lookup"><span data-stu-id="6da87-114">Apps using ADAL on existing OS versions will continue to work after this time but will not get any technical support or security updates.</span></span>

    - <span data-ttu-id="6da87-115">Приложенията, използващи пад Graph след този час, вече не могат да получават отговори от крайна точка на графиката с пад</span><span class="sxs-lookup"><span data-stu-id="6da87-115">Apps using AAD Graph after this time may no longer receive responses from the AAD Graph endpoint</span></span>

<span data-ttu-id="6da87-116">_ *ADALна миграция*\*</span><span class="sxs-lookup"><span data-stu-id="6da87-116">_ *ADAL Migration*\*</span></span>

<span data-ttu-id="6da87-117">Ако използвате приложения на Microsoft, ви препоръчваме да актуализирате до библиотеката за удостоверяване на Microsoft (MSAL), която има най-новите функции и актуализации на защитата.</span><span class="sxs-lookup"><span data-stu-id="6da87-117">If you're using Microsoft apps, we recommend updating to the Microsoft Authentication Library (MSAL), which has the latest features and security updates.</span></span> <span data-ttu-id="6da87-118">Тази препоръка е в контекста на Microsoft за започване на процеса на мигриране на приложенията към MSAL от крайния срок за поддръжка.</span><span class="sxs-lookup"><span data-stu-id="6da87-118">This recommendation is in the context of Microsoft initiating the process of migrating its apps to MSAL by the end-of-support deadline.</span></span> 

<span data-ttu-id="6da87-119">Мигрирането от Microsoft на приложенията към MSAL гарантира, че приложенията се възползват от текущите подобрения в защитата и функциите на MSAL.</span><span class="sxs-lookup"><span data-stu-id="6da87-119">The migration by Microsoft of its apps to MSAL ensures that the apps benefit from MSAL's ongoing security and feature improvements.</span></span>

1. [<span data-ttu-id="6da87-120">Прочетете ЧЗВ за ADAL</span><span class="sxs-lookup"><span data-stu-id="6da87-120">Read the ADAL FAQ</span></span>](https://docs.microsoft.com/azure/active-directory/develop/msal-migration#frequently-asked-questions-faq) 
2. [<span data-ttu-id="6da87-121">Научете повече за това как да мигрирате приложения на база платформа</span><span class="sxs-lookup"><span data-stu-id="6da87-121">Learn about how to migrate apps on a per-platform basis</span></span>](https://docs.microsoft.com/azure/active-directory/develop/msal-migration#frequently-asked-questions-faq) 
3. <span data-ttu-id="6da87-122">Ако имате нужда от помощ, за да разберете кой от вашите приложения използва ADAL, ви препоръчваме да прегледате всички изходния код на вашите приложения и, ако е приложимо, да се свържете с всички независими доставчици на софтуер (ISV) или доставчици на приложения.</span><span class="sxs-lookup"><span data-stu-id="6da87-122">If you need help in understanding which of your apps use ADAL, we recommend you review all of your apps' source code and, if applicable, reach out to any independent software vendors (ISVs) or app providers.</span></span> <span data-ttu-id="6da87-123">Поддръжката на Microsoft може да ви предостави и списък с всички приложения, които не са на Microsoft ADAL, във вашия клиент.</span><span class="sxs-lookup"><span data-stu-id="6da87-123">Microsoft support can also provide you with a list of all non-Microsoft ADAL apps in your tenant.</span></span>

<span data-ttu-id="6da87-124">**Преминаване към графиката в пад**</span><span class="sxs-lookup"><span data-stu-id="6da87-124">**AAD Graph Migration**</span></span>

<span data-ttu-id="6da87-125">За приложенията, които използват пад Graph, следвайте нашите указания за мигриране на приложения на "пад Graph" към Microsoft Graph:</span><span class="sxs-lookup"><span data-stu-id="6da87-125">For applications that are using AAD Graph, follow our guidance to migrate AAD Graph apps to Microsoft Graph:</span></span>

1. <span data-ttu-id="6da87-126">[Нашият контролен списък за мигриране предоставя първи стъпки](https://docs.microsoft.com/graph/migrate-azure-ad-graph-planning-checklist).</span><span class="sxs-lookup"><span data-stu-id="6da87-126">[Our migration checklist provides a getting started point](https://docs.microsoft.com/graph/migrate-azure-ad-graph-planning-checklist).</span></span> 
2. <span data-ttu-id="6da87-127">Вашият портал за регистрация на Azure App показва кои приложения използват пад Graph.</span><span class="sxs-lookup"><span data-stu-id="6da87-127">Your Azure app registration portal shows which applications are using AAD Graph.</span></span> <span data-ttu-id="6da87-128">Препоръчваме ви да прегледате всички изходни кодове на вашите приложения и, ако е приложимо, да се свържете с всички независими доставчици на софтуер (ISV) или с доставчиците на приложения.</span><span class="sxs-lookup"><span data-stu-id="6da87-128">We recommend you review all of your apps' source code and, if applicable, reach out to any independent software vendors (ISVs) or app providers.</span></span> <span data-ttu-id="6da87-129">Поддръжката на Microsoft може да ви предостави и информация за използването на пад Graph във вашия клиент.</span><span class="sxs-lookup"><span data-stu-id="6da87-129">Microsoft support can also provide you information on AAD Graph usage in your tenant.</span></span>







