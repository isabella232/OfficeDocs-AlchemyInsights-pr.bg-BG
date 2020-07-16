---
title: Проблеми с лицензирането на Yammer
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/14/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "5900"
- "9003071"
ms.openlocfilehash: 6d9b2126dc1ed90968738ddb2e249dce9857f1db
ms.sourcegitcommit: b677b85395b7244b2bf2b753468b696b4cf27c8d
ms.translationtype: MT
ms.contentlocale: bg-BG
ms.lasthandoff: 07/16/2020
ms.locfileid: "45148181"
---
# <a name="yammer-licensing-issues"></a><span data-ttu-id="d3129-102">Проблеми с лицензирането на Yammer</span><span class="sxs-lookup"><span data-stu-id="d3129-102">Yammer licensing issues</span></span>

<span data-ttu-id="d3129-103">Всички потребители трябва да имат лиценз за използване на yammer Enterprise услуга, но по подразбиране Yammer не изисква потребителите да имат лиценз за достъп до услугата.</span><span class="sxs-lookup"><span data-stu-id="d3129-103">All users must have a license to use the Yammer Enterprise service, but by default Yammer does not require that users have a license to access the service.</span></span> <span data-ttu-id="d3129-104">Когато администратор променя настройката да блокирате потребителите на Microsoft 365 без Yammer лицензи, потребителите не присвоени Yammer Enterprise лиценз не достъп до услугата Yammer.</span><span class="sxs-lookup"><span data-stu-id="d3129-104">When an administrator changes the setting to block Microsoft 365 users without Yammer licenses, users not assigned a Yammer Enterprise license can't access the Yammer service.</span></span> <span data-ttu-id="d3129-105">За повече информация вижте [управление на Yammer потребителски лицензи в Office 365](https://docs.microsoft.com/yammer/manage-yammer-users/manage-yammer-licenses-in-office-365)</span><span class="sxs-lookup"><span data-stu-id="d3129-105">For more info, see [Manage Yammer user licenses in Office 365](https://docs.microsoft.com/yammer/manage-yammer-users/manage-yammer-licenses-in-office-365)</span></span> 

<span data-ttu-id="d3129-106">Когато лицензи се премахват от потребителите, Yammer плочка вече не се показва и други услуги да използвате лиценз за премахване на функции.</span><span class="sxs-lookup"><span data-stu-id="d3129-106">When licenses are removed from users, the Yammer tile is no longer displayed, and other services can use license removal to hide features.</span></span> <span data-ttu-id="d3129-107">В други случаи характеристиките могат да се появят, но изискват да се извършва възлагането на лиценз.</span><span class="sxs-lookup"><span data-stu-id="d3129-107">In other cases, features can still appear but require licence assignment to operate.</span></span>  

<span data-ttu-id="d3129-108">**Лицензът не се актуализира за потребителя**</span><span class="sxs-lookup"><span data-stu-id="d3129-108">**License is not getting updated for the user**</span></span>  

<span data-ttu-id="d3129-109">Понякога потребител е присвоен лиценз, но все още не може да достъп до Yammer.</span><span class="sxs-lookup"><span data-stu-id="d3129-109">Occasionally, a user is assigned a license but is still unable to access Yammer.</span></span> <span data-ttu-id="d3129-110">Закъсненията са по-склонни да се случат, когато се извършва масово възлагане на лицензи.</span><span class="sxs-lookup"><span data-stu-id="d3129-110">Delays are more likely to occur when a mass license assignment is in progress.</span></span> <span data-ttu-id="d3129-111">Yammer потребители може да не се актуализира в същия ред като лицензи се променят в Azure AD защото системата работи асинхронно.</span><span class="sxs-lookup"><span data-stu-id="d3129-111">Yammer users might not be updated in the same order as licenses are changed in Azure AD because the system runs asynchronously.</span></span> <span data-ttu-id="d3129-112">Изчакайте до 24 часа, преди да отворите случай с поддръжка, за да съобщите за проблеми със синхронизирането на лицензи.</span><span class="sxs-lookup"><span data-stu-id="d3129-112">Wait up to 24 hours before opening a support case to report license sync issues.</span></span>  

<span data-ttu-id="d3129-113">**Разпределяне на насипни лицензии**</span><span class="sxs-lookup"><span data-stu-id="d3129-113">**Bulk licence assignment**</span></span>  

<span data-ttu-id="d3129-114">Лицензи могат да бъдат присвоени чрез център за администриране или PowerShell скриптове.</span><span class="sxs-lookup"><span data-stu-id="d3129-114">Licenses can be assigned through the admin center or PowerShell scripting.</span></span> <span data-ttu-id="d3129-115">За повече информация вижте [Присвояване на лицензи на потребители](https://docs.microsoft.com/microsoft-365/admin/manage/assign-licenses-to-users) и [Присвояване на лицензи към потребителски акаунти с Office 365 PowerShell](https://docs.microsoft.com/office365/enterprise/powershell/assign-licenses-to-user-accounts-with-office-365-powershell).</span><span class="sxs-lookup"><span data-stu-id="d3129-115">For more info, see [Assign licenses to users](https://docs.microsoft.com/microsoft-365/admin/manage/assign-licenses-to-users) and [Assign licenses to user accounts with Office 365 PowerShell](https://docs.microsoft.com/office365/enterprise/powershell/assign-licenses-to-user-accounts-with-office-365-powershell).</span></span> 

<span data-ttu-id="d3129-116">Поддръжката на Microsoft не предоставя помощ при създаване на скриптове, но документация за Присвояване на Yammer лиценз е налична.</span><span class="sxs-lookup"><span data-stu-id="d3129-116">Microsoft Support does not provide assistance with creating scripts, but documentation on Yammer license assignment is available.</span></span> <span data-ttu-id="d3129-117">За повече информация вижте [Управление на Yammer лицензи с помощта на Windows PowerShell](https://docs.microsoft.com/yammer/manage-yammer-users/manage-yammer-licenses-in-office-365#manage-yammer-licenses-by-using-windows-powershell).</span><span class="sxs-lookup"><span data-stu-id="d3129-117">For more info, see [Manage Yammer licenses by using Windows PowerShell](https://docs.microsoft.com/yammer/manage-yammer-users/manage-yammer-licenses-in-office-365#manage-yammer-licenses-by-using-windows-powershell).</span></span>