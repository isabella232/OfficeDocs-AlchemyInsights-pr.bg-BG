---
title: Проблеми с използването на конзолата за администриране на администратора
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/29/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "1790"
- "9000214"
ms.openlocfilehash: 10b37b2ffda50dc77396039a9e0e443ad81aef72
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: bg-BG
ms.lasthandoff: 09/14/2020
ms.locfileid: "47728276"
---
# <a name="problems-using-the-intune-admin-console"></a><span data-ttu-id="4a682-102">Проблеми с използването на конзолата за администриране на администратора</span><span class="sxs-lookup"><span data-stu-id="4a682-102">Problems using the Intune admin console</span></span>

<span data-ttu-id="4a682-103">**"Достъпът е отказан" при навигация в портала за администриране на администратора.**</span><span class="sxs-lookup"><span data-stu-id="4a682-103">**"Access denied" when navigating the Intune admin portal.**</span></span>

- <span data-ttu-id="4a682-104">Ако сте член на персонализирана роля по избор, се уверете, че за вашия акаунт е присвоен лиценз за настройка или корпоративен пакет за мобилност (EMS).</span><span class="sxs-lookup"><span data-stu-id="4a682-104">If you are a member of an Intune custom role, ensure that an Intune or Enterprise Mobility Suite (EMS) license is assigned to your account.</span></span>
- <span data-ttu-id="4a682-105">Ако използвате конфигурационен Диспечер за управление на устройства, уверете се, че не сте част от потребителската колекция за конфигуриране на диспечера за конфигурация MDM.</span><span class="sxs-lookup"><span data-stu-id="4a682-105">If you are using Configuration Manager to manage devices, verify you are not part of the Intune user collection for Configuration Manager MDM.</span></span>
- <span data-ttu-id="4a682-106">Уверете се, че сте задали подходящите разрешения за управление, базирано на роли (RBAC), в острието на ролите.</span><span class="sxs-lookup"><span data-stu-id="4a682-106">Verify that you have been assigned the appropriate role-based administration control (RBAC) permissions in the Intune roles blade.</span></span>
- <span data-ttu-id="4a682-107">Проверете дали използваната група не е списък за разпространение.</span><span class="sxs-lookup"><span data-stu-id="4a682-107">Verify the group used is not a distribution list.</span></span> <span data-ttu-id="4a682-108">Настройването в портала на Azure поддържа само потребителски акаунти, които принадлежат на групи за защита на Azure Active Directory.</span><span class="sxs-lookup"><span data-stu-id="4a682-108">Intune in the Azure portal only supports user accounts that belong to Azure Active Directory security groups.</span></span> <span data-ttu-id="4a682-109">Преглеждайте своите групи в портала на Azure, за > групи за **Настройване**  >  **Groups**или в портала на Azure > **Azure Active Directory**.</span><span class="sxs-lookup"><span data-stu-id="4a682-109">Review your groups in the Azure portal > **Intune** > **Groups**, or in Azure portal > **Azure Active Directory**.</span></span>

<span data-ttu-id="4a682-110">**Потребителят има твърде много разрешения за присвоена роля на ненастроие**</span><span class="sxs-lookup"><span data-stu-id="4a682-110">**User has too many permissions for assigned Intune role**</span></span>

<span data-ttu-id="4a682-111">Информирайте потребителя, за да **отидете в**  >  **ролите**за настройване на "  >  **моите разрешения**  >  за**експортиране** ", за да прегледате разрешените разрешения.</span><span class="sxs-lookup"><span data-stu-id="4a682-111">Advise the user to go to **Intune** > **Intune roles** > **My permissions** > **Export** to review granted permissions.</span></span>

<span data-ttu-id="4a682-112">**Добавих група за обхват към роля, но потребителите в тази роля все още виждат други потребители или устройства.**</span><span class="sxs-lookup"><span data-stu-id="4a682-112">**I added a scope group to a role, but users in that role still see other users or devices.**</span></span>

<span data-ttu-id="4a682-113">Групите за обхват не филтрират потребители или устройства.</span><span class="sxs-lookup"><span data-stu-id="4a682-113">Scope groups do not filter out users or devices.</span></span> <span data-ttu-id="4a682-114">Групи обхвати:</span><span class="sxs-lookup"><span data-stu-id="4a682-114">Scope groups:</span></span>

- <span data-ttu-id="4a682-115">Ограничаване на потребителите, на които може да се присвояват правила или приложения.</span><span class="sxs-lookup"><span data-stu-id="4a682-115">Limit who users can assign policies or applications to.</span></span>
- <span data-ttu-id="4a682-116">Позволяване само на определени потребители да изпълняват отдалечени задачи на устройства.</span><span class="sxs-lookup"><span data-stu-id="4a682-116">Allow only specific users to run remote tasks on devices.</span></span>

<span data-ttu-id="4a682-117">За повече информация за групите обхвати вижте  [управление на достъпа, базирано на роли (RBAC), с Microsoft Настройте](https://docs.microsoft.com/intune/role-based-access-control).</span><span class="sxs-lookup"><span data-stu-id="4a682-117">For more information about scope groups, see  [Role-based access control (RBAC) with Microsoft Intune](https://docs.microsoft.com/intune/role-based-access-control).</span></span>

<span data-ttu-id="4a682-118">**Добавих потребител към роля за запознаване, но те все още имат пълен достъп до конзолата за администриране на администратора.**</span><span class="sxs-lookup"><span data-stu-id="4a682-118">**I added a user to an Intune role but they still have full access to the Intune admin console.**</span></span>

<span data-ttu-id="4a682-119">Придвижете се до Настройте > **потребители** в портала на Azure и проверете дали потребителят не е присвоен на никоя от следните роли в портала на Azure:</span><span class="sxs-lookup"><span data-stu-id="4a682-119">Navigate to Intune > **Users** in the Azure portal and verify that the user is not assigned to any of the following roles in the Azure portal:</span></span>

- <span data-ttu-id="4a682-120">Глобален администратор</span><span class="sxs-lookup"><span data-stu-id="4a682-120">Global administrator</span></span>
- <span data-ttu-id="4a682-121">Настройване на администратора на услугата</span><span class="sxs-lookup"><span data-stu-id="4a682-121">Intune service administrator</span></span>
- <span data-ttu-id="4a682-122">Администратор на SharePoint</span><span class="sxs-lookup"><span data-stu-id="4a682-122">SharePoint administrator</span></span>

<span data-ttu-id="4a682-123">За повече информация вижте [управление на достъпа, базирано на роли (RBAC), с помощта на Microsoft](https://docs.microsoft.com/intune/role-based-access-control).</span><span class="sxs-lookup"><span data-stu-id="4a682-123">For more info, see [Role-based access control (RBAC) with Microsoft Intune](https://docs.microsoft.com/intune/role-based-access-control).</span></span>

<span data-ttu-id="4a682-124">**Проблеми с достъпа**</span><span class="sxs-lookup"><span data-stu-id="4a682-124">**Access Issues**</span></span>

<span data-ttu-id="4a682-125">За повече информация вижте не можете да [влезете в Office 365, Azure или](https://support.microsoft.com/help/2412085/you-can-t-sign-in-to-office-365-azure-or-intune)в "Настройки".</span><span class="sxs-lookup"><span data-stu-id="4a682-125">For more info, see [You can't sign in to Office 365, Azure, or Intune](https://support.microsoft.com/help/2412085/you-can-t-sign-in-to-office-365-azure-or-intune).</span></span>