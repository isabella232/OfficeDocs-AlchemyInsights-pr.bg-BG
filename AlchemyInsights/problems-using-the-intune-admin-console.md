---
title: Проблеми с използване на интуне конзолата на администратора
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/29/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "1790"
- "9000214"
ms.openlocfilehash: 7a36d502a92d360b06336ccfa6183f666f0260ab
ms.sourcegitcommit: ffbed67c0a16ec423fa1d79b71e48ea4e2d320e1
ms.translationtype: MT
ms.contentlocale: bg-BG
ms.lasthandoff: 07/29/2020
ms.locfileid: "46554796"
---
# <a name="problems-using-the-intune-admin-console"></a><span data-ttu-id="62e7f-102">Проблеми с използване на интуне конзолата на администратора</span><span class="sxs-lookup"><span data-stu-id="62e7f-102">Problems using the Intune admin console</span></span>

<span data-ttu-id="62e7f-103">**"Достъпът е отказан" при навигиране на intune администраторския портал.**</span><span class="sxs-lookup"><span data-stu-id="62e7f-103">**"Access denied" when navigating the Intune admin portal.**</span></span>

- <span data-ttu-id="62e7f-104">Ако сте член на потребителска роля intune, уверете се, че лицензът Intune или Enterprise Mobility Suite (EMS) е присвоен на вашия акаунт.</span><span class="sxs-lookup"><span data-stu-id="62e7f-104">If you are a member of an Intune custom role, ensure that an Intune or Enterprise Mobility Suite (EMS) license is assigned to your account.</span></span>
- <span data-ttu-id="62e7f-105">Ако използвате Configuration Manager за управление на устройства, проверете не сте част от intune потребителски колекция за конфигурационен диспечер MDM.</span><span class="sxs-lookup"><span data-stu-id="62e7f-105">If you are using Configuration Manager to manage devices, verify you are not part of the Intune user collection for Configuration Manager MDM.</span></span>
- <span data-ttu-id="62e7f-106">Уверете се, че са присвоени подходящи ролеви управление (RBAC) разрешения в intune роли острие.</span><span class="sxs-lookup"><span data-stu-id="62e7f-106">Verify that you have been assigned the appropriate role-based administration control (RBAC) permissions in the Intune roles blade.</span></span>
- <span data-ttu-id="62e7f-107">Проверете дали използваната група не е списък за разпространение.</span><span class="sxs-lookup"><span data-stu-id="62e7f-107">Verify the group used is not a distribution list.</span></span> <span data-ttu-id="62e7f-108">Intune в портала на Azure поддържа само потребителски акаунти, които принадлежат към групи за защита на Azure Active Directory.</span><span class="sxs-lookup"><span data-stu-id="62e7f-108">Intune in the Azure portal only supports user accounts that belong to Azure Active Directory security groups.</span></span> <span data-ttu-id="62e7f-109">Прегледайте групите в портала на Azure > **Intune**  >  **групи**или в портала на Azure > **Azure Active Directory**.</span><span class="sxs-lookup"><span data-stu-id="62e7f-109">Review your groups in the Azure portal > **Intune** > **Groups**, or in Azure portal > **Azure Active Directory**.</span></span>

<span data-ttu-id="62e7f-110">**Потребителят има твърде много разрешения за присвоена роля на Intune**</span><span class="sxs-lookup"><span data-stu-id="62e7f-110">**User has too many permissions for assigned Intune role**</span></span>

<span data-ttu-id="62e7f-111">Съветва потребителя да отидете **на Intune**  >  **Intune роли**Моите  >  **разрешения**за  >  **експортиране** за преглед предоставени разрешения.</span><span class="sxs-lookup"><span data-stu-id="62e7f-111">Advise the user to go to **Intune** > **Intune roles** > **My permissions** > **Export** to review granted permissions.</span></span>

