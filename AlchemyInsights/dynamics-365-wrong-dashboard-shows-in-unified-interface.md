---
title: Dynamics 365 – неправилни показвания на таблото в Dynamics 365 унифициран интерфейс
ms.author: pebaum
author: pebaum
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1484"
- "6200024"
ms.openlocfilehash: 02e33c7dbdfe9b7d2ad7a04f154cf067fba0aab2
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: bg-BG
ms.lasthandoff: 09/14/2020
ms.locfileid: "47711264"
---
# <a name="wrong-dashboard-shows-in-dynamics-365-unified-interface"></a><span data-ttu-id="93464-102">Грешен изглед на таблото в Dynamics 365 унифициран интерфейс</span><span class="sxs-lookup"><span data-stu-id="93464-102">Wrong dashboard shows in Dynamics 365 unified interface</span></span>

<span data-ttu-id="93464-103">Има няколко причини, поради които може да видите различно табло от това, което очаквате:</span><span class="sxs-lookup"><span data-stu-id="93464-103">There are several reasons why you may see a different dashboard than the one you expect:</span></span>

## <a name="the-user-has-set-a-user-default-dashboard"></a><span data-ttu-id="93464-104">Потребителят е задал потребителско табло по подразбиране</span><span class="sxs-lookup"><span data-stu-id="93464-104">The user has set a user default dashboard</span></span> 

<span data-ttu-id="93464-105">Обикновено можете да идентифицирате потребителско табло по подразбиране е зададено, ако бутонът **Задай като по подразбиране** не се показва в командната лента на таблото.</span><span class="sxs-lookup"><span data-stu-id="93464-105">Typically you can identify a user default dashboard is set if the **Set As Default** button does not show in the dashboard command bar.</span></span> <span data-ttu-id="93464-106">Таблото на потребителските подразбирания ще замести всички други табла по подразбиране дори ако таблото по подразбиране на потребителя не е в текущото приложение.</span><span class="sxs-lookup"><span data-stu-id="93464-106">The user default dashboard will override all other default dashboards, even if the user's default dashboard is not in the current app.</span></span>

<span data-ttu-id="93464-107">Използвайте следните заобиколни решения, за да унищожите тяхното табло по подразбиране.</span><span class="sxs-lookup"><span data-stu-id="93464-107">Use the following workaround to unset their default dashboard.</span></span>

1. <span data-ttu-id="93464-108">Създаване на ново лично табло.</span><span class="sxs-lookup"><span data-stu-id="93464-108">Create a new personal dashboard.</span></span>

2. <span data-ttu-id="93464-109">Задайте новото табло като потребителско по подразбиране.</span><span class="sxs-lookup"><span data-stu-id="93464-109">Set that new dashboard as the user default.</span></span>

3. <span data-ttu-id="93464-110">Изтриване на това табло.</span><span class="sxs-lookup"><span data-stu-id="93464-110">Delete that dashboard.</span></span>

## <a name="the-dashboard-is-set-in-the-sitemap"></a><span data-ttu-id="93464-111">Таблото е зададено на карта на сайта</span><span class="sxs-lookup"><span data-stu-id="93464-111">The dashboard is set in the sitemap</span></span>

<span data-ttu-id="93464-112">Може да сте задали табло по подразбиране на организацията, като изберете табло и изберете "Задай по подразбиране" под "Персонализиране на системата".</span><span class="sxs-lookup"><span data-stu-id="93464-112">You may have set an organization default dashboard by selecting a dashboard and choosing 'Set As Default' under 'Customize The System'.</span></span> <span data-ttu-id="93464-113">Но таблото, дефинирано в конструктора на Sitemap, ще има предимство пред това табло, ако потребителят има достъп до него.</span><span class="sxs-lookup"><span data-stu-id="93464-113">But the dashboard defined in the sitemap designer will take precedence over this dashboard, if the user has access to it.</span></span>

<span data-ttu-id="93464-114">За да могат потребителите да виждат таблото, което сте задали като организация по подразбиране, можете да направите едно от следните:</span><span class="sxs-lookup"><span data-stu-id="93464-114">To have users see the dashboard you've set as the organization default, you can either:</span></span>

* <span data-ttu-id="93464-115">Задаване на табло в карта на сайта</span><span class="sxs-lookup"><span data-stu-id="93464-115">Set that dashboard in the sitemap</span></span>

* <span data-ttu-id="93464-116">Премахване на достъпа до дефинираните табло на Sitemap за тези потребители</span><span class="sxs-lookup"><span data-stu-id="93464-116">Remove access to the sitemap defined dashboard for those users</span></span>
