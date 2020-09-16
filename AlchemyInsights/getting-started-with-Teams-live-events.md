---
title: Първи стъпки в събитията на живо на Teams
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9000208"
- "3436"
ms.openlocfilehash: 979555a6fba46437adaf7e8c201cb9d6c4a8e965
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: bg-BG
ms.lasthandoff: 09/14/2020
ms.locfileid: "47677268"
---
# <a name="getting-started-with-teams-live-events"></a><span data-ttu-id="7f2cf-102">Първи стъпки в събитията на живо на Teams</span><span class="sxs-lookup"><span data-stu-id="7f2cf-102">Getting started with Teams live events</span></span>

<span data-ttu-id="7f2cf-103">Събитията на живо на Microsoft Teams са разширение на събранията на Teams, които ви позволяват да планирате и да създавате събития, които излъчват поточно за големи онлайн аудитории.</span><span class="sxs-lookup"><span data-stu-id="7f2cf-103">Microsoft Teams live events are an extension of Teams meetings that enable you to schedule and produce events that stream to large online audiences.</span></span>

<span data-ttu-id="7f2cf-104">За да създадете събитие на живо, ще ви трябва следното:</span><span class="sxs-lookup"><span data-stu-id="7f2cf-104">To create a live event, you will need the following:</span></span>

- <span data-ttu-id="7f2cf-105">Първо, уверете се, че събития на живо в Teams са [налични във вашата страна и регион](https://docs.microsoft.com/microsoftteams/teams-live-events/plan-for-teams-live-events#regional-availability); В някои страни все още не се поддържат събития на живо.</span><span class="sxs-lookup"><span data-stu-id="7f2cf-105">First, confirm that Teams Live Events are [available in your Country and Region](https://docs.microsoft.com/microsoftteams/teams-live-events/plan-for-teams-live-events#regional-availability); Live Events are not yet supported in some countries.</span></span>  <span data-ttu-id="7f2cf-106">Ако сте присвоили лицензи и сте задали правила, но все още не можете да създадете събитие на живо в Teams, е вероятно да сте в страна или регион, където събития на живо все още не са налични.</span><span class="sxs-lookup"><span data-stu-id="7f2cf-106">If you’ve assigned licenses and set policies, but still cannot create a Teams Live Event, it is likely you are in a Country or Region where Live Events is not yet available.</span></span>

- <span data-ttu-id="7f2cf-107">Лиценз за [Office 365 Enterprise E1, E3 или E5 или лиценз за Office 365 A3 или A5](https://docs.microsoft.com/microsoftteams/teams-live-events/set-up-for-teams-live-events#step-2-get-and-assign-licenses).</span><span class="sxs-lookup"><span data-stu-id="7f2cf-107">An [Office 365 Enterprise E1, E3, or E5 license or an Office 365 A3 or A5 license](https://docs.microsoft.com/microsoftteams/teams-live-events/set-up-for-teams-live-events#step-2-get-and-assign-licenses).</span></span> <span data-ttu-id="7f2cf-108">**Забележка**: поради нарастването на използването на Teams в последно време, когато присвоявате лиценз за Teams на потребител, това може да отнеме около 24 часа, преди да бъде напълно настроен.</span><span class="sxs-lookup"><span data-stu-id="7f2cf-108">**Note**: Due to a recent increase in Teams usage, when you assign a Teams license to a user, it may take around 24 hours before they'll be fully set up.</span></span> <span data-ttu-id="7f2cf-109">Дотогава няма да можете да присвоявате правилата на Teams за тях и те може да нямат достъп до някои функции на екипа, например разговори и аудио конференции.</span><span class="sxs-lookup"><span data-stu-id="7f2cf-109">Until then, you won't be able to assign Teams policies to them, and they might not have access to some Teams features like calling and audio conferencing.</span></span>

- <span data-ttu-id="7f2cf-110">Разрешение за [продуциране на събития на живо в центъра за администриране на Microsoft Teams](https://docs.microsoft.com/microsoftteams/teams-live-events/set-up-for-teams-live-events#create-or-edit-a-live-events-policy).</span><span class="sxs-lookup"><span data-stu-id="7f2cf-110">Permission to [create live events in Microsoft Teams admin center](https://docs.microsoft.com/microsoftteams/teams-live-events/set-up-for-teams-live-events#create-or-edit-a-live-events-policy).</span></span>

- <span data-ttu-id="7f2cf-111">Разрешение за [създаване на събития на живо в Microsoft Stream](https://docs.microsoft.com/microsoftteams/teams-live-events/what-are-teams-live-events) (за събития, които са продуцирани чрез външно приложение или устройство за излъчване).</span><span class="sxs-lookup"><span data-stu-id="7f2cf-111">Permission to [create live events in Microsoft Stream](https://docs.microsoft.com/microsoftteams/teams-live-events/what-are-teams-live-events) (for events produced using an external broadcasting app or device).</span></span>

- <span data-ttu-id="7f2cf-112">Пълноправно членство в екипа в организацията (не като гост или от друга организация).</span><span class="sxs-lookup"><span data-stu-id="7f2cf-112">Full team membership in the org (can't be a guest or from another org).</span></span>
<span data-ttu-id="7f2cf-113">Планиране на частни събрания, споделяне на екрана и споделяне на IP видео, включено в правилата за събрания на Teams.</span><span class="sxs-lookup"><span data-stu-id="7f2cf-113">Private meeting scheduling, screensharing, and IP video sharing, turned on in Team meeting policy.</span></span>

- <span data-ttu-id="7f2cf-114">[Най-добри практики](https://support.office.com/article/Best-practices-for-producing-a-Teams-live-event-e500370e-4dd1-4187-8b48-af10ef02cf42) за събития на живо на Teams.</span><span class="sxs-lookup"><span data-stu-id="7f2cf-114">[Best practices](https://support.office.com/article/Best-practices-for-producing-a-Teams-live-event-e500370e-4dd1-4187-8b48-af10ef02cf42) for Teams Live Events.</span></span>

<span data-ttu-id="7f2cf-115">За повече информация вижте [Първи стъпки в събитията на живо на Microsoft Teams](https://support.office.com/article/get-started-with-microsoft-teams-live-events-d077fec2-a058-483e-9ab5-1494afda578a).</span><span class="sxs-lookup"><span data-stu-id="7f2cf-115">For more information, please see [Get started with Microsoft Teams live events](https://support.office.com/article/get-started-with-microsoft-teams-live-events-d077fec2-a058-483e-9ab5-1494afda578a).</span></span>