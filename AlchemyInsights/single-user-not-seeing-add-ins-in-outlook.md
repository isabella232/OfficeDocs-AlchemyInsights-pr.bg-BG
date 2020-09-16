---
title: Отделен потребител, който не вижда добавки в Outlook
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/16/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom: ''
ms.openlocfilehash: 8c99b443a2d83f3ac24362d63cd6363a66a81393
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: bg-BG
ms.lasthandoff: 09/14/2020
ms.locfileid: "47719654"
---
# <a name="single-user-not-seeing-add-ins-in-outlook"></a><span data-ttu-id="f3530-102">Отделен потребител, който не вижда добавки в Outlook</span><span class="sxs-lookup"><span data-stu-id="f3530-102">Single user not seeing add-ins in Outlook</span></span>

<span data-ttu-id="f3530-103">Потребителят може да бъде част от роля, която не съдържа правилния параметър на AppsForOfficeEnabled.</span><span class="sxs-lookup"><span data-stu-id="f3530-103">The user might be part of a role that doesn’t have the correct AppsForOfficeEnabled parameter.</span></span> <span data-ttu-id="f3530-104">Изпълнете тази кратка команда, за да разберете дали правилната роля е свързана с потребителя:</span><span class="sxs-lookup"><span data-stu-id="f3530-104">Run this cmdlet to find out if the correct role is associated with the user:</span></span>

<span data-ttu-id="f3530-105">Get-ManagementRoleAssignment-RoleAssignee user@domain.com-делегиране на $false | Формат-таблица – автоматична роля, RoleAssigneeName, RoleAssigneeType</span><span class="sxs-lookup"><span data-stu-id="f3530-105">Get-ManagementRoleAssignment -RoleAssignee user@domain.com -Delegating $false | Format-Table -Auto Role,RoleAssigneeName,RoleAssigneeType</span></span>

<span data-ttu-id="f3530-106">За повече информация вижте [Задаване на администраторите и потребителите, които могат да инсталират и управляват добавки за Outlook](https://docs.microsoft.com/exchange/clients-and-mobile-in-exchange-online/add-ins-for-outlook/specify-who-can-install-and-manage-add-ins).</span><span class="sxs-lookup"><span data-stu-id="f3530-106">For more info, see [Specify the administrators and users who can install and manage add-ins for Outlook](https://docs.microsoft.com/exchange/clients-and-mobile-in-exchange-online/add-ins-for-outlook/specify-who-can-install-and-manage-add-ins).</span></span>
