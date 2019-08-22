---
title: Dynamics 365 - грешен таблото показва в Dynamics 365 унифициран интерфейс
ms.author: pebaum
author: pebaum
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1484"
- "6200024"
ms.openlocfilehash: 3d7258bdd7366f679b048e93926ab7dfe0b956d9
ms.sourcegitcommit: 1d98db8acb9959aba3b5e308a567ade6b62da56c
ms.translationtype: MT
ms.contentlocale: bg-BG
ms.lasthandoff: 08/22/2019
ms.locfileid: "36528540"
---
# <a name="wrong-dashboard-shows-in-dynamics-365-unified-interface"></a><span data-ttu-id="68aaa-102">Грешен таблото показва в Dynamics 365 унифициран интерфейс</span><span class="sxs-lookup"><span data-stu-id="68aaa-102">Wrong dashboard shows in Dynamics 365 unified interface</span></span>

<span data-ttu-id="68aaa-103">Има няколко причини, можете да видите различна табло от тази, която очаквате:</span><span class="sxs-lookup"><span data-stu-id="68aaa-103">There are several reasons why you may see a different dashboard than the one you expect:</span></span>

## <a name="the-user-has-set-a-user-default-dashboard"></a><span data-ttu-id="68aaa-104">Потребителят е задал дадено потребителско табло по подразбиране</span><span class="sxs-lookup"><span data-stu-id="68aaa-104">The user has set a user default dashboard</span></span> 

<span data-ttu-id="68aaa-105">Обикновено можете да идентифицирате потребителско табло по подразбиране е настроен ако бутона **Задаване като по подразбиране** не се показват в таблото командната лента.</span><span class="sxs-lookup"><span data-stu-id="68aaa-105">Typically you can identify a user default dashboard is set if the **Set As Default** button does not show in the dashboard command bar.</span></span> <span data-ttu-id="68aaa-106">Таблото на потребителя по подразбиране ще замести всички други табла по подразбиране, дори ако на потребителя табло по подразбиране не е в текущата ап.</span><span class="sxs-lookup"><span data-stu-id="68aaa-106">The user default dashboard will override all other default dashboards, even if the user's default dashboard is not in the current app.</span></span>

<span data-ttu-id="68aaa-107">Употреба определителен член последователи workaround към изключено табло им по подразбиране.</span><span class="sxs-lookup"><span data-stu-id="68aaa-107">Use the following workaround to unset their default dashboard.</span></span>

1. <span data-ttu-id="68aaa-108">Създаване на нов личен табло.</span><span class="sxs-lookup"><span data-stu-id="68aaa-108">Create a new personal dashboard.</span></span>

2. <span data-ttu-id="68aaa-109">Задаване на това ново табло по подразбиране за потребителя.</span><span class="sxs-lookup"><span data-stu-id="68aaa-109">Set that new dashboard as the user default.</span></span>

3. <span data-ttu-id="68aaa-110">Изтриване на това табло.</span><span class="sxs-lookup"><span data-stu-id="68aaa-110">Delete that dashboard.</span></span>

## <a name="the-dashboard-is-set-in-the-sitemap"></a><span data-ttu-id="68aaa-111">Таблото е разположен в сайта на</span><span class="sxs-lookup"><span data-stu-id="68aaa-111">The dashboard is set in the sitemap</span></span>

<span data-ttu-id="68aaa-112">Може да задали организация табло по подразбиране, като изберете табло и изберете "По подразбиране" под "Персонализиране на системата".</span><span class="sxs-lookup"><span data-stu-id="68aaa-112">You may have set an organization default dashboard by selecting a dashboard and choosing 'Set As Default' under 'Customize The System'.</span></span> <span data-ttu-id="68aaa-113">Но таблото, дефинирани в сайта дизайнер ще имат предимство пред този табло, ако потребителят има достъп до него.</span><span class="sxs-lookup"><span data-stu-id="68aaa-113">But the dashboard defined in the sitemap designer will take precedence over this dashboard, if the user has access to it.</span></span>

<span data-ttu-id="68aaa-114">За да видите на таблото, сте задали като организация по подразбиране на потребителите, можете:</span><span class="sxs-lookup"><span data-stu-id="68aaa-114">To have users see the dashboard you've set as the organization default, you can either:</span></span>

* <span data-ttu-id="68aaa-115">Задаване на това табло в сайта на</span><span class="sxs-lookup"><span data-stu-id="68aaa-115">Set that dashboard in the sitemap</span></span>

* <span data-ttu-id="68aaa-116">Премахване на достъп до сайта дефинирани таблото за тези потребители</span><span class="sxs-lookup"><span data-stu-id="68aaa-116">Remove access to the sitemap defined dashboard for those users</span></span>
