---
title: Един потребител не вижда добавки в Outlook
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/16/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom: ''
ms.openlocfilehash: 1f547c3f593b3256bd44f518aacbc36ed1c4c848
ms.sourcegitcommit: a05276bd623466ad211e1f8d9f0c616672dd3640
ms.translationtype: MT
ms.contentlocale: bg-BG
ms.lasthandoff: 07/16/2020
ms.locfileid: "45197735"
---
# <a name="single-user-not-seeing-add-ins-in-outlook"></a><span data-ttu-id="ce991-102">Един потребител не вижда добавки в Outlook</span><span class="sxs-lookup"><span data-stu-id="ce991-102">Single user not seeing add-ins in Outlook</span></span>

<span data-ttu-id="ce991-103">Потребителят може да е част от роля, която няма правилния параметър AppsForOfficeEnabled.</span><span class="sxs-lookup"><span data-stu-id="ce991-103">The user might be part of a role that doesn’t have the correct AppsForOfficeEnabled parameter.</span></span> <span data-ttu-id="ce991-104">Изпълнете тази команда, за да разберете дали правилната роля е свързана с потребителя:</span><span class="sxs-lookup"><span data-stu-id="ce991-104">Run this cmdlet to find out if the correct role is associated with the user:</span></span>

<span data-ttu-id="ce991-105">User@domain.com за управление на $false | Формат-таблица -автоматична роля,Ролевиези име,Ролевиезитип</span><span class="sxs-lookup"><span data-stu-id="ce991-105">Get-ManagementRoleAssignment -RoleAssignee user@domain.com -Delegating $false | Format-Table -Auto Role,RoleAssigneeName,RoleAssigneeType</span></span>

<span data-ttu-id="ce991-106">За повече информация вижте [Указване на администраторите и потребителите, които могат да инсталират и управляват добавки за Outlook](https://docs.microsoft.com/exchange/clients-and-mobile-in-exchange-online/add-ins-for-outlook/specify-who-can-install-and-manage-add-ins).</span><span class="sxs-lookup"><span data-stu-id="ce991-106">For more info, see [Specify the administrators and users who can install and manage add-ins for Outlook](https://docs.microsoft.com/exchange/clients-and-mobile-in-exchange-online/add-ins-for-outlook/specify-who-can-install-and-manage-add-ins).</span></span>
