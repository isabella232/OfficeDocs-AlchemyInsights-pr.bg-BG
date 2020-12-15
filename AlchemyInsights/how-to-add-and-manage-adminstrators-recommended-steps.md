---
title: Как да добавяте и управлявате adminstrators-Препоръчителни стъпки
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 12/07/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004114"
- "7194"
ms.openlocfilehash: 142bf1474ac0e0eac5cecb9dddd35e28b6b6631e
ms.sourcegitcommit: 94036315916fbc79dca2a692c2e9bc1139dd28f6
ms.translationtype: MT
ms.contentlocale: bg-BG
ms.lasthandoff: 12/08/2020
ms.locfileid: "49676836"
---
# <a name="how-to-add-and-manage-adminstrators---recommended-steps"></a><span data-ttu-id="9452f-102">Как да добавяте и управлявате adminstrators-Препоръчителни стъпки</span><span class="sxs-lookup"><span data-stu-id="9452f-102">How to add and manage adminstrators - recommended steps</span></span>

<span data-ttu-id="9452f-103">**Редактиране на администратора на абонамента или съ-администратора**</span><span class="sxs-lookup"><span data-stu-id="9452f-103">**Edit the Subscription Administrator or Co-administrator**</span></span>

- <span data-ttu-id="9452f-104">Администраторът на акаунта може да редактира и двете роли, като има предвид, че администраторът на абонамента може само да променя съвместно администраторите в [портала на Azure](https://ms.portal.azure.com/#home).</span><span class="sxs-lookup"><span data-stu-id="9452f-104">The Account Administrator can edit both roles whereas the Subscription Administrator can only change Co-administrators in the [Azure portal](https://ms.portal.azure.com/#home).</span></span>
- [<span data-ttu-id="9452f-105">Добавяне или промяна на администратори на абонаменти за Azure</span><span class="sxs-lookup"><span data-stu-id="9452f-105">Add or change Azure subscription administrators</span></span>](https://docs.microsoft.com/azure/cost-management-billing/manage/add-change-subscription-administrator)

<span data-ttu-id="9452f-106">**Актуализиране на администратора на абонамента или Co-Administrator за вътрешните абонаменти (ИЗЛЪЧВАния)**</span><span class="sxs-lookup"><span data-stu-id="9452f-106">**Update the Subscription Administrator or Co-Administrator for Internal (AIRS) Subscriptions**</span></span>

<span data-ttu-id="9452f-107">Администраторът на услугата или съадминистраторът могат да използват самостоятелно това действие с помощта на следните стъпки:</span><span class="sxs-lookup"><span data-stu-id="9452f-107">The Service Administrator or the Co-administrator can self-serve this action by using the following steps:</span></span>

1. <span data-ttu-id="9452f-108">Влезте в портала на [Azure](https://ms.portal.azure.com/#home) и щракнете върху **управление на разходите + плащане** в левия нож.</span><span class="sxs-lookup"><span data-stu-id="9452f-108">Log in to the [Azure portal](https://ms.portal.azure.com/#home) and click **Cost Management + Billing** in the left blade.</span></span>
2. <span data-ttu-id="9452f-109">Щракнете върху договорения ред с абонамента си.</span><span class="sxs-lookup"><span data-stu-id="9452f-109">Click on the line item with your subscription.</span></span> <span data-ttu-id="9452f-110">Това отваря общия преглед на вашия абонамент.</span><span class="sxs-lookup"><span data-stu-id="9452f-110">This opens the Overview for your subscription.</span></span>
3. <span data-ttu-id="9452f-111">В Блейд за **абонамента** щракнете върху **свойства**.</span><span class="sxs-lookup"><span data-stu-id="9452f-111">On the **Subscription** blade, click **Properties**.</span></span> 
4. <span data-ttu-id="9452f-112">Щракнете върху бутона **администратор на услуга** .</span><span class="sxs-lookup"><span data-stu-id="9452f-112">Click the **Service Admin** button.</span></span>
5. <span data-ttu-id="9452f-113">Въведете имейла на потребителя, когото искате да зададете като администратор на услугата, и щракнете върху **OK**.</span><span class="sxs-lookup"><span data-stu-id="9452f-113">Enter the email of the user whom you want to set as a Service Administrator and click **OK**.</span></span>

<span data-ttu-id="9452f-114">**Добавяне/промяна/премахване на съвместно управление**</span><span class="sxs-lookup"><span data-stu-id="9452f-114">**Add/Change/Remove Co-administrator**</span></span>

1. <span data-ttu-id="9452f-115">Влезте в портала на [Azure](https://ms.portal.azure.com/#home) като администратор на услуга.</span><span class="sxs-lookup"><span data-stu-id="9452f-115">Log in to the [Azure portal](https://ms.portal.azure.com/#home) as a Service Administrator.</span></span>
2. <span data-ttu-id="9452f-116">Отваряне [на абонаменти](https://ms.portal.azure.com/#blade/Microsoft_Azure_Billing/SubscriptionsBlade) и избиране на план.</span><span class="sxs-lookup"><span data-stu-id="9452f-116">Open [Subscriptions](https://ms.portal.azure.com/#blade/Microsoft_Azure_Billing/SubscriptionsBlade) and select a subscription.</span></span> <span data-ttu-id="9452f-117">(CO-adminstrators може да бъде присвояван само в обхвата на абонамента.)</span><span class="sxs-lookup"><span data-stu-id="9452f-117">(Co-adminstrators can only be assigned at the subscription scope.)</span></span>
3. <span data-ttu-id="9452f-118">Навигиране до " **управление на достъпа" (IAM)**  >  **Classic администраторите**  >  **добавят**  >  **Добави съадминистратор** , за да отворите екрана **Добавяне на съвместно администриране** (ако опцията Добавяне на съвместно администриране е забранена, това означава, че нямате разрешения).</span><span class="sxs-lookup"><span data-stu-id="9452f-118">Navigate to **Access control (IAM)** > **Classic administrators** > **Add** > **Add co-administrator** to open the **Add co-admin** pane (If the Add co-administrator option is disabled, it denotes that you do not have permissions).</span></span>
4. <span data-ttu-id="9452f-119">Изберете потребителя, когото искате да добавите, и щракнете върху **Добави**.</span><span class="sxs-lookup"><span data-stu-id="9452f-119">Select the user whom you want to add and click **Add**.</span></span>

<span data-ttu-id="9452f-120">**Научете повече:**</span><span class="sxs-lookup"><span data-stu-id="9452f-120">**Learn more:**</span></span>
- [<span data-ttu-id="9452f-121">Добавяне на съ-администратор</span><span class="sxs-lookup"><span data-stu-id="9452f-121">Add a Co-Administrator</span></span>](https://docs.microsoft.com/azure/role-based-access-control/classic-administrators)
- [<span data-ttu-id="9452f-122">Премахване на съ-администратор</span><span class="sxs-lookup"><span data-stu-id="9452f-122">Remove a co-administrator</span></span>](https://docs.microsoft.com/azure/role-based-access-control/classic-administrators)
- [<span data-ttu-id="9452f-123">Промяна на администратора на услугата</span><span class="sxs-lookup"><span data-stu-id="9452f-123">Change the Service Administrator</span></span>](https://docs.microsoft.com/azure/role-based-access-control/classic-administrators)
- [<span data-ttu-id="9452f-124">Преглед на администратора на акаунт</span><span class="sxs-lookup"><span data-stu-id="9452f-124">View the Account Administrator</span></span>](https://docs.microsoft.com/azure/role-based-access-control/classic-administrators)
- [<span data-ttu-id="9452f-125">Управление на достъпа чрез RBAC и Azure Portal</span><span class="sxs-lookup"><span data-stu-id="9452f-125">Manage access using RBAC and Azure portal</span></span>](https://docs.microsoft.com/azure/role-based-access-control/role-assignments-portal)

<span data-ttu-id="9452f-126">**Добавяне/изтриване на потребители, използващи Azure Active Directory (AD)**</span><span class="sxs-lookup"><span data-stu-id="9452f-126">**Add/delete users using Azure Active Directory (AD)**</span></span>

<span data-ttu-id="9452f-127">Можете да добавяте нови потребители или да изтривате съществуващи потребители от вашата организация на Azure Active Directory (Azure AD):</span><span class="sxs-lookup"><span data-stu-id="9452f-127">You can add new users or delete existing users from your Azure Active Directory (Azure AD) organization:</span></span>

1. <span data-ttu-id="9452f-128">За да добавите нов потребител, влезте в портала на [Azure](https://ms.portal.azure.com/#home) като администратор на потребителя за организацията.</span><span class="sxs-lookup"><span data-stu-id="9452f-128">To add a new user, log in to the [Azure portal](https://ms.portal.azure.com/#home) as a User-administrator for the organization.</span></span>
2. <span data-ttu-id="9452f-129">Изберете **Azure Active Directory**, изберете **потребители** и след това щракнете върху **нов потребител**.</span><span class="sxs-lookup"><span data-stu-id="9452f-129">Select **Azure Active Directory**, select **Users** and then click **New user**.</span></span>
3. <span data-ttu-id="9452f-130">На страницата **User** попълнете необходимата информация.</span><span class="sxs-lookup"><span data-stu-id="9452f-130">On the **User** page, fill out the required information.</span></span> <span data-ttu-id="9452f-131">Щракнете върху **Създай**.</span><span class="sxs-lookup"><span data-stu-id="9452f-131">Click **Create**.</span></span> <span data-ttu-id="9452f-132">Потребителят се създава и добавя към вашия клиент на Azure AD.</span><span class="sxs-lookup"><span data-stu-id="9452f-132">The user is created and added to your Azure AD tenant.</span></span>

<span data-ttu-id="9452f-133">**Научете повече**:</span><span class="sxs-lookup"><span data-stu-id="9452f-133">**Learn more**:</span></span>

- [<span data-ttu-id="9452f-134">Добавяне на нов потребител</span><span class="sxs-lookup"><span data-stu-id="9452f-134">Add a new user</span></span>](https://docs.microsoft.com/azure/active-directory/fundamentals/add-users-azure-active-directory)
- [<span data-ttu-id="9452f-135">Изтриване на потребител</span><span class="sxs-lookup"><span data-stu-id="9452f-135">Delete a user</span></span>](https://docs.microsoft.com/azure/active-directory/fundamentals/add-users-azure-active-directory)
- [<span data-ttu-id="9452f-136">Добавяне или актуализиране на информация за потребителския профил чрез Azure Active Directory</span><span class="sxs-lookup"><span data-stu-id="9452f-136">Add or update a user's profile information using Azure Active Directory</span></span>](https://docs.microsoft.com/azure/active-directory/fundamentals/active-directory-users-profile-azure-portal)

<span data-ttu-id="9452f-137">**Препоръчвани документи**</span><span class="sxs-lookup"><span data-stu-id="9452f-137">**Recommended documents**</span></span>

- [<span data-ttu-id="9452f-138">Какво представлява базираното на роли управление на достъпа (RBAC)?</span><span class="sxs-lookup"><span data-stu-id="9452f-138">What is role-based access control (RBAC)?</span></span>](https://docs.microsoft.com/azure/role-based-access-control/overview)
- [<span data-ttu-id="9452f-139">Разбиране на различните роли в Azure</span><span class="sxs-lookup"><span data-stu-id="9452f-139">Understand the different roles in Azure</span></span>](https://docs.microsoft.com/azure/role-based-access-control/rbac-and-directory-admin-roles)
- [<span data-ttu-id="9452f-140">Разрешения за роля на администратор в Azure Active Directory</span><span class="sxs-lookup"><span data-stu-id="9452f-140">Administrator role permissions in Azure Active Directory</span></span>](https://docs.microsoft.com/azure/active-directory/roles/permissions-reference)
- [<span data-ttu-id="9452f-141">Урок: предоставяне на достъп за потребител чрез RBAC и портал на Azure</span><span class="sxs-lookup"><span data-stu-id="9452f-141">Tutorial: Grant access for a user using RBAC and the Azure portal</span></span>](https://docs.microsoft.com/azure/role-based-access-control/quickstart-assign-role-user-portal)
- [<span data-ttu-id="9452f-142">Отстраняване на проблеми с RBAC в Azure</span><span class="sxs-lookup"><span data-stu-id="9452f-142">Troubleshoot RBAC in Azure</span></span>](https://docs.microsoft.com/azure/role-based-access-control/troubleshooting)
- [<span data-ttu-id="9452f-143">Организиране на вашите ресурси с групи за управление на Azure</span><span class="sxs-lookup"><span data-stu-id="9452f-143">Organize your resources with Azure management groups</span></span>](https://docs.microsoft.com/azure/governance/management-groups/overview)
- [<span data-ttu-id="9452f-144">Как да поискате копие на Azure фактура по имейл</span><span class="sxs-lookup"><span data-stu-id="9452f-144">How to request copy of Azure invoice via email</span></span>](https://azure.microsoft.com/en-us/blog/azure-email-invoices/)
- [<span data-ttu-id="9452f-145">Как да добавите, актуализирате или премахнете кредитна или дебитна карта от Azure</span><span class="sxs-lookup"><span data-stu-id="9452f-145">How to add, update or remove a credit or debit card from Azure</span></span>](https://docs.microsoft.com/azure/cost-management-billing/manage/change-credit-card)
- [<span data-ttu-id="9452f-146">Управление (повторно активиране/отмяна/превключване) на абонамент</span><span class="sxs-lookup"><span data-stu-id="9452f-146">Manage (Reactivate/Cancel/Switch) subscription</span></span>](https://docs.microsoft.com/azure/cost-management-billing/manage/subscription-disabled)



