---
title: Липсва работният поток не успя да активира
ms.author: kirks
author: Techwriter40
ms.date: 12/3/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: e46ae8c5-3d81-457e-8c77-f7c1cbe267c4
ms.openlocfilehash: ce088227a3206fa05b99331fdb022fbe4886203f
ms.sourcegitcommit: 9d78905c512192ffc4675468abd2efc5f2e4baf4
ms.translationtype: MT
ms.contentlocale: bg-BG
ms.lasthandoff: 04/23/2019
ms.locfileid: "32418422"
---
# <a name="missing-workflow-failed-to-activate"></a><span data-ttu-id="3baea-102">Липсва работният поток не успя да активира</span><span class="sxs-lookup"><span data-stu-id="3baea-102">Missing Workflow Failed to Activate</span></span>

<span data-ttu-id="3baea-103">В колекция сайтове Microsoft SharePoint не можете да добавяте глобално повторно използваем работен поток (като "одобрение - SharePoint 2010") към списък или библиотека.</span><span class="sxs-lookup"><span data-stu-id="3baea-103">In a Microsoft SharePoint site collection, you can't add a globally reusable workflow (such as "Approval - SharePoint 2010") to a list or library.</span></span>
  
<span data-ttu-id="3baea-104">За да разрешите този проблем, изпълнете следните стъпки:</span><span class="sxs-lookup"><span data-stu-id="3baea-104">To resolve this issue, follow these steps:</span></span> 
  
1. <span data-ttu-id="3baea-105">Отваряне на главната интернет страницата на колекцията в SharePoint Designer 2013.</span><span class="sxs-lookup"><span data-stu-id="3baea-105">Open the root website of the site collection in SharePoint Designer 2013.</span></span>
  
2. <span data-ttu-id="3baea-106">Под **Сайт обекти**изберете **работни потоци**.</span><span class="sxs-lookup"><span data-stu-id="3baea-106">Under **Site Objects**, select **Workflows**.</span></span> 
  
3. <span data-ttu-id="3baea-107">В **новия** раздел на лентата на **работни потоци** изберете **Повторно използваемо поток**.</span><span class="sxs-lookup"><span data-stu-id="3baea-107">In the **New** section of the **Workflows** ribbon, select **Reusable Workflow**.</span></span> 
  
4. <span data-ttu-id="3baea-108">Върху формуляра за **Създаване на повторно използваемо работен поток** , въведете името на \*\* *Repair2010* \*\*.</span><span class="sxs-lookup"><span data-stu-id="3baea-108">On the **Create Reusable Workflow** form, enter the name \*\* *Repair2010* \*\*.</span></span> <span data-ttu-id="3baea-109">За **Платформа тип**щракнете върху **SharePoint 2010 поток**и след това щракнете върху **OK**.</span><span class="sxs-lookup"><span data-stu-id="3baea-109">For **Platform Type**, click **SharePoint 2010 Workflow**, and then click **OK**.</span></span> 
  
1. <span data-ttu-id="3baea-110">В раздела **Запиши** на лентата на **работния поток** изберете **публикуване**.</span><span class="sxs-lookup"><span data-stu-id="3baea-110">In the **Save** section of the **Workflow** ribbon, select **Publish**.</span></span> 
  
2. <span data-ttu-id="3baea-111">В раздела **управление** на **работния поток** лентата изберете **Публикуване в световен мащаб**.</span><span class="sxs-lookup"><span data-stu-id="3baea-111">In the **Manage** section of the **Workflow** ribbon, select **Publish Globally**.</span></span> <span data-ttu-id="3baea-112">В диалоговия прозорец за потвърждение, който се появява изберете **OK**.</span><span class="sxs-lookup"><span data-stu-id="3baea-112">In the confirmation dialog box that appears, select **OK**.</span></span> 
  
3. <span data-ttu-id="3baea-113">В уеб браузър, намерете корена сайта на колекцията със сайтове и след това достъп до **Настройки на сайта** \> **Функции на колекцията сайтове**.</span><span class="sxs-lookup"><span data-stu-id="3baea-113">In a web browser, locate the root website of the site collection, and then access **Site Settings** \> **Site Collection Features**.</span></span> <span data-ttu-id="3baea-114">След това превключване функцията на **работни потоци** :</span><span class="sxs-lookup"><span data-stu-id="3baea-114">Then, toggle the **Workflows** feature:</span></span> 
  
<span data-ttu-id="3baea-115">· Ако функцията е *активен* , щракнете върху **Дезактивирай** и след това щракнете върху **активиране**.</span><span class="sxs-lookup"><span data-stu-id="3baea-115">· If the feature is  *Activated*  , click **Deactivate,** and then click **Activate**.</span></span> 
  
<span data-ttu-id="3baea-116">· Ако функцията е *Deactivated* , щракнете върху **Активирай**.</span><span class="sxs-lookup"><span data-stu-id="3baea-116">· If the feature is  *Deactivated*  , click **Activate**.</span></span> 
  
<span data-ttu-id="3baea-117">За повече информация се обърнете към следната [статия](https://go.microsoft.com/fwlink/?linkid=2047770&amp;clcid=0x409).</span><span class="sxs-lookup"><span data-stu-id="3baea-117">For more information please refer to the following [article](https://go.microsoft.com/fwlink/?linkid=2047770&amp;clcid=0x409).</span></span>
  

