---
title: Не може да се добави 2010 процес на одобрение
ms.author: pebaum
author: pebaum
ms.date: 12/3/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 0df65cf9-7eae-4de7-88e9-1914635c8d11
ms.openlocfilehash: 11ba9bf04f826b0d7465a9a81a36c327e79f4d13
ms.sourcegitcommit: 0f0186044a3597e42ad14c32ca58e7224344dcfa
ms.translationtype: MT
ms.contentlocale: bg-BG
ms.lasthandoff: 12/15/2019
ms.locfileid: "40049542"
---
# <a name="unable-to-add-2010-approval-workflow"></a><span data-ttu-id="a3436-102">Не може да се добави 2010 процес на одобрение</span><span class="sxs-lookup"><span data-stu-id="a3436-102">Unable to add 2010 Approval Workflow</span></span>

<span data-ttu-id="a3436-103">В колекцията от сайтове на Microsoft SharePoint не можете да добавите глобален поток за многократна употреба (като например "одобрение-SharePoint 2010") към списък или библиотека.</span><span class="sxs-lookup"><span data-stu-id="a3436-103">In a Microsoft SharePoint site collection, you can't add a globally reusable workflow (such as "Approval - SharePoint 2010") to a list or library.</span></span>
  
<span data-ttu-id="a3436-104">За да разрешите този проблем, изпълнете следните стъпки:</span><span class="sxs-lookup"><span data-stu-id="a3436-104">To resolve this issue, follow these steps:</span></span> 
  
1. <span data-ttu-id="a3436-105">Отворете главния уеб сайт на колекцията от сайтове в SharePoint Designer 2013.</span><span class="sxs-lookup"><span data-stu-id="a3436-105">Open the root website of the site collection in SharePoint Designer 2013.</span></span>
  
2. <span data-ttu-id="a3436-106">Под **обекти на сайта**изберете **работни потоци**.</span><span class="sxs-lookup"><span data-stu-id="a3436-106">Under **Site Objects**, select **Workflows**.</span></span> 
  
3. <span data-ttu-id="a3436-107">В **новия** раздел на лентата с **работни потоци** изберете повторно използване на **работен поток**.</span><span class="sxs-lookup"><span data-stu-id="a3436-107">In the **New** section of the **Workflows** ribbon, select **Reusable Workflow**.</span></span> 
  
4. <span data-ttu-id="a3436-108">В създаване на формуляр за **многократна употреба работен поток** въведете името \* \* *Repair2010* \* \*.</span><span class="sxs-lookup"><span data-stu-id="a3436-108">On the **Create Reusable Workflow** form, enter the name \*\* *Repair2010* \*\*.</span></span> <span data-ttu-id="a3436-109">За **тип на платформата**щракнете върху **SharePoint 2010 работен поток**и след това щракнете върху **OK**.</span><span class="sxs-lookup"><span data-stu-id="a3436-109">For **Platform Type**, click **SharePoint 2010 Workflow**, and then click **OK**.</span></span> 
  
1. <span data-ttu-id="a3436-110">В раздела **Save** на лентата на **работния поток** изберете **публикуване**.</span><span class="sxs-lookup"><span data-stu-id="a3436-110">In the **Save** section of the **Workflow** ribbon, select **Publish**.</span></span> 
  
2. <span data-ttu-id="a3436-111">В раздела **управление** на лентата на **работния поток** изберете **публикуване глобално**.</span><span class="sxs-lookup"><span data-stu-id="a3436-111">In the **Manage** section of the **Workflow** ribbon, select **Publish Globally**.</span></span> <span data-ttu-id="a3436-112">В диалоговия прозорец за потвърждение, който се появява, изберете **OK**.</span><span class="sxs-lookup"><span data-stu-id="a3436-112">In the confirmation dialog box that appears, select **OK**.</span></span> 
  
3. <span data-ttu-id="a3436-113">В уеб браузър Намерете главния уеб сайт на колекцията от сайтове и след това Access **Настройки** \> на сайта **колекция функции**.</span><span class="sxs-lookup"><span data-stu-id="a3436-113">In a web browser, locate the root website of the site collection, and then access **Site Settings** \> **Site Collection Features**.</span></span> <span data-ttu-id="a3436-114">Превключване на функцията за **работни потоци** :</span><span class="sxs-lookup"><span data-stu-id="a3436-114">Toggle the **Workflows** feature:</span></span> 
  
<span data-ttu-id="a3436-115">· Ако функцията е *активирана* , щракнете върху **Деактивирай** и след това щракнете върху **Активирай**.</span><span class="sxs-lookup"><span data-stu-id="a3436-115">· If the feature is  *Activated*  , click **Deactivate,** and then click **Activate**.</span></span> 
  
<span data-ttu-id="a3436-116">· Ако функцията е *деактивирана* , щракнете върху **активиране**.</span><span class="sxs-lookup"><span data-stu-id="a3436-116">· If the feature is  *Deactivated*  , click **Activate**.</span></span> 
  
<span data-ttu-id="a3436-117">За повече информация, моля, вижте следната [статия](https://go.microsoft.com/fwlink/?linkid=2047770&amp;clcid=0x409).</span><span class="sxs-lookup"><span data-stu-id="a3436-117">For more information please refer to the following [article](https://go.microsoft.com/fwlink/?linkid=2047770&amp;clcid=0x409).</span></span>
  

