---
title: Липсващ работен поток Неуспешно активиране
ms.author: pebaum
author: Techwriter40
ms.date: 12/3/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: e46ae8c5-3d81-457e-8c77-f7c1cbe267c4
ms.openlocfilehash: f03d7e1441465050c4b0608f4100f217b183d2e2
ms.sourcegitcommit: b43f77221f47b50c41197a448a9c26c423ce1ad5
ms.translationtype: MT
ms.contentlocale: bg-BG
ms.lasthandoff: 11/15/2019
ms.locfileid: "36753785"
---
# <a name="missing-workflow-failed-to-activate"></a><span data-ttu-id="b1f9b-102">Липсващ работен поток Неуспешно активиране</span><span class="sxs-lookup"><span data-stu-id="b1f9b-102">Missing Workflow Failed to Activate</span></span>

<span data-ttu-id="b1f9b-103">В колекцията от сайтове на Microsoft SharePoint не можете да добавите глобален поток за многократна употреба (като например "одобрение-SharePoint 2010") към списък или библиотека.</span><span class="sxs-lookup"><span data-stu-id="b1f9b-103">In a Microsoft SharePoint site collection, you can't add a globally reusable workflow (such as "Approval - SharePoint 2010") to a list or library.</span></span>
  
<span data-ttu-id="b1f9b-104">За да разрешите този проблем, изпълнете следните стъпки:</span><span class="sxs-lookup"><span data-stu-id="b1f9b-104">To resolve this issue, follow these steps:</span></span> 
  
1. <span data-ttu-id="b1f9b-105">Отворете главния уеб сайт на колекцията от сайтове в SharePoint Designer 2013.</span><span class="sxs-lookup"><span data-stu-id="b1f9b-105">Open the root website of the site collection in SharePoint Designer 2013.</span></span>
  
2. <span data-ttu-id="b1f9b-106">Под **обекти на сайта**изберете **работни потоци**.</span><span class="sxs-lookup"><span data-stu-id="b1f9b-106">Under **Site Objects**, select **Workflows**.</span></span> 
  
3. <span data-ttu-id="b1f9b-107">В **новия** раздел на лентата с **работни потоци** изберете повторно използване на **работен поток**.</span><span class="sxs-lookup"><span data-stu-id="b1f9b-107">In the **New** section of the **Workflows** ribbon, select **Reusable Workflow**.</span></span> 
  
4. <span data-ttu-id="b1f9b-108">В създаване на формуляр за **многократна употреба работен поток** въведете името \* \* *Repair2010* \* \*.</span><span class="sxs-lookup"><span data-stu-id="b1f9b-108">On the **Create Reusable Workflow** form, enter the name \*\* *Repair2010* \*\*.</span></span> <span data-ttu-id="b1f9b-109">За **тип на платформата**щракнете върху **SharePoint 2010 работен поток**и след това щракнете върху **OK**.</span><span class="sxs-lookup"><span data-stu-id="b1f9b-109">For **Platform Type**, click **SharePoint 2010 Workflow**, and then click **OK**.</span></span> 
  
1. <span data-ttu-id="b1f9b-110">В раздела **Save** на лентата на **работния поток** изберете **публикуване**.</span><span class="sxs-lookup"><span data-stu-id="b1f9b-110">In the **Save** section of the **Workflow** ribbon, select **Publish**.</span></span> 
  
2. <span data-ttu-id="b1f9b-111">В раздела **управление** на лентата на **работния поток** изберете **публикуване глобално**.</span><span class="sxs-lookup"><span data-stu-id="b1f9b-111">In the **Manage** section of the **Workflow** ribbon, select **Publish Globally**.</span></span> <span data-ttu-id="b1f9b-112">В диалоговия прозорец за потвърждение, който се появява, изберете **OK**.</span><span class="sxs-lookup"><span data-stu-id="b1f9b-112">In the confirmation dialog box that appears, select **OK**.</span></span> 
  
3. <span data-ttu-id="b1f9b-113">В уеб браузър Намерете главния уеб сайт на колекцията от сайтове и след това Access **Настройки** \> на сайта **колекция функции**.</span><span class="sxs-lookup"><span data-stu-id="b1f9b-113">In a web browser, locate the root website of the site collection, and then access **Site Settings** \> **Site Collection Features**.</span></span> <span data-ttu-id="b1f9b-114">След това превключете функцията за **работни потоци** :</span><span class="sxs-lookup"><span data-stu-id="b1f9b-114">Then, toggle the **Workflows** feature:</span></span> 
  
<span data-ttu-id="b1f9b-115">· Ако функцията е *активирана* , щракнете върху **Деактивирай** и след това щракнете върху **Активирай**.</span><span class="sxs-lookup"><span data-stu-id="b1f9b-115">· If the feature is  *Activated*  , click **Deactivate,** and then click **Activate**.</span></span> 
  
<span data-ttu-id="b1f9b-116">· Ако функцията е *деактивирана* , щракнете върху **активиране**.</span><span class="sxs-lookup"><span data-stu-id="b1f9b-116">· If the feature is  *Deactivated*  , click **Activate**.</span></span> 
  
<span data-ttu-id="b1f9b-117">За повече информация, моля, вижте следната [статия](https://go.microsoft.com/fwlink/?linkid=2047770&amp;clcid=0x409).</span><span class="sxs-lookup"><span data-stu-id="b1f9b-117">For more information please refer to the following [article](https://go.microsoft.com/fwlink/?linkid=2047770&amp;clcid=0x409).</span></span>
  

