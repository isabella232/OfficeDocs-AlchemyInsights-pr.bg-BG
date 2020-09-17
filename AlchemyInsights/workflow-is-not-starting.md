---
title: Работният поток не се стартира
ms.author: pebaum
author: pebaum
manager: pamgreen
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000144"
- "1670"
ms.openlocfilehash: e3b8777ed74b812b31338784999eea43a95d3456
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: bg-BG
ms.lasthandoff: 09/15/2020
ms.locfileid: "47794756"
---
# <a name="workflow-is-not-starting"></a><span data-ttu-id="f7efe-102">Работният поток не се стартира</span><span class="sxs-lookup"><span data-stu-id="f7efe-102">Workflow is not starting</span></span>

- <span data-ttu-id="f7efe-103">Работните потоци на SharePoint 2010 и SharePoint 2013 не се стартират.</span><span class="sxs-lookup"><span data-stu-id="f7efe-103">SharePoint 2010 and SharePoint 2013 workflows are not starting.</span></span>

    - <span data-ttu-id="f7efe-104">Ако работният поток не се стартира, е възможно да има проблем с временен услуга, при който потребителите могат да се сблъскат с периодични закъснения с напредъка на работния поток.</span><span class="sxs-lookup"><span data-stu-id="f7efe-104">If your workflow is not starting, there may be a temporary service issue where users may experience intermittent delays with workflow progress.</span></span> <span data-ttu-id="f7efe-105">Проверете [таблото за изправност на услугите](https:/admin.microsoft.com/AdminPortal/Home#/servicehealth) , за да видите дали вашата организация е засегната.</span><span class="sxs-lookup"><span data-stu-id="f7efe-105">Check the [Service Health Dashboard](https:/admin.microsoft.com/AdminPortal/Home#/servicehealth) to see if your organization is impacted.</span></span>

    - <span data-ttu-id="f7efe-106">Ако са изминали повече от 24 часа, откакто за пръв път видяхте този проблем, можете да регистрирате билет за поддръжка.</span><span class="sxs-lookup"><span data-stu-id="f7efe-106">If more than 24 hours have passed since you first saw this issue, please log a support ticket.</span></span> <span data-ttu-id="f7efe-107">В много случаи вече работим върху решение.</span><span class="sxs-lookup"><span data-stu-id="f7efe-107">In many cases, we're already working on a solution.</span></span> <span data-ttu-id="f7efe-108">Моля, дайте ни най-малко 24 часа, за да завършите решение.</span><span class="sxs-lookup"><span data-stu-id="f7efe-108">Please give us at least 24 hours to complete a solution.</span></span>

- <span data-ttu-id="f7efe-109">Работните потоци на SharePoint 2010 се забавиха при стартиране.</span><span class="sxs-lookup"><span data-stu-id="f7efe-109">SharePoint 2010 workflows delayed on start.</span></span>

    - <span data-ttu-id="f7efe-110">Това се случва, ако работният поток се задейства в големи партиди.</span><span class="sxs-lookup"><span data-stu-id="f7efe-110">This occurs if the workflow is triggered in large batches.</span></span> <span data-ttu-id="f7efe-111">(например когато са добавени няколко елемента наведнъж).</span><span class="sxs-lookup"><span data-stu-id="f7efe-111">(for example, when several items are added at once).</span></span>

    - <span data-ttu-id="f7efe-112">Работните потоци не са предназначени да се изпълняват в реално време, така че закъснението е по-модел на поведение.</span><span class="sxs-lookup"><span data-stu-id="f7efe-112">Workflows are not designed to run real-time, so a delay is by-design behavior.</span></span>

   -  <span data-ttu-id="f7efe-113">Ако работният поток е сложен език за коректура на обекти (XMOL), съставянето може да бъде бавно.</span><span class="sxs-lookup"><span data-stu-id="f7efe-113">If the Workflow is complex Extensible Object Markup Language (XMOL), compilation can be slow.</span></span> <span data-ttu-id="f7efe-114">Проверете [тази](https://support.microsoft.com//kb/3043697) статия.</span><span class="sxs-lookup"><span data-stu-id="f7efe-114">Check [this](https://support.microsoft.com//kb/3043697) article.</span></span>

    - <span data-ttu-id="f7efe-115">Трябва да опростите работния поток или да го препроектирате, като използвате типа платформа на работен поток на Microsoft SharePoint 2013.</span><span class="sxs-lookup"><span data-stu-id="f7efe-115">You should simplify the workflow or redesign it using the Microsoft SharePoint 2013 Workflow platform type.</span></span>

    - <span data-ttu-id="f7efe-116">Ако вашата хронология на работния поток е нараснал голям, може да поискате да изчистите елементите или да създадете нов списък с хронологии.</span><span class="sxs-lookup"><span data-stu-id="f7efe-116">If your workflow history has grown large, you may want to purge the items or create a new history list.</span></span>

        <span data-ttu-id="f7efe-117">Още информация: [изчистване на хронологията на работния поток](https://blogs.technet.microsoft.com/marj/2015/08/07/sharepoint-2010-workflows-best-practice-purge-workflow-history-list-items/)</span><span class="sxs-lookup"><span data-stu-id="f7efe-117">More Information : [Purge Workflow History](https://blogs.technet.microsoft.com/marj/2015/08/07/sharepoint-2010-workflows-best-practice-purge-workflow-history-list-items/)</span></span>


## <a name="related-topics"></a><span data-ttu-id="f7efe-118">Сродни теми</span><span class="sxs-lookup"><span data-stu-id="f7efe-118">Related topics</span></span>
<span data-ttu-id="f7efe-119">Искате да изпробвате Microsoft Flow в SharePoint online?</span><span class="sxs-lookup"><span data-stu-id="f7efe-119">Want to try Microsoft Flow in SharePoint Online?</span></span>
- [<span data-ttu-id="f7efe-120">Създаване на поток</span><span class="sxs-lookup"><span data-stu-id="f7efe-120">Create Flow</span></span>](https://support.office.com/article/Create-a-flow-for-a-list-or-library-in-SharePoint-Online-or-OneDrive-for-Business-a9c3e03b-0654-46af-a254-20252e580d01) 
- [<span data-ttu-id="f7efe-121">SharePoint и Flow</span><span class="sxs-lookup"><span data-stu-id="f7efe-121">SharePoint and Flow</span></span>](https://flow.microsoft.com/blog/sharepoint-and-flow/) 


