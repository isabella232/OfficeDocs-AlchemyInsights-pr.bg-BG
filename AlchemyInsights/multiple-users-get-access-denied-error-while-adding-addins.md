---
title: Много потребители получават грешка отказан достъп, докато добавят добавки в Outlook
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/23/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "5892"
- "6700008"
ms.openlocfilehash: 624d880c535b7d8888b676ff23c774c6d138a75a
ms.sourcegitcommit: 07e56267dedfc4cec1143072c791670cbf81186b
ms.translationtype: MT
ms.contentlocale: bg-BG
ms.lasthandoff: 07/24/2020
ms.locfileid: "45423361"
---
# <a name="multiple-users-get-access-denied-error-while-adding-add-ins-in-outlook"></a><span data-ttu-id="dcb98-102">Много потребители получават грешка отказан достъп, докато добавят добавки в Outlook</span><span class="sxs-lookup"><span data-stu-id="dcb98-102">Multiple users get Access Denied error while adding add-ins in Outlook</span></span>

<span data-ttu-id="dcb98-103">Можете да укажете кои администратори във вашата организация да имат разрешения за инсталиране и управление на добавки за Outlook.</span><span class="sxs-lookup"><span data-stu-id="dcb98-103">You can specify which administrators in your organization have permissions to install and manage add-ins for Outlook.</span></span> <span data-ttu-id="dcb98-104">Можете също да укажете кои потребители във вашата организация имат разрешение да инсталират и управляват добавки за тяхна собствена употреба.</span><span class="sxs-lookup"><span data-stu-id="dcb98-104">You can also specify which users in your organization have permission to install and manage add-ins for their own use.</span></span>

<span data-ttu-id="dcb98-105">За подробности вижте [Указване на администраторите и потребителите, които могат да инсталират и управляват добавки за Outlook](https://docs.microsoft.com/exchange/clients-and-mobile-in-exchange-online/add-ins-for-outlook/specify-who-can-install-and-manage-add-ins).</span><span class="sxs-lookup"><span data-stu-id="dcb98-105">For details, see [Specify the administrators and users who can install and manage add-ins for Outlook](https://docs.microsoft.com/exchange/clients-and-mobile-in-exchange-online/add-ins-for-outlook/specify-who-can-install-and-manage-add-ins).</span></span>

<span data-ttu-id="dcb98-106">За да проверите дали сте присвоили разрешения за потребител, заменя <Role Name> с името на ролята за проверка и изпълнете следната команда в Exchange Online PowerShell:</span><span class="sxs-lookup"><span data-stu-id="dcb98-106">To verify that you've successfully assigned permissions for a user, replace <Role Name> with the name of the role to verify, and run the following command in Exchange Online PowerShell:</span></span>

<span data-ttu-id="dcb98-107"><Role Name>1000000000000000000000000000000000000000000000000000000000000</span><span class="sxs-lookup"><span data-stu-id="dcb98-107">Get-ManagementRoleAssignment -Role "<Role Name>" -GetEffectiveUsers</span></span>

<span data-ttu-id="dcb98-108">Този пример ви показва как да проверите на кого сте присвоили разрешения за инсталиране на добавки от Office хранилището за организацията.</span><span class="sxs-lookup"><span data-stu-id="dcb98-108">This example shows you how to verify whom you've assigned permissions to install add-ins from the Office Store for the organization.</span></span>

<span data-ttu-id="dcb98-109">Powershell</span><span class="sxs-lookup"><span data-stu-id="dcb98-109">PowerShell</span></span>

<span data-ttu-id="dcb98-110">-Роля "Орг пазара приложения" -GetЕfectiveUsers</span><span class="sxs-lookup"><span data-stu-id="dcb98-110">-Role "Org Marketplace Apps" -GetEffectiveUsers</span></span>

<span data-ttu-id="dcb98-111">В резултатите Get-ManagementRoleПодписване, прегледайте записите в колоната "Ефективни потребители".</span><span class="sxs-lookup"><span data-stu-id="dcb98-111">In the results, Get-ManagementRoleAssignment, review the entries in the Effective Users column.</span></span>

<span data-ttu-id="dcb98-112">За подробна информация за синтаксиса и параметрите вижте [Получаване на управлениеRoleПодписване](https://docs.microsoft.com/powershell/module/exchange/get-managementroleassignment).</span><span class="sxs-lookup"><span data-stu-id="dcb98-112">For detailed syntax and parameter information, see [Get-ManagementRoleAssignment](https://docs.microsoft.com/powershell/module/exchange/get-managementroleassignment).</span></span>
 