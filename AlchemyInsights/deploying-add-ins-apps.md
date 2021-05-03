---
title: Разполагане на добавки за Приложения на Microsoft 365
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 04/30/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "11107"
- "9005477"
ms.openlocfilehash: e55d8e5453f60b5993500dae1eb6efce11a8aa1a
ms.sourcegitcommit: d74039304002e526ba6f8ca02e76e4ce7e1aa743
ms.translationtype: MT
ms.contentlocale: bg-BG
ms.lasthandoff: 04/30/2021
ms.locfileid: "52124843"
---
# <a name="deploying-add-ins-for-microsoft-365-apps"></a><span data-ttu-id="4248c-102">Разполагане на добавки за Приложения на Microsoft 365</span><span class="sxs-lookup"><span data-stu-id="4248c-102">Deploying add-ins for Microsoft 365 Apps</span></span>

<span data-ttu-id="4248c-103">Централизирано разполагане е препоръчителният начин за разполагане Office добавки за потребители и групи във вашата организация.</span><span class="sxs-lookup"><span data-stu-id="4248c-103">Centralized Deployment is the recommended way for deploying Office add-ins to users and groups within your organization.</span></span> <span data-ttu-id="4248c-104">За да разположите добавки, изпълнете стъпките по-долу:</span><span class="sxs-lookup"><span data-stu-id="4248c-104">To deploy add-ins, follow the steps below:</span></span>

