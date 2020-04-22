---
title: Неуспешно активиране на липсващия работен поток
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: e46ae8c5-3d81-457e-8c77-f7c1cbe267c4
ms.openlocfilehash: 2598111005c219c398b63ca374e8e99348efc02c
ms.sourcegitcommit: 631cbb5f03e5371f0995e976536d24e9d13746c3
ms.translationtype: MT
ms.contentlocale: bg-BG
ms.lasthandoff: 04/22/2020
ms.locfileid: "43762090"
---
# <a name="missing-workflow-failed-to-activate"></a><span data-ttu-id="8ef73-102">Неуспешно активиране на липсващия работен поток</span><span class="sxs-lookup"><span data-stu-id="8ef73-102">Missing Workflow Failed to Activate</span></span>

<span data-ttu-id="8ef73-103">В колекция от сайтове на Microsoft SharePoint не можете да добавите глобално многократна тава работен поток (като "Одобрение – SharePoint 2010") към списък или библиотека.</span><span class="sxs-lookup"><span data-stu-id="8ef73-103">In a Microsoft SharePoint site collection, you can't add a globally reusable workflow (such as "Approval - SharePoint 2010") to a list or library.</span></span>
  
<span data-ttu-id="8ef73-104">За да разрешите този проблем, изпълнете следните стъпки:</span><span class="sxs-lookup"><span data-stu-id="8ef73-104">To resolve this issue, follow these steps:</span></span> 
  
1. <span data-ttu-id="8ef73-105">Отворете главния уеб сайт на колекцията от сайтове в SharePoint Designer 2013.</span><span class="sxs-lookup"><span data-stu-id="8ef73-105">Open the root website of the site collection in SharePoint Designer 2013.</span></span>
  
2. <span data-ttu-id="8ef73-106">Под **Обекти на сайта**изберете работни **потоци**.</span><span class="sxs-lookup"><span data-stu-id="8ef73-106">Under **Site Objects**, select **Workflows**.</span></span> 
  
3. <span data-ttu-id="8ef73-107">В раздела **Нови** **работни потоци** изберете **Повторно използваем работен поток**.</span><span class="sxs-lookup"><span data-stu-id="8ef73-107">In the **New** section of the **Workflows** ribbon, select **Reusable Workflow**.</span></span> 
  
4. <span data-ttu-id="8ef73-108">Във формуляра за създаване на работен поток за **многократна използваемост** въведете името \*\* *Repair2010* \*\*.</span><span class="sxs-lookup"><span data-stu-id="8ef73-108">On the **Create Reusable Workflow** form, enter the name \*\* *Repair2010* \*\*.</span></span> <span data-ttu-id="8ef73-109">За **тип платформа**щракнете върху Работен поток на **SharePoint 2010**и след това щракнете върху **OK**.</span><span class="sxs-lookup"><span data-stu-id="8ef73-109">For **Platform Type**, click **SharePoint 2010 Workflow**, and then click **OK**.</span></span> 
  
1. <span data-ttu-id="8ef73-110">В раздела **Запиши** на лентата **на работния поток** изберете **Публикуване**.</span><span class="sxs-lookup"><span data-stu-id="8ef73-110">In the **Save** section of the **Workflow** ribbon, select **Publish**.</span></span> 
  
2. <span data-ttu-id="8ef73-111">В раздела **управление** на лентата **на работния поток** изберете Публикуване **глобално**.</span><span class="sxs-lookup"><span data-stu-id="8ef73-111">In the **Manage** section of the **Workflow** ribbon, select **Publish Globally**.</span></span> <span data-ttu-id="8ef73-112">В диалоговия прозорец за потвърждение, който се появява, изберете **OK**.</span><span class="sxs-lookup"><span data-stu-id="8ef73-112">In the confirmation dialog box that appears, select **OK**.</span></span> 
  
3. <span data-ttu-id="8ef73-113">В уеб браузър намерете главния уеб сайт на колекцията от сайтове и след това достъп до **функциите** \> на **колекцията от сайтове**.</span><span class="sxs-lookup"><span data-stu-id="8ef73-113">In a web browser, locate the root website of the site collection, and then access **Site Settings** \> **Site Collection Features**.</span></span> <span data-ttu-id="8ef73-114">След това превключете функцията **за работни потоци:**</span><span class="sxs-lookup"><span data-stu-id="8ef73-114">Then, toggle the **Workflows** feature:</span></span> 
  
<span data-ttu-id="8ef73-115">· Ако функцията е *активирана* , щракнете върху **Дезактивиране,** след което щракнете върху **Активирай**.</span><span class="sxs-lookup"><span data-stu-id="8ef73-115">· If the feature is  *Activated*  , click **Deactivate,** and then click **Activate**.</span></span> 
  
<span data-ttu-id="8ef73-116">· Ако функцията е *дезактивирана* , щракнете върху **Активирай**.</span><span class="sxs-lookup"><span data-stu-id="8ef73-116">· If the feature is  *Deactivated*  , click **Activate**.</span></span> 
  
<span data-ttu-id="8ef73-117">За повече информация вижте следната [статия](https://go.microsoft.com/fwlink/?linkid=2047770&amp;clcid=0x409).</span><span class="sxs-lookup"><span data-stu-id="8ef73-117">For more information please refer to the following [article](https://go.microsoft.com/fwlink/?linkid=2047770&amp;clcid=0x409).</span></span>
  

