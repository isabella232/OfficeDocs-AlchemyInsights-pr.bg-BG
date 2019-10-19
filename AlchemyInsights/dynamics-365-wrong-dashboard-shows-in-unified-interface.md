---
title: Dynamics 365 – неправилно табло показва в Dynamics 365 унифициран интерфейс
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
ms.sourcegitcommit: 037331d71f06750d972c0b6278b23bb15c4806ca
ms.translationtype: MT
ms.contentlocale: bg-BG
ms.lasthandoff: 10/18/2019
ms.locfileid: "36528540"
---
# <a name="wrong-dashboard-shows-in-dynamics-365-unified-interface"></a><span data-ttu-id="9880d-102">Грешно табло показва в Dynamics 365 унифициран интерфейс</span><span class="sxs-lookup"><span data-stu-id="9880d-102">Wrong dashboard shows in Dynamics 365 unified interface</span></span>

<span data-ttu-id="9880d-103">Има няколко причини, поради които може да видите различно табло от това, което очаквате:</span><span class="sxs-lookup"><span data-stu-id="9880d-103">There are several reasons why you may see a different dashboard than the one you expect:</span></span>

## <a name="the-user-has-set-a-user-default-dashboard"></a><span data-ttu-id="9880d-104">Потребителят е задали потребителско табло по подразбиране</span><span class="sxs-lookup"><span data-stu-id="9880d-104">The user has set a user default dashboard</span></span> 

<span data-ttu-id="9880d-105">Обикновено можете да идентифицирате потребителско табло по подразбиране е зададено, ако бутона " **Задай по подразбиране** " не се показва в командната лента на таблото.</span><span class="sxs-lookup"><span data-stu-id="9880d-105">Typically you can identify a user default dashboard is set if the **Set As Default** button does not show in the dashboard command bar.</span></span> <span data-ttu-id="9880d-106">Таблото по подразбиране на потребителя ще замести всички други табла по подразбиране, дори ако таблото по подразбиране на потребителя не е в текущото приложение.</span><span class="sxs-lookup"><span data-stu-id="9880d-106">The user default dashboard will override all other default dashboards, even if the user's default dashboard is not in the current app.</span></span>

<span data-ttu-id="9880d-107">Използвайте следния заобиколно решение за изключено тяхното табло по подразбиране.</span><span class="sxs-lookup"><span data-stu-id="9880d-107">Use the following workaround to unset their default dashboard.</span></span>

1. <span data-ttu-id="9880d-108">Създаване на ново лично табло.</span><span class="sxs-lookup"><span data-stu-id="9880d-108">Create a new personal dashboard.</span></span>

2. <span data-ttu-id="9880d-109">Задайте това ново табло като потребител по подразбиране.</span><span class="sxs-lookup"><span data-stu-id="9880d-109">Set that new dashboard as the user default.</span></span>

3. <span data-ttu-id="9880d-110">Изтрийте това табло.</span><span class="sxs-lookup"><span data-stu-id="9880d-110">Delete that dashboard.</span></span>

## <a name="the-dashboard-is-set-in-the-sitemap"></a><span data-ttu-id="9880d-111">Таблото е зададено в сайта</span><span class="sxs-lookup"><span data-stu-id="9880d-111">The dashboard is set in the sitemap</span></span>

<span data-ttu-id="9880d-112">Може да сте задали табло по подразбиране за организация, като изберете табло и изберете "Задай по подразбиране" под "Персонализиране на системата".</span><span class="sxs-lookup"><span data-stu-id="9880d-112">You may have set an organization default dashboard by selecting a dashboard and choosing 'Set As Default' under 'Customize The System'.</span></span> <span data-ttu-id="9880d-113">Но таблото, дефинирано в дизайнера на сайта, ще има предимство пред това табло, ако потребителят има достъп до него.</span><span class="sxs-lookup"><span data-stu-id="9880d-113">But the dashboard defined in the sitemap designer will take precedence over this dashboard, if the user has access to it.</span></span>

<span data-ttu-id="9880d-114">За да може потребителите да виждат таблото, което сте задали като организация по подразбиране, можете или:</span><span class="sxs-lookup"><span data-stu-id="9880d-114">To have users see the dashboard you've set as the organization default, you can either:</span></span>

* <span data-ttu-id="9880d-115">Задаване на таблото в сайта</span><span class="sxs-lookup"><span data-stu-id="9880d-115">Set that dashboard in the sitemap</span></span>

* <span data-ttu-id="9880d-116">Премахване на достъпа до определено табло на сайта за тези потребители</span><span class="sxs-lookup"><span data-stu-id="9880d-116">Remove access to the sitemap defined dashboard for those users</span></span>