<span data-ttu-id="4248c-105">**Забележка:** За да инсталирате добавки за Office като отделен потребител, вижте [Преглед, управление](https://support.microsoft.com/topic/view-manage-and-install-add-ins-in-office-programs-16278816-1948-4028-91e5-76dca5380f8d)и инсталиране на добавки в Office програми .</span><span class="sxs-lookup"><span data-stu-id="4248c-105">**Note:** To install add-ins for Office as an individual user, see [View, manage, and install add-ins in Office programs](https://support.microsoft.com/topic/view-manage-and-install-add-ins-in-office-programs-16278816-1948-4028-91e5-76dca5380f8d).</span></span> <span data-ttu-id="4248c-106">Също така се уверете, че е разрешено индивидуално Office на добавки в магазина.</span><span class="sxs-lookup"><span data-stu-id="4248c-106">Also, make sure that individual acquisition of Office Store add-ins is enabled.</span></span> 

1. <span data-ttu-id="4248c-107">Уверете се, че вашата среда отговаря на изискванията за разполагане на добавки с помощта на централизирано разполагане.</span><span class="sxs-lookup"><span data-stu-id="4248c-107">Ensure that your environment meets the requirements for deployment of add-ins using Centralized Deployment.</span></span> <span data-ttu-id="4248c-108">За подробности вижте [Изисквания](https://docs.microsoft.com/microsoft-365/admin/manage/centralized-deployment-of-add-ins?#requirements).</span><span class="sxs-lookup"><span data-stu-id="4248c-108">For details, see [Requirements](https://docs.microsoft.com/microsoft-365/admin/manage/centralized-deployment-of-add-ins?#requirements).</span></span>
2. <span data-ttu-id="4248c-109">Отидете на **Настройки** Приложения Получаване на приложения  >    >   в центъра за Microsoft 365 за администриране, за да разположите добавки.</span><span class="sxs-lookup"><span data-stu-id="4248c-109">Go to **Settings** > **Integrated Apps** > **Get apps** in the Microsoft 365 admin center to deploy add-ins.</span></span> 

<span data-ttu-id="4248c-110">Бележки:</span><span class="sxs-lookup"><span data-stu-id="4248c-110">Notes:</span></span> 

- <span data-ttu-id="4248c-111">Интегрираните приложения изискват администраторът да има разрешения за глобален администратор или Exchange администратор.</span><span class="sxs-lookup"><span data-stu-id="4248c-111">Integrated Apps requires that the admin has Global Admin or Exchange Admin permissions.</span></span>

- <span data-ttu-id="4248c-112">Когато разполагате добавки за няколко потребители, ви препоръчваме да извършвате задачи с помощта на групи, а не на отделни потребители.</span><span class="sxs-lookup"><span data-stu-id="4248c-112">When deploying add-ins to multiple users, we recommend making assignments by using groups instead of individual users.</span></span> <span data-ttu-id="4248c-113">За подробности вижте [Съображения при присвояване на добавка към потребители и групи](https://docs.microsoft.com/microsoft-365/admin/manage/manage-deployment-of-add-ins?view=o365-worldwide#considerations-when-assigning-an-add-in-to-users-and-groups).</span><span class="sxs-lookup"><span data-stu-id="4248c-113">For details, see [Considerations when assigning an add-in to users and groups](https://docs.microsoft.com/microsoft-365/admin/manage/manage-deployment-of-add-ins?view=o365-worldwide#considerations-when-assigning-an-add-in-to-users-and-groups).</span></span>

- <span data-ttu-id="4248c-114">Централизирано разполагане не поддържа потребители в вложени групи или групи, които имат родителски групи.</span><span class="sxs-lookup"><span data-stu-id="4248c-114">Centralized Deployment doesn't support users in nested groups or groups that have parent groups.</span></span> <span data-ttu-id="4248c-115">За подробности вижте [Задачи на потребител и група](https://docs.microsoft.com/microsoft-365/admin/manage/centralized-deployment-of-add-ins?view=o365-worldwide#user-and-group-assignments).</span><span class="sxs-lookup"><span data-stu-id="4248c-115">For details, see [User and group assignments](https://docs.microsoft.com/microsoft-365/admin/manage/centralized-deployment-of-add-ins?view=o365-worldwide#user-and-group-assignments).</span></span>

- <span data-ttu-id="4248c-116">Уверете се, че услугата за управление на приложения на Microsoft 365 (GUID: '0517ffae-825d-4aff-999e-3f2336b8a20a') е разрешена за влизане от потребителите.</span><span class="sxs-lookup"><span data-stu-id="4248c-116">Ensure that the Microsoft 365 App Management Service (GUID: '0517ffae-825d-4aff-999e-3f2336b8a20a') is enabled for users to sign in.</span></span> <span data-ttu-id="4248c-117">За подробности вижте Конфигуриране [на свойствата на приложението](https://docs.microsoft.com/azure/active-directory/manage-apps/add-application-portal-configure#configure-app-properties).</span><span class="sxs-lookup"><span data-stu-id="4248c-117">For details, see [Configure app properties](https://docs.microsoft.com/azure/active-directory/manage-apps/add-application-portal-configure#configure-app-properties).</span></span>

- <span data-ttu-id="4248c-118">Ако имате проблеми с разполагането на добавки с помощта на интегрирани приложения, опитайте да разположите [с помощта на добавки](https://admin.microsoft.com/AdminPortal/Home?#/Settings/AddIns).</span><span class="sxs-lookup"><span data-stu-id="4248c-118">If you experience issues deploying add-ins by using Integrated Apps, try deploying by using [Add-Ins](https://admin.microsoft.com/AdminPortal/Home?#/Settings/AddIns).</span></span>

<span data-ttu-id="4248c-119">За повече информация вижте:</span><span class="sxs-lookup"><span data-stu-id="4248c-119">For more information, see:</span></span>

<span data-ttu-id="4248c-120">[Разполагане на добавки в центъра за администриране](https://docs.microsoft.com/microsoft-365/admin/manage/manage-deployment-of-add-ins) 
 [Управление на добавки в центъра за администриране](https://docs.microsoft.com/microsoft-365/admin/manage/manage-addins-in-the-admin-center) 
 [Използване на кратки команди на PowerShell за централизирано разполагане за управление на добавки](https://docs.microsoft.com/microsoft-365/enterprise/use-the-centralized-deployment-powershell-cmdlets-to-manage-add-ins) 
 [Публикуване Office добавки с помощта на централизирано разполагане чрез центъра Microsoft 365 администриране](https://docs.microsoft.com/office/dev/add-ins/publish/centralized-deployment#publish-an-office-add-in-via-centralized-deployment) 
 [Отстраняване на неизправности: Потребител не вижда добавки](https://docs.microsoft.com/office365/troubleshoot/access-management/user-not-seeing-add-ins) 
 [Отстраняване на грешки на потребители Office добавки](https://docs.microsoft.com/office/dev/add-ins/testing/testing-and-troubleshooting)</span><span class="sxs-lookup"><span data-stu-id="4248c-120">[Deploy add-ins in the admin center](https://docs.microsoft.com/microsoft-365/admin/manage/manage-deployment-of-add-ins)
[Manage add-ins in the admin center](https://docs.microsoft.com/microsoft-365/admin/manage/manage-addins-in-the-admin-center)
[Use the Centralized Deployment PowerShell cmdlets to manage add-ins](https://docs.microsoft.com/microsoft-365/enterprise/use-the-centralized-deployment-powershell-cmdlets-to-manage-add-ins)
[Publish Office Add-ins using Centralized Deployment via the Microsoft 365 admin center](https://docs.microsoft.com/office/dev/add-ins/publish/centralized-deployment#publish-an-office-add-in-via-centralized-deployment)
[Troubleshoot: User not seeing add-ins](https://docs.microsoft.com/office365/troubleshoot/access-management/user-not-seeing-add-ins)
[Troubleshoot user errors with Office Add-ins](https://docs.microsoft.com/office/dev/add-ins/testing/testing-and-troubleshooting)</span></span>