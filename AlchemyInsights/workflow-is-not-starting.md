---
title: Работният поток не се стартира
ms.author: pebaum
author: pebaum
manager: pamgreen
ms.date: 8/2/2019
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000144"
- "1670"
ms.openlocfilehash: cf7bd95e9a8f1d0842f0abcf82c758d649e80c0f
ms.sourcegitcommit: 0f0186044a3597e42ad14c32ca58e7224344dcfa
ms.translationtype: MT
ms.contentlocale: bg-BG
ms.lasthandoff: 12/15/2019
ms.locfileid: "40049326"
---
# <a name="workflow-is-not-starting"></a><span data-ttu-id="06ab8-102">Работният поток не се стартира</span><span class="sxs-lookup"><span data-stu-id="06ab8-102">Workflow is not starting</span></span>

- <span data-ttu-id="06ab8-103">SharePoint 2010 и SharePoint 2013 работни потоци не се стартира.</span><span class="sxs-lookup"><span data-stu-id="06ab8-103">SharePoint 2010 and SharePoint 2013 workflows are not starting.</span></span>

    - <span data-ttu-id="06ab8-104">Ако вашият работен поток не се стартира, може да има временен проблем с услугата, при който потребителите могат да изпитват периодични закъснения с напредъка на работния поток.</span><span class="sxs-lookup"><span data-stu-id="06ab8-104">If your workflow is not starting, there may be a temporary service issue where users may experience intermittent delays with workflow progress.</span></span> <span data-ttu-id="06ab8-105">Проверете [услугата Health табло](https:/admin.microsoft.com/AdminPortal/Home#/servicehealth) , за да видите дали вашата организация е засегната.</span><span class="sxs-lookup"><span data-stu-id="06ab8-105">Check the [Service Health Dashboard](https:/admin.microsoft.com/AdminPortal/Home#/servicehealth) to see if your organization is impacted.</span></span>

    - <span data-ttu-id="06ab8-106">Ако са изминали повече от 24 часа от първия път, когато сте видели този проблем, моля, впишете билет за поддръжка.</span><span class="sxs-lookup"><span data-stu-id="06ab8-106">If more than 24 hours have passed since you first saw this issue, please log a support ticket.</span></span> <span data-ttu-id="06ab8-107">В много случаи вече работим по решение.</span><span class="sxs-lookup"><span data-stu-id="06ab8-107">In many cases, we're already working on a solution.</span></span> <span data-ttu-id="06ab8-108">Моля, дайте ни поне 24 часа, за да завършим решение.</span><span class="sxs-lookup"><span data-stu-id="06ab8-108">Please give us at least 24 hours to complete a solution.</span></span>

- <span data-ttu-id="06ab8-109">Работни потоци на SharePoint 2010 забавени при стартиране.</span><span class="sxs-lookup"><span data-stu-id="06ab8-109">SharePoint 2010 workflows delayed on start.</span></span>

    - <span data-ttu-id="06ab8-110">Това се случва, ако работният поток се задейства в големи папки.</span><span class="sxs-lookup"><span data-stu-id="06ab8-110">This occurs if the workflow is triggered in large batches.</span></span> <span data-ttu-id="06ab8-111">(например, когато няколко елемента се добавят наведнъж).</span><span class="sxs-lookup"><span data-stu-id="06ab8-111">(for example, when several items are added at once).</span></span>

    - <span data-ttu-id="06ab8-112">Работните потоци не са предназначени за изпълнение в реално време, така че забавянето е поведението по дизайн.</span><span class="sxs-lookup"><span data-stu-id="06ab8-112">Workflows are not designed to run real-time, so a delay is by-design behavior.</span></span>

   -  <span data-ttu-id="06ab8-113">Ако работният поток е сложен разширен обект маркиране език (XMOL), компилация може да бъде бавен.</span><span class="sxs-lookup"><span data-stu-id="06ab8-113">If the Workflow is complex Extensible Object Markup Language (XMOL), compilation can be slow.</span></span> <span data-ttu-id="06ab8-114">Проверете [тази](https://support.microsoft.com//kb/3043697) статия.</span><span class="sxs-lookup"><span data-stu-id="06ab8-114">Check [this](https://support.microsoft.com//kb/3043697) article.</span></span>

    - <span data-ttu-id="06ab8-115">Трябва да опростите работния поток или да го препроменяте с помощта на типа на платформата Microsoft SharePoint 2013 поток.</span><span class="sxs-lookup"><span data-stu-id="06ab8-115">You should simplify the workflow or redesign it using the Microsoft SharePoint 2013 Workflow platform type.</span></span>

    - <span data-ttu-id="06ab8-116">Ако хронологията на работния поток е пораснала голяма, може да искате да изчистите елементите или да създадете нов списък с хронология.</span><span class="sxs-lookup"><span data-stu-id="06ab8-116">If your workflow history has grown large, you may want to purge the items or create a new history list.</span></span>

        <span data-ttu-id="06ab8-117">Повече информация: [изчистване на хронологията на работния поток](https://blogs.technet.microsoft.com/marj/2015/08/07/sharepoint-2010-workflows-best-practice-purge-workflow-history-list-items/)</span><span class="sxs-lookup"><span data-stu-id="06ab8-117">More Information : [Purge Workflow History](https://blogs.technet.microsoft.com/marj/2015/08/07/sharepoint-2010-workflows-best-practice-purge-workflow-history-list-items/)</span></span>


## <a name="related-topics"></a><span data-ttu-id="06ab8-118">Сродни теми</span><span class="sxs-lookup"><span data-stu-id="06ab8-118">Related topics</span></span>
<span data-ttu-id="06ab8-119">Искате ли да опитате Microsoft Flow в SharePoint online?</span><span class="sxs-lookup"><span data-stu-id="06ab8-119">Want to try Microsoft Flow in SharePoint Online?</span></span>
- [<span data-ttu-id="06ab8-120">Създаване на поток</span><span class="sxs-lookup"><span data-stu-id="06ab8-120">Create Flow</span></span>](https://support.office.com/article/Create-a-flow-for-a-list-or-library-in-SharePoint-Online-or-OneDrive-for-Business-a9c3e03b-0654-46af-a254-20252e580d01) 
- [<span data-ttu-id="06ab8-121">SharePoint и поток</span><span class="sxs-lookup"><span data-stu-id="06ab8-121">SharePoint and Flow</span></span>](https://flow.microsoft.com/blog/sharepoint-and-flow/) 


