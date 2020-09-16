---
title: Грешка "много потребители получавате отказан достъп" при добавяне на добавки в Outlook
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/23/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "5892"
- "6700008"
ms.openlocfilehash: 611a4df473458abc0ab0c65442f2141763f7b868
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: bg-BG
ms.lasthandoff: 09/14/2020
ms.locfileid: "47724352"
---
# <a name="multiple-users-get-access-denied-error-while-adding-add-ins-in-outlook"></a><span data-ttu-id="e8806-102">Грешка "много потребители получавате отказан достъп" при добавяне на добавки в Outlook</span><span class="sxs-lookup"><span data-stu-id="e8806-102">Multiple users get Access Denied error while adding add-ins in Outlook</span></span>

<span data-ttu-id="e8806-103">Можете да зададете кои администратори във вашата организация да имат разрешения за инсталиране и управление на добавки за Outlook.</span><span class="sxs-lookup"><span data-stu-id="e8806-103">You can specify which administrators in your organization have permissions to install and manage add-ins for Outlook.</span></span> <span data-ttu-id="e8806-104">Можете също да укажете кои потребители във вашата организация да имат разрешение за инсталиране и управление на добавки за тяхна собствена употреба.</span><span class="sxs-lookup"><span data-stu-id="e8806-104">You can also specify which users in your organization have permission to install and manage add-ins for their own use.</span></span>

<span data-ttu-id="e8806-105">За подробности вижте [Задаване на администраторите и потребителите, които могат да инсталират и управляват добавки за Outlook](https://docs.microsoft.com/exchange/clients-and-mobile-in-exchange-online/add-ins-for-outlook/specify-who-can-install-and-manage-add-ins).</span><span class="sxs-lookup"><span data-stu-id="e8806-105">For details, see [Specify the administrators and users who can install and manage add-ins for Outlook](https://docs.microsoft.com/exchange/clients-and-mobile-in-exchange-online/add-ins-for-outlook/specify-who-can-install-and-manage-add-ins).</span></span>

<span data-ttu-id="e8806-106">За да се уверите, че сте задали успешно разрешения за потребител, заменете <Role Name> с името на ролята за проверка и изпълнете следната команда в PowerShell на Exchange Online:</span><span class="sxs-lookup"><span data-stu-id="e8806-106">To verify that you've successfully assigned permissions for a user, replace <Role Name> with the name of the role to verify, and run the following command in Exchange Online PowerShell:</span></span>

<span data-ttu-id="e8806-107">Get-ManagementRoleAssignment-роля " <Role Name> "-GetEffectiveUsers</span><span class="sxs-lookup"><span data-stu-id="e8806-107">Get-ManagementRoleAssignment -Role "<Role Name>" -GetEffectiveUsers</span></span>

<span data-ttu-id="e8806-108">Този пример ви показва как да проверите кого сте задали разрешения за инсталиране на добавки от Office магазина за организацията.</span><span class="sxs-lookup"><span data-stu-id="e8806-108">This example shows you how to verify whom you've assigned permissions to install add-ins from the Office Store for the organization.</span></span>

<span data-ttu-id="e8806-109">PowerShell</span><span class="sxs-lookup"><span data-stu-id="e8806-109">PowerShell</span></span>

<span data-ttu-id="e8806-110">-Роля "приложения за пазара на org" – GetEffectiveUsers</span><span class="sxs-lookup"><span data-stu-id="e8806-110">-Role "Org Marketplace Apps" -GetEffectiveUsers</span></span>

<span data-ttu-id="e8806-111">В резултатите Получете ManagementRoleAssignment, прегледайте записите в колоната за ефективни потребители.</span><span class="sxs-lookup"><span data-stu-id="e8806-111">In the results, Get-ManagementRoleAssignment, review the entries in the Effective Users column.</span></span>

<span data-ttu-id="e8806-112">За подробен синтаксис и информация за параметрите вижте [get-ManagementRoleAssignment](https://docs.microsoft.com/powershell/module/exchange/get-managementroleassignment).</span><span class="sxs-lookup"><span data-stu-id="e8806-112">For detailed syntax and parameter information, see [Get-ManagementRoleAssignment](https://docs.microsoft.com/powershell/module/exchange/get-managementroleassignment).</span></span>
 