---
title: Работният поток не започва
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
ms.openlocfilehash: e69f3e529e4a2202f641cb62f42b1a20d774a398
ms.sourcegitcommit: db908b3da2c7a6508a77bf4f2c80afb294fadbd1
ms.translationtype: MT
ms.contentlocale: bg-BG
ms.lasthandoff: 03/29/2021
ms.locfileid: "51403732"
---
# <a name="workflow-is-not-starting"></a><span data-ttu-id="9603e-102">Работният поток не започва</span><span class="sxs-lookup"><span data-stu-id="9603e-102">Workflow is not starting</span></span>

- <span data-ttu-id="9603e-103">Работните потоци на SharePoint 2010 и SharePoint 2013 не се стартират.</span><span class="sxs-lookup"><span data-stu-id="9603e-103">SharePoint 2010 and SharePoint 2013 workflows are not starting.</span></span>

    - <span data-ttu-id="9603e-104">Ако вашият работен поток не се стартира, може да има временен проблем с услугата, при който потребителите може да изпитват неспоменато забавяне с напредъка на работния поток.</span><span class="sxs-lookup"><span data-stu-id="9603e-104">If your workflow is not starting, there may be a temporary service issue where users may experience intermittent delays with workflow progress.</span></span> <span data-ttu-id="9603e-105">Проверете [таблото за изтезания на](https://admin.microsoft.com/AdminPortal/Home/servicehealth) услугите, за да видите дали вашата организация е засегнати.</span><span class="sxs-lookup"><span data-stu-id="9603e-105">Check the [Service Health Dashboard](https://admin.microsoft.com/AdminPortal/Home/servicehealth) to see if your organization is impacted.</span></span>

    - <span data-ttu-id="9603e-106">Ако са минали повече от 24 часа, откакто за първи път сте видели този проблем, влезте в билет за поддръжка.</span><span class="sxs-lookup"><span data-stu-id="9603e-106">If more than 24 hours have passed since you first saw this issue, please log a support ticket.</span></span> <span data-ttu-id="9603e-107">В много случаи вече работим по решение.</span><span class="sxs-lookup"><span data-stu-id="9603e-107">In many cases, we're already working on a solution.</span></span> <span data-ttu-id="9603e-108">Дайте ни поне 24 часа, за да завършим решение.</span><span class="sxs-lookup"><span data-stu-id="9603e-108">Please give us at least 24 hours to complete a solution.</span></span>

- <span data-ttu-id="9603e-109">Работните потоци на SharePoint 2010 се забавят при стартиране.</span><span class="sxs-lookup"><span data-stu-id="9603e-109">SharePoint 2010 workflows delayed on start.</span></span>

    - <span data-ttu-id="9603e-110">Това се случва, ако работният поток се активира в големи партиди.</span><span class="sxs-lookup"><span data-stu-id="9603e-110">This occurs if the workflow is triggered in large batches.</span></span> <span data-ttu-id="9603e-111">(например когато се добавят няколко елемента наведнъж).</span><span class="sxs-lookup"><span data-stu-id="9603e-111">(for example, when several items are added at once).</span></span>

    - <span data-ttu-id="9603e-112">Работните потоци не са предназначени да се изпълняват в реално време, така че забавянето е поведението при проектиране.</span><span class="sxs-lookup"><span data-stu-id="9603e-112">Workflows are not designed to run real-time, so a delay is by-design behavior.</span></span>

   -  <span data-ttu-id="9603e-113">Ако работният поток е сложен език за маркиране на разширяеми обекти (XMOL), компилацията може да бъде бавна.</span><span class="sxs-lookup"><span data-stu-id="9603e-113">If the Workflow is complex Extensible Object Markup Language (XMOL), compilation can be slow.</span></span> <span data-ttu-id="9603e-114">Проверете [тази](https://support.microsoft.com//kb/3043697) статия.</span><span class="sxs-lookup"><span data-stu-id="9603e-114">Check [this](https://support.microsoft.com//kb/3043697) article.</span></span>

    - <span data-ttu-id="9603e-115">Трябва да опростите работния поток или да го пренавивате с помощта на типа платформа за работни потоци на Microsoft SharePoint 2013.</span><span class="sxs-lookup"><span data-stu-id="9603e-115">You should simplify the workflow or redesign it using the Microsoft SharePoint 2013 Workflow platform type.</span></span>

    - <span data-ttu-id="9603e-116">Ако хронологията на работния поток е нараснала голяма, може да искате да прочистите елементите или да създадете нов списък с хронология.</span><span class="sxs-lookup"><span data-stu-id="9603e-116">If your workflow history has grown large, you may want to purge the items or create a new history list.</span></span>

        <span data-ttu-id="9603e-117">Повече информация: [Изчистване на хронологията на работния поток](https://blogs.technet.microsoft.com/marj/2015/08/07/sharepoint-2010-workflows-best-practice-purge-workflow-history-list-items/)</span><span class="sxs-lookup"><span data-stu-id="9603e-117">More Information : [Purge Workflow History](https://blogs.technet.microsoft.com/marj/2015/08/07/sharepoint-2010-workflows-best-practice-purge-workflow-history-list-items/)</span></span>


## <a name="related-topics"></a><span data-ttu-id="9603e-118">Сродни теми</span><span class="sxs-lookup"><span data-stu-id="9603e-118">Related topics</span></span>
<span data-ttu-id="9603e-119">Искате да изпробвате Microsoft Flow в SharePoint Online?</span><span class="sxs-lookup"><span data-stu-id="9603e-119">Want to try Microsoft Flow in SharePoint Online?</span></span>
- [<span data-ttu-id="9603e-120">Създаване на поток</span><span class="sxs-lookup"><span data-stu-id="9603e-120">Create Flow</span></span>](https://support.office.com/article/Create-a-flow-for-a-list-or-library-in-SharePoint-Online-or-OneDrive-for-Business-a9c3e03b-0654-46af-a254-20252e580d01) 
- [<span data-ttu-id="9603e-121">SharePoint и Flow</span><span class="sxs-lookup"><span data-stu-id="9603e-121">SharePoint and Flow</span></span>](https://flow.microsoft.com/blog/sharepoint-and-flow/) 
