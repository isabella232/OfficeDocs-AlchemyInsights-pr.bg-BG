---
title: Присвояване на групи на Azure AD роля
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 01/15/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "7898"
- "9003230"
ms.openlocfilehash: feca81fe785bc45e47f6faa876230b5c7701713d
ms.sourcegitcommit: 6dc6f999e840c90694a246b90062950205679420
ms.translationtype: MT
ms.contentlocale: bg-BG
ms.lasthandoff: 01/15/2021
ms.locfileid: "49884791"
---
# <a name="assigning-groups-to-azure-ad-role"></a><span data-ttu-id="4a6c5-102">Присвояване на групи на Azure AD роля</span><span class="sxs-lookup"><span data-stu-id="4a6c5-102">Assigning groups to Azure AD role</span></span>

<span data-ttu-id="4a6c5-103">За да присвоите РЕКЛАМНА група на Azure с източник на авторитет в Azure ad към РЕКЛАМНА роля на Azure, изпълнете следните стъпки:</span><span class="sxs-lookup"><span data-stu-id="4a6c5-103">To assign an Azure AD group with source of authority in Azure AD to an Azure AD role, perform the following steps:</span></span>

1. <span data-ttu-id="4a6c5-104">Създайте нова група – за да създадете нова група:</span><span class="sxs-lookup"><span data-stu-id="4a6c5-104">Create a new group - To create a new group:</span></span>

    <span data-ttu-id="4a6c5-105">на.</span><span class="sxs-lookup"><span data-stu-id="4a6c5-105">a.</span></span> <span data-ttu-id="4a6c5-106">Влезте в центъра за администриране на Azure AD с **привилегировани администраторски** права или разрешения на **глобален администратор** .</span><span class="sxs-lookup"><span data-stu-id="4a6c5-106">Sign in to the Azure AD admin center with **privileged role administrator** or **global administrator** permissions.</span></span>
    <span data-ttu-id="4a6c5-107">b.</span><span class="sxs-lookup"><span data-stu-id="4a6c5-107">b.</span></span> <span data-ttu-id="4a6c5-108">Изберете **Azure Active Directory > групи > всички групи > нова група**.</span><span class="sxs-lookup"><span data-stu-id="4a6c5-108">Select **Azure Active Directory > Groups > All groups > New group**.</span></span>
    <span data-ttu-id="4a6c5-109">c.</span><span class="sxs-lookup"><span data-stu-id="4a6c5-109">c.</span></span> <span data-ttu-id="4a6c5-110">Създайте групата.</span><span class="sxs-lookup"><span data-stu-id="4a6c5-110">Create the group.</span></span>

2. <span data-ttu-id="4a6c5-111">Присвояване на ролята на групата по време на създаване на група или след създаването на групата.</span><span class="sxs-lookup"><span data-stu-id="4a6c5-111">Assign the role to the group either during group creation or after the group is created.</span></span>

    <span data-ttu-id="4a6c5-112">на.</span><span class="sxs-lookup"><span data-stu-id="4a6c5-112">a.</span></span> <span data-ttu-id="4a6c5-113">За да присвоите роля на групата по време на създаването на групи, можете да превключите към групата за превключване на **ролите на AZURE ad, за** да създадете групата.</span><span class="sxs-lookup"><span data-stu-id="4a6c5-113">To assign a role to the group at the time of group creation, switch on the toggle **Azure AD roles can be assigned to the group** and create the group.</span></span>
    <span data-ttu-id="4a6c5-114">b.</span><span class="sxs-lookup"><span data-stu-id="4a6c5-114">b.</span></span> <span data-ttu-id="4a6c5-115">За да присвоите роля на групата, след като е била създадена, преминете към раздела **присвоени роли** за новосъздадената група и задайте ролята на групата.</span><span class="sxs-lookup"><span data-stu-id="4a6c5-115">To assign a role to the group after it has been created, navigate to the **Assigned roles** tab for the newly created group, and assign the role to the group.</span></span>  

<span data-ttu-id="4a6c5-116">**Управление на членството в група, на която е присвоена РЕКЛАМНА роля на Azure**</span><span class="sxs-lookup"><span data-stu-id="4a6c5-116">**Manage membership of a group that is assigned to Azure AD role**</span></span>

<span data-ttu-id="4a6c5-117">За да се предотврати увеличаване на привилегиите по подразбиране, само привилегированите администратори на роли и глобалните администратори могат да променят членството в група, която е присвоена на роля.</span><span class="sxs-lookup"><span data-stu-id="4a6c5-117">To prevent elevation of privileges, by default, only privileged role administrators and global administrators can modify the membership of a group that is assigned to a role.</span></span> <span data-ttu-id="4a6c5-118">Те обаче могат да решат да начислят собственик за такава група и да делегират тази задача.</span><span class="sxs-lookup"><span data-stu-id="4a6c5-118">They can, however, choose to assign an owner for such a group and delegate this task.</span></span>

<span data-ttu-id="4a6c5-119">За повече информация относно присвояването на групи в облака на Azure AD роли вижте [Присвояване на рекламна роля на група в облака](https://docs.microsoft.com/azure/active-directory/roles/groups-concept).</span><span class="sxs-lookup"><span data-stu-id="4a6c5-119">For more details on assigning cloud groups to Azure AD roles, see [Assign a AD roles to Cloud Group](https://docs.microsoft.com/azure/active-directory/roles/groups-concept).</span></span> <span data-ttu-id="4a6c5-120">За повече информация относно ролите за отстраняване на неизправности, присвоени на групи в облака, вижте [отстраняване на неизправности при определени групи](https://docs.microsoft.com/azure/active-directory/roles/groups-faq-troubleshooting)</span><span class="sxs-lookup"><span data-stu-id="4a6c5-120">For more details on troubleshooting roles assigned to cloud groups, see [Troubleshoot roles assigned to cloud groups](https://docs.microsoft.com/azure/active-directory/roles/groups-faq-troubleshooting).</span></span>





