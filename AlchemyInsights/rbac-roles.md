---
title: 'RBAC роли '
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9003230"
- "7265"
ms.openlocfilehash: 7c4c9d1a76f395dfb2f831d555199b76c354ca57
ms.sourcegitcommit: 2e4a5153e530bf15744a52e982eeb0d99757e9d2
ms.translationtype: MT
ms.contentlocale: bg-BG
ms.lasthandoff: 12/04/2020
ms.locfileid: "49583241"
---
# <a name="rbac-rules"></a><span data-ttu-id="d1728-102">Правила за RBAC</span><span class="sxs-lookup"><span data-stu-id="d1728-102">RBAC rules</span></span>

<span data-ttu-id="d1728-103">Ако получите съобщение за грешка:</span><span class="sxs-lookup"><span data-stu-id="d1728-103">If you get the permission error:</span></span> 

- <span data-ttu-id="d1728-104">**Клиентът с ИД на обекта няма разрешение за извършване на действие по обхват (код: AuthorizationFailed)**: когато се опитате да създадете ресурс, проверете дали сте влезли в момента с потребител, на когото е присвоена роля, която има разрешение за писане на ресурса в избрания обхват.</span><span class="sxs-lookup"><span data-stu-id="d1728-104">**The client with object id does not have authorization to perform action over scope (code: AuthorizationFailed)**: when you try to create a resource, check that you are currently signed in with a user that is assigned a role that has write permission to the resource at the selected scope.</span></span> <span data-ttu-id="d1728-105">Например, за да управлявате виртуални машини в група ресурси, трябва да имате ролята на [сътрудник за виртуална машина](https://docs.microsoft.com/azure/role-based-access-control/built-in-roles?WT.mc_id=Portal-Microsoft_Azure_Support#virtual-machine-contributor) в групата ресурс (или родителен обхват).</span><span class="sxs-lookup"><span data-stu-id="d1728-105">For example, to manage virtual machines in a resource group, you should have the [Virtual Machine Contributor](https://docs.microsoft.com/azure/role-based-access-control/built-in-roles?WT.mc_id=Portal-Microsoft_Azure_Support#virtual-machine-contributor) role on the resource group (or parent scope).</span></span> <span data-ttu-id="d1728-106">За списък на разрешенията за всяка вградена роля вижте [вградени роли за ресурси на Azure](https://docs.microsoft.com/azure/role-based-access-control/built-in-roles?WT.mc_id=Portal-Microsoft_Azure_Support).</span><span class="sxs-lookup"><span data-stu-id="d1728-106">For a list of the permissions for each built-in role, see [Built-in roles for Azure resources](https://docs.microsoft.com/azure/role-based-access-control/built-in-roles?WT.mc_id=Portal-Microsoft_Azure_Support).</span></span>
- <span data-ttu-id="d1728-107">Нямате **разрешение за създаване на заявка за поддръжка**: когато се опитате да създадете или актуализирате билет за поддръжка, проверете дали сте влезли в момента с потребител, на когото е присвоена роля, която има Microsoft. support/supportTickets/write, като например [сътрудник за искане на поддръжка](https://docs.microsoft.com/azure/role-based-access-control/built-in-roles?WT.mc_id=Portal-Microsoft_Azure_Support#support-request-contributor).</span><span class="sxs-lookup"><span data-stu-id="d1728-107">**You don't have permission to create a support request**: when you try to create or update a support ticket, check that you are currently signed in with a user that is assigned a role that has the Microsoft.Support/supportTickets/write permission, such as [Support Request Contributor](https://docs.microsoft.com/azure/role-based-access-control/built-in-roles?WT.mc_id=Portal-Microsoft_Azure_Support#support-request-contributor).</span></span>
- <span data-ttu-id="d1728-108">**Не могат да се създават повече присвоявания на роли (код: RoleAssignmentLimitExceeded)**: когато се опитвате да присвоите роля, опитайте се да намалите броя на присвояванията на роли, като разпределите роля на групи вместо това.</span><span class="sxs-lookup"><span data-stu-id="d1728-108">**No more role assignments can be created (code: RoleAssignmentLimitExceeded)**: when you try to assign a role, try to reduce the number of role assignments by assigning roles to groups instead.</span></span> <span data-ttu-id="d1728-109">Azure поддържа до **2000** присвоявания на роля за абонамент.</span><span class="sxs-lookup"><span data-stu-id="d1728-109">Azure supports up to **2000** role assignments per subscription.</span></span>

<span data-ttu-id="d1728-110">За повече информация за ролите в Azure RBAC вижте [ролите в AZURE RBAC](https://docs.microsoft.com/azure/role-based-access-control/role-assignments-portal?WT.mc_id=Portal-Microsoft_Azure_Support).</span><span class="sxs-lookup"><span data-stu-id="d1728-110">For more details on Azure RBAC roles, see [Azure RBAC roles](https://docs.microsoft.com/azure/role-based-access-control/role-assignments-portal?WT.mc_id=Portal-Microsoft_Azure_Support).</span></span>