<span data-ttu-id="62e7f-112">**Добавих група от обхвати към роля, но потребителите в тази роля все още виждат други потребители или устройства.**</span><span class="sxs-lookup"><span data-stu-id="62e7f-112">**I added a scope group to a role, but users in that role still see other users or devices.**</span></span>

<span data-ttu-id="62e7f-113">Обхват групи не филтрират потребители или устройства.</span><span class="sxs-lookup"><span data-stu-id="62e7f-113">Scope groups do not filter out users or devices.</span></span> <span data-ttu-id="62e7f-114">Обхват групи:</span><span class="sxs-lookup"><span data-stu-id="62e7f-114">Scope groups:</span></span>

- <span data-ttu-id="62e7f-115">Ограничете потребителите, които могат да присвояват политики или приложения.</span><span class="sxs-lookup"><span data-stu-id="62e7f-115">Limit who users can assign policies or applications to.</span></span>
- <span data-ttu-id="62e7f-116">Позволява само на определени потребители да изпълняват отдалечени задачи на устройства.</span><span class="sxs-lookup"><span data-stu-id="62e7f-116">Allow only specific users to run remote tasks on devices.</span></span>

<span data-ttu-id="62e7f-117">За повече информация относно обхват групи вижте [ролеви контрол на достъпа (RBAC) с Microsoft Intune](https://docs.microsoft.com/intune/role-based-access-control).</span><span class="sxs-lookup"><span data-stu-id="62e7f-117">For more information about scope groups, see  [Role-based access control (RBAC) with Microsoft Intune](https://docs.microsoft.com/intune/role-based-access-control).</span></span>

<span data-ttu-id="62e7f-118">**Добавих потребител към ролята на Intune, но те все още имат пълен достъп до intune администратор конзола.**</span><span class="sxs-lookup"><span data-stu-id="62e7f-118">**I added a user to an Intune role but they still have full access to the Intune admin console.**</span></span>

<span data-ttu-id="62e7f-119">Навигирайте до Intune > **потребители** в портала на Azure и проверете дали потребителят не е присвоен на някоя от следните роли в портала на Azure:</span><span class="sxs-lookup"><span data-stu-id="62e7f-119">Navigate to Intune > **Users** in the Azure portal and verify that the user is not assigned to any of the following roles in the Azure portal:</span></span>

- <span data-ttu-id="62e7f-120">Глобален администратор</span><span class="sxs-lookup"><span data-stu-id="62e7f-120">Global administrator</span></span>
- <span data-ttu-id="62e7f-121">Intune администратор на услуги</span><span class="sxs-lookup"><span data-stu-id="62e7f-121">Intune service administrator</span></span>
- <span data-ttu-id="62e7f-122">Администратор на SharePoint</span><span class="sxs-lookup"><span data-stu-id="62e7f-122">SharePoint administrator</span></span>

<span data-ttu-id="62e7f-123">За повече информация вижте [Ролеви базирани контрол на достъпа (RBAC) с Microsoft Intune](https://docs.microsoft.com/intune/role-based-access-control).</span><span class="sxs-lookup"><span data-stu-id="62e7f-123">For more info, see [Role-based access control (RBAC) with Microsoft Intune](https://docs.microsoft.com/intune/role-based-access-control).</span></span>

<span data-ttu-id="62e7f-124">**Проблеми с достъпа**</span><span class="sxs-lookup"><span data-stu-id="62e7f-124">**Access Issues**</span></span>

<span data-ttu-id="62e7f-125">За повече информация вижте [Не можете да влезете в Office 365, Azure или Intune](https://support.microsoft.com/help/2412085/you-can-t-sign-in-to-office-365-azure-or-intune).</span><span class="sxs-lookup"><span data-stu-id="62e7f-125">For more info, see [You can't sign in to Office 365, Azure, or Intune](https://support.microsoft.com/help/2412085/you-can-t-sign-in-to-office-365-azure-or-intune).</span></span>