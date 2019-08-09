---
title: Не стартиране на работен поток
ms.author: efrene
author: efrene
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
ms.openlocfilehash: a3bac74c19a77b7703f948c1d8b6bcd182e9b075
ms.sourcegitcommit: 631e527967f4d641bc9227642ffe38967ae87a00
ms.translationtype: MT
ms.contentlocale: bg-BG
ms.lasthandoff: 08/09/2019
ms.locfileid: "36270769"
---
# <a name="workflow-is-not-starting"></a><span data-ttu-id="fa1df-102">Не стартиране на работен поток</span><span class="sxs-lookup"><span data-stu-id="fa1df-102">Workflow is not starting</span></span>

- <span data-ttu-id="fa1df-103">SharePoint 2010 и SharePoint 2013 работни потоци не се започва.</span><span class="sxs-lookup"><span data-stu-id="fa1df-103">SharePoint 2010 and SharePoint 2013 workflows are not starting.</span></span>

    - <span data-ttu-id="fa1df-104">Ако не се стартира работния поток, може да има проблем при временна услуга където потребителите могат да изпитат прекъсвания отлагам с поток прогрес.</span><span class="sxs-lookup"><span data-stu-id="fa1df-104">If your workflow is not starting, there may be a temporary service issue where users may experience intermittent delays with workflow progress.</span></span> <span data-ttu-id="fa1df-105">Проверете [Услуги здравето таблото](https:/admin.microsoft.com/AdminPortal/Home#/servicehealth) за да видите дали вашата организация е ударена.</span><span class="sxs-lookup"><span data-stu-id="fa1df-105">Check the [Service Health Dashboard](https:/admin.microsoft.com/AdminPortal/Home#/servicehealth) to see if your organization is impacted.</span></span>

    - <span data-ttu-id="fa1df-106">Ако повече от 24 часа са изминали от вас за първи път видях този проблем, моля влезте билет подкрепа.</span><span class="sxs-lookup"><span data-stu-id="fa1df-106">If more than 24 hours have passed since you first saw this issue, please log a support ticket.</span></span> <span data-ttu-id="fa1df-107">В много случаи ние вече работим върху решение.</span><span class="sxs-lookup"><span data-stu-id="fa1df-107">In many cases, we're already working on a solution.</span></span> <span data-ttu-id="fa1df-108">Моля, дайте ни най-малко 24 часа да завършите решение.</span><span class="sxs-lookup"><span data-stu-id="fa1df-108">Please give us at least 24 hours to complete a solution.</span></span>

- <span data-ttu-id="fa1df-109">SharePoint 2010 работни потоци, които бавят Старт.</span><span class="sxs-lookup"><span data-stu-id="fa1df-109">SharePoint 2010 workflows delayed on start.</span></span>

    - <span data-ttu-id="fa1df-110">Това се случва, ако работният поток се задейства в големи партиди.</span><span class="sxs-lookup"><span data-stu-id="fa1df-110">This occurs if the workflow is triggered in large batches.</span></span> <span data-ttu-id="fa1df-111">(например, когато няколко позиции се добавят наведнъж).</span><span class="sxs-lookup"><span data-stu-id="fa1df-111">(for example, when several items are added at once).</span></span>

    - <span data-ttu-id="fa1df-112">Работните потоци не са проектирани да работят в реално време, така че закъснението е по проект поведение.</span><span class="sxs-lookup"><span data-stu-id="fa1df-112">Workflows are not designed to run real-time, so a delay is by-design behavior.</span></span>

   -  <span data-ttu-id="fa1df-113">Ако работният поток е сложна разтегателен обект Markup език (XMOL), компилация може да бъде бавно.</span><span class="sxs-lookup"><span data-stu-id="fa1df-113">If the Workflow is complex Extensible Object Markup Language (XMOL), compilation can be slow.</span></span> <span data-ttu-id="fa1df-114">Проверете [тази](https://support.microsoft.com/en-us/kb/3043697) статия.</span><span class="sxs-lookup"><span data-stu-id="fa1df-114">Check [this](https://support.microsoft.com/en-us/kb/3043697) article.</span></span>

    - <span data-ttu-id="fa1df-115">Трябва да опрости работния поток или го използва Microsoft SharePoint 2013 поток платформа тип редизайн.</span><span class="sxs-lookup"><span data-stu-id="fa1df-115">You should simplify the workflow or redesign it using the Microsoft SharePoint 2013 Workflow platform type.</span></span>

    - <span data-ttu-id="fa1df-116">Ако хронологията на работния поток е нараснал големи, може да искате да прочисти елементи или да създадете нов списък с хронологии.</span><span class="sxs-lookup"><span data-stu-id="fa1df-116">If your workflow history has grown large, you may want to purge the items or create a new history list.</span></span>

        <span data-ttu-id="fa1df-117">Повече информация: [Изтриване на хронологията на работния поток](https://blogs.technet.microsoft.com/marj/2015/08/07/sharepoint-2010-workflows-best-practice-purge-workflow-history-list-items/)</span><span class="sxs-lookup"><span data-stu-id="fa1df-117">More Information : [Purge Workflow History](https://blogs.technet.microsoft.com/marj/2015/08/07/sharepoint-2010-workflows-best-practice-purge-workflow-history-list-items/)</span></span>


## <a name="related-topics"></a><span data-ttu-id="fa1df-118">Сродни теми</span><span class="sxs-lookup"><span data-stu-id="fa1df-118">Related topics</span></span>
<span data-ttu-id="fa1df-119">Искате ли да опитате Microsoft поток в SharePoint Online?</span><span class="sxs-lookup"><span data-stu-id="fa1df-119">Want to try Microsoft Flow in SharePoint Online?</span></span>
- [<span data-ttu-id="fa1df-120">Създаване на поток</span><span class="sxs-lookup"><span data-stu-id="fa1df-120">Create Flow</span></span>](https://support.office.com/article/Create-a-flow-for-a-list-or-library-in-SharePoint-Online-or-OneDrive-for-Business-a9c3e03b-0654-46af-a254-20252e580d01) 
- [<span data-ttu-id="fa1df-121">SharePoint и поток</span><span class="sxs-lookup"><span data-stu-id="fa1df-121">SharePoint and Flow</span></span>](https://flow.microsoft.com/blog/sharepoint-and-flow/) 


