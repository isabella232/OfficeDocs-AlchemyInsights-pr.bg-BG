---
title: Работният поток не започва
ms.author: pebaum
author: pebaum
manager: pamgreen
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000144"
- "1670"
ms.openlocfilehash: 941e6349c98278a1a8cdac77457ec1cc72cdef8b
ms.sourcegitcommit: 631cbb5f03e5371f0995e976536d24e9d13746c3
ms.translationtype: MT
ms.contentlocale: bg-BG
ms.lasthandoff: 04/22/2020
ms.locfileid: "43766086"
---
# <a name="workflow-is-not-starting"></a><span data-ttu-id="30065-102">Работният поток не започва</span><span class="sxs-lookup"><span data-stu-id="30065-102">Workflow is not starting</span></span>

- <span data-ttu-id="30065-103">SharePoint 2010 и SharePoint 2013 работни потоци не се стартира.</span><span class="sxs-lookup"><span data-stu-id="30065-103">SharePoint 2010 and SharePoint 2013 workflows are not starting.</span></span>

    - <span data-ttu-id="30065-104">Ако вашият работен поток не се стартира, може да има временен проблем, когато потребителите могат да възникнат временни забавяния с напредъка на работния поток.</span><span class="sxs-lookup"><span data-stu-id="30065-104">If your workflow is not starting, there may be a temporary service issue where users may experience intermittent delays with workflow progress.</span></span> <span data-ttu-id="30065-105">Проверете [таблото за изправност](https:/admin.microsoft.com/AdminPortal/Home#/servicehealth) на услугата, за да видите дали вашата организация е повлияна.</span><span class="sxs-lookup"><span data-stu-id="30065-105">Check the [Service Health Dashboard](https:/admin.microsoft.com/AdminPortal/Home#/servicehealth) to see if your organization is impacted.</span></span>

    - <span data-ttu-id="30065-106">Ако са изминали повече от 24 часа, откакто за първи път видяхте този проблем, моля, регистрирайте билет за поддръжка.</span><span class="sxs-lookup"><span data-stu-id="30065-106">If more than 24 hours have passed since you first saw this issue, please log a support ticket.</span></span> <span data-ttu-id="30065-107">В много случаи вече работим по решение.</span><span class="sxs-lookup"><span data-stu-id="30065-107">In many cases, we're already working on a solution.</span></span> <span data-ttu-id="30065-108">Моля, дайте ни поне 24 часа, за да завършите решение.</span><span class="sxs-lookup"><span data-stu-id="30065-108">Please give us at least 24 hours to complete a solution.</span></span>

- <span data-ttu-id="30065-109">SharePoint 2010 работни потоци забавяне при стартиране.</span><span class="sxs-lookup"><span data-stu-id="30065-109">SharePoint 2010 workflows delayed on start.</span></span>

    - <span data-ttu-id="30065-110">Това се случва, ако поток се задейства в големи папки.</span><span class="sxs-lookup"><span data-stu-id="30065-110">This occurs if the workflow is triggered in large batches.</span></span> <span data-ttu-id="30065-111">(например, когато се добавят няколко елемента едновременно).</span><span class="sxs-lookup"><span data-stu-id="30065-111">(for example, when several items are added at once).</span></span>

    - <span data-ttu-id="30065-112">Работните потоци не са проектирани да работят в реално време, така че забавянето е по-проектно поведение.</span><span class="sxs-lookup"><span data-stu-id="30065-112">Workflows are not designed to run real-time, so a delay is by-design behavior.</span></span>

   -  <span data-ttu-id="30065-113">Ако работният поток е сложен разширим обект markup Language (XMOL), компилация може да бъде бавно.</span><span class="sxs-lookup"><span data-stu-id="30065-113">If the Workflow is complex Extensible Object Markup Language (XMOL), compilation can be slow.</span></span> <span data-ttu-id="30065-114">Проверете [тази](https://support.microsoft.com//kb/3043697) статия.</span><span class="sxs-lookup"><span data-stu-id="30065-114">Check [this](https://support.microsoft.com//kb/3043697) article.</span></span>

    - <span data-ttu-id="30065-115">Трябва да опрости работния поток или да го редизайн с помощта на microsoft SharePoint 2013 поток платформа тип.</span><span class="sxs-lookup"><span data-stu-id="30065-115">You should simplify the workflow or redesign it using the Microsoft SharePoint 2013 Workflow platform type.</span></span>

    - <span data-ttu-id="30065-116">Ако вашата хронология на работния поток е нараснала, може да искате да изчистите елементите или да създадете нов списък с хронология.</span><span class="sxs-lookup"><span data-stu-id="30065-116">If your workflow history has grown large, you may want to purge the items or create a new history list.</span></span>

        <span data-ttu-id="30065-117">Повече информация: [Прочистване на хронологията на работния поток](https://blogs.technet.microsoft.com/marj/2015/08/07/sharepoint-2010-workflows-best-practice-purge-workflow-history-list-items/)</span><span class="sxs-lookup"><span data-stu-id="30065-117">More Information : [Purge Workflow History](https://blogs.technet.microsoft.com/marj/2015/08/07/sharepoint-2010-workflows-best-practice-purge-workflow-history-list-items/)</span></span>


## <a name="related-topics"></a><span data-ttu-id="30065-118">Сродни теми</span><span class="sxs-lookup"><span data-stu-id="30065-118">Related topics</span></span>
<span data-ttu-id="30065-119">Искате ли да опитате Microsoft Flow в SharePoint Online?</span><span class="sxs-lookup"><span data-stu-id="30065-119">Want to try Microsoft Flow in SharePoint Online?</span></span>
- [<span data-ttu-id="30065-120">Създаване на поток</span><span class="sxs-lookup"><span data-stu-id="30065-120">Create Flow</span></span>](https://support.office.com/article/Create-a-flow-for-a-list-or-library-in-SharePoint-Online-or-OneDrive-for-Business-a9c3e03b-0654-46af-a254-20252e580d01) 
- [<span data-ttu-id="30065-121">SharePoint и поток</span><span class="sxs-lookup"><span data-stu-id="30065-121">SharePoint and Flow</span></span>](https://flow.microsoft.com/blog/sharepoint-and-flow/) 


