---
title: Не можете да добавите работен поток "одобрение на 2010"
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 0df65cf9-7eae-4de7-88e9-1914635c8d11
ms.openlocfilehash: aa61f1615b60d27cffad15f02f6ce5dbac1b607f
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: bg-BG
ms.lasthandoff: 09/14/2020
ms.locfileid: "47699724"
---
# <a name="unable-to-add-2010-approval-workflow"></a><span data-ttu-id="678fe-102">Не можете да добавите работен поток "одобрение на 2010"</span><span class="sxs-lookup"><span data-stu-id="678fe-102">Unable to add 2010 Approval Workflow</span></span>

<span data-ttu-id="678fe-103">В колекция от сайтове на Microsoft SharePoint не можете да добавяте глобален многократно използваем работен поток (като например "одобрение-SharePoint 2010") към списък или библиотека.</span><span class="sxs-lookup"><span data-stu-id="678fe-103">In a Microsoft SharePoint site collection, you can't add a globally reusable workflow (such as "Approval - SharePoint 2010") to a list or library.</span></span>
  
<span data-ttu-id="678fe-104">За да отстраните този проблем, изпълнете следните стъпки:</span><span class="sxs-lookup"><span data-stu-id="678fe-104">To resolve this issue, follow these steps:</span></span> 
  
1. <span data-ttu-id="678fe-105">Отворете главния уеб сайт на колекцията от сайтове в SharePoint Designer 2013.</span><span class="sxs-lookup"><span data-stu-id="678fe-105">Open the root website of the site collection in SharePoint Designer 2013.</span></span>
  
2. <span data-ttu-id="678fe-106">Под **обекти на сайт**изберете **работни потоци**.</span><span class="sxs-lookup"><span data-stu-id="678fe-106">Under **Site Objects**, select **Workflows**.</span></span> 
  
3. <span data-ttu-id="678fe-107">В **новата** секция на лентата на **работни потоци** изберете **повторно използваем работен поток**.</span><span class="sxs-lookup"><span data-stu-id="678fe-107">In the **New** section of the **Workflows** ribbon, select **Reusable Workflow**.</span></span> 
  
4. <span data-ttu-id="678fe-108">В диалоговия прозорец **Създаване на повторно използваем работен поток** въведете името \* \* *Repair2010* \* \*.</span><span class="sxs-lookup"><span data-stu-id="678fe-108">On the **Create Reusable Workflow** form, enter the name \*\* *Repair2010* \*\*.</span></span> <span data-ttu-id="678fe-109">За **тип платформа**щракнете върху **работен поток на SharePoint 2010**, след което щракнете върху **OK**.</span><span class="sxs-lookup"><span data-stu-id="678fe-109">For **Platform Type**, click **SharePoint 2010 Workflow**, and then click **OK**.</span></span> 
  
1. <span data-ttu-id="678fe-110">В секцията **Запиши** на лентата на **работния поток** щракнете върху **публикуване**.</span><span class="sxs-lookup"><span data-stu-id="678fe-110">In the **Save** section of the **Workflow** ribbon, select **Publish**.</span></span> 
  
2. <span data-ttu-id="678fe-111">В секцията **управление** на лентата на **работния поток** изберете **публикуване глобално**.</span><span class="sxs-lookup"><span data-stu-id="678fe-111">In the **Manage** section of the **Workflow** ribbon, select **Publish Globally**.</span></span> <span data-ttu-id="678fe-112">В диалоговия прозорец за потвърждение, който се появява, изберете **OK**.</span><span class="sxs-lookup"><span data-stu-id="678fe-112">In the confirmation dialog box that appears, select **OK**.</span></span> 
  
3. <span data-ttu-id="678fe-113">В уеб браузър Намерете главния уеб сайт на колекцията от сайтове и след **това Получете** достъп до \> **функциите на колекцията**от сайтове.</span><span class="sxs-lookup"><span data-stu-id="678fe-113">In a web browser, locate the root website of the site collection, and then access **Site Settings** \> **Site Collection Features**.</span></span> <span data-ttu-id="678fe-114">Включване на функцията " **работни потоци** ":</span><span class="sxs-lookup"><span data-stu-id="678fe-114">Toggle the **Workflows** feature:</span></span> 
  
<span data-ttu-id="678fe-115">· Ако функцията е  *активирана* **, щракнете върху дезактивиране** и след това върху **Активирай**.</span><span class="sxs-lookup"><span data-stu-id="678fe-115">· If the feature is  *Activated*  , click **Deactivate,** and then click **Activate**.</span></span> 
  
<span data-ttu-id="678fe-116">· Ако функцията е  *дезактивирана*  , щракнете върху **Активирай**.</span><span class="sxs-lookup"><span data-stu-id="678fe-116">· If the feature is  *Deactivated*  , click **Activate**.</span></span> 
  
<span data-ttu-id="678fe-117">За повече информация вижте [статията](https://go.microsoft.com/fwlink/?linkid=2047770&amp;clcid=0x409)по-долу.</span><span class="sxs-lookup"><span data-stu-id="678fe-117">For more information please refer to the following [article](https://go.microsoft.com/fwlink/?linkid=2047770&amp;clcid=0x409).</span></span>
  

