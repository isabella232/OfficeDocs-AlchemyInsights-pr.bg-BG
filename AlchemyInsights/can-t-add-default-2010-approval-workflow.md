---
title: Не може да добави по подразбиране работният поток за одобрение на 2010
ms.author: kirks
author: Techwriter40
ms.date: 12/3/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.assetid: 2060c9a1-e714-4d93-925e-629c82c35986
ms.openlocfilehash: 758b0339b842478f9609eb716b5b4ddab6579c80
ms.sourcegitcommit: d6ea5e9458a2b8ceaab3ac4bd483e1130b9a398a
ms.translationtype: MT
ms.contentlocale: bg-BG
ms.lasthandoff: 01/15/2019
ms.locfileid: "28275531"
---
# <a name="cant-add-default-2010-approval-workflow"></a><span data-ttu-id="58884-102">Не може да добави по подразбиране работният поток за одобрение на 2010</span><span class="sxs-lookup"><span data-stu-id="58884-102">Can't add default 2010 Approval Workflow</span></span>

<span data-ttu-id="58884-103">В колекция сайтове Microsoft SharePoint не можете да добавяте глобално повторно използваем работен поток (като "одобрение - SharePoint 2010") към списък или библиотека.</span><span class="sxs-lookup"><span data-stu-id="58884-103">In a Microsoft SharePoint site collection, you can't add a globally reusable workflow (such as "Approval - SharePoint 2010") to a list or library.</span></span>
  
<span data-ttu-id="58884-104">За да разрешите този проблем, изпълнете следните стъпки:</span><span class="sxs-lookup"><span data-stu-id="58884-104">To resolve this issue, follow these steps:</span></span> 
  
1. <span data-ttu-id="58884-105">Отваряне на главната интернет страницата на колекцията в SharePoint Designer 2013.</span><span class="sxs-lookup"><span data-stu-id="58884-105">Open the root website of the site collection in SharePoint Designer 2013.</span></span>
  
2. <span data-ttu-id="58884-106">Под **Сайт обекти**изберете **работни потоци**.</span><span class="sxs-lookup"><span data-stu-id="58884-106">Under **Site Objects**, select **Workflows**.</span></span> 
  
3. <span data-ttu-id="58884-107">В **новия** раздел на лентата на **работни потоци** изберете **Повторно използваемо поток**.</span><span class="sxs-lookup"><span data-stu-id="58884-107">In the **New** section of the **Workflows** ribbon, select **Reusable Workflow**.</span></span> 
  
4. <span data-ttu-id="58884-p101">Върху формуляра за **Създаване на повторно използваемо работен поток** , въведете името на \* \*\*Repair2010\*\*\*. За **Платформа тип**изберете **SharePoint 2010 поток**и след това изберете **OK**.</span><span class="sxs-lookup"><span data-stu-id="58884-p101">On the **Create Reusable Workflow** form, enter the name  \* **Repair2010**\* . For **Platform Type**, select **SharePoint 2010 Workflow**, and then select **OK**.</span></span> 
  
5. <span data-ttu-id="58884-110">В раздела **Запиши** на лентата на **работния поток** изберете **публикуване**.</span><span class="sxs-lookup"><span data-stu-id="58884-110">In the **Save** section of the **Workflow** ribbon, select **Publish**.</span></span> 
  
6. <span data-ttu-id="58884-p102">В раздела **управление** на **работния поток** лентата изберете **Публикуване в световен мащаб**. В диалоговия прозорец за потвърждение, който се появява изберете **OK**.</span><span class="sxs-lookup"><span data-stu-id="58884-p102">In the **Manage** section of the **Workflow** ribbon, select **Publish Globally**. In the confirmation dialog box that appears, select **OK**.</span></span> 
  
7. <span data-ttu-id="58884-p103">В уеб браузър, намерете корена сайта на колекцията със сайтове и след това достъп до **Настройки на сайта** \> **Функции на колекцията сайтове**. След това превключване функцията на **работни потоци** :</span><span class="sxs-lookup"><span data-stu-id="58884-p103">In a web browser, locate the root website of the site collection, and then access **Site Settings** \> **Site Collection Features**. Then, toggle the **Workflows** feature:</span></span> 
  
<span data-ttu-id="58884-115">· Ако функцията е *активен* , щракнете върху **Дезактивирай** и след това щракнете върху **активиране**.</span><span class="sxs-lookup"><span data-stu-id="58884-115">· If the feature is  *Activated*  , click **Deactivate,** and then click **Activate**.</span></span> 
  
<span data-ttu-id="58884-116">· Ако функцията е *Deactivated* , щракнете върху **Активирай**.</span><span class="sxs-lookup"><span data-stu-id="58884-116">· If the feature is  *Deactivated*  , click **Activate**.</span></span> 
  
<span data-ttu-id="58884-117">За повече информация се обърнете към следната [статия](https://go.microsoft.com/fwlink/?linkid=2047770&amp;clcid=0x409).</span><span class="sxs-lookup"><span data-stu-id="58884-117">For more information please refer to the following [article](https://go.microsoft.com/fwlink/?linkid=2047770&amp;clcid=0x409).</span></span>
  

