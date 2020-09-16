---
title: Проблеми с лицензирането в Yammer
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/14/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "5900"
- "9003071"
ms.openlocfilehash: f0a7625c7b77860e5ba0e29f2df47101749aace3
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: bg-BG
ms.lasthandoff: 09/14/2020
ms.locfileid: "47657265"
---
# <a name="yammer-licensing-issues"></a><span data-ttu-id="c1bd2-102">Проблеми с лицензирането в Yammer</span><span class="sxs-lookup"><span data-stu-id="c1bd2-102">Yammer licensing issues</span></span>

<span data-ttu-id="c1bd2-103">Всички потребители трябва да имат лиценз за използване на услугата Yammer Enterprise, но по подразбиране Yammer не изисква потребителите да имат лиценз за достъп до услугата.</span><span class="sxs-lookup"><span data-stu-id="c1bd2-103">All users must have a license to use the Yammer Enterprise service, but by default Yammer does not require that users have a license to access the service.</span></span> <span data-ttu-id="c1bd2-104">Когато администратор промени настройката за блокиране на потребители на Microsoft 365 без лицензи на Yammer, потребителите, на които не е даден лиценз за yammer Enterprise, нямат достъп до услугата Yammer.</span><span class="sxs-lookup"><span data-stu-id="c1bd2-104">When an administrator changes the setting to block Microsoft 365 users without Yammer licenses, users not assigned a Yammer Enterprise license can't access the Yammer service.</span></span> <span data-ttu-id="c1bd2-105">За повече информация вижте [управление на потребителските лицензи за Yammer в Office 365](https://docs.microsoft.com/yammer/manage-yammer-users/manage-yammer-licenses-in-office-365)</span><span class="sxs-lookup"><span data-stu-id="c1bd2-105">For more info, see [Manage Yammer user licenses in Office 365](https://docs.microsoft.com/yammer/manage-yammer-users/manage-yammer-licenses-in-office-365)</span></span> 

<span data-ttu-id="c1bd2-106">Когато лицензи се премахват от потребители, плочката Yammer вече не се показва и други услуги могат да използват премахването на лицензи, за да скриват функции.</span><span class="sxs-lookup"><span data-stu-id="c1bd2-106">When licenses are removed from users, the Yammer tile is no longer displayed, and other services can use license removal to hide features.</span></span> <span data-ttu-id="c1bd2-107">В други случаи функциите все още могат да се появяват, но изисква присвояване на лиценз за работа.</span><span class="sxs-lookup"><span data-stu-id="c1bd2-107">In other cases, features can still appear but require licence assignment to operate.</span></span>  

<span data-ttu-id="c1bd2-108">**Лицензът не се актуализира за потребителя**</span><span class="sxs-lookup"><span data-stu-id="c1bd2-108">**License is not getting updated for the user**</span></span>  

<span data-ttu-id="c1bd2-109">Понякога на даден потребител е присвоен лиценз, но все още не може да получи достъп до Yammer.</span><span class="sxs-lookup"><span data-stu-id="c1bd2-109">Occasionally, a user is assigned a license but is still unable to access Yammer.</span></span> <span data-ttu-id="c1bd2-110">Забавянето е по-вероятно да възникне, когато се изпълнява задача за масово лицензиране.</span><span class="sxs-lookup"><span data-stu-id="c1bd2-110">Delays are more likely to occur when a mass license assignment is in progress.</span></span> <span data-ttu-id="c1bd2-111">Потребителите на Yammer може да не се актуализират по същия начин, по който се променят лицензите в Azure AD, тъй като системата се стартира асинхронно.</span><span class="sxs-lookup"><span data-stu-id="c1bd2-111">Yammer users might not be updated in the same order as licenses are changed in Azure AD because the system runs asynchronously.</span></span> <span data-ttu-id="c1bd2-112">Изчакайте до 24 часа, преди да отворите калъф за поддръжка, за да съобщите за проблеми при синхронизиране на лицензи.</span><span class="sxs-lookup"><span data-stu-id="c1bd2-112">Wait up to 24 hours before opening a support case to report license sync issues.</span></span>  

<span data-ttu-id="c1bd2-113">**Присвояване на групови лицензи**</span><span class="sxs-lookup"><span data-stu-id="c1bd2-113">**Bulk licence assignment**</span></span>  

<span data-ttu-id="c1bd2-114">Лицензи могат да бъдат присвоени чрез скриптове на центъра за администриране или PowerShell.</span><span class="sxs-lookup"><span data-stu-id="c1bd2-114">Licenses can be assigned through the admin center or PowerShell scripting.</span></span> <span data-ttu-id="c1bd2-115">За повече информация вижте даване [на лицензи на потребители](https://docs.microsoft.com/microsoft-365/admin/manage/assign-licenses-to-users) и даване [на лицензи на потребителски акаунти с Office 365 PowerShell](https://docs.microsoft.com/office365/enterprise/powershell/assign-licenses-to-user-accounts-with-office-365-powershell).</span><span class="sxs-lookup"><span data-stu-id="c1bd2-115">For more info, see [Assign licenses to users](https://docs.microsoft.com/microsoft-365/admin/manage/assign-licenses-to-users) and [Assign licenses to user accounts with Office 365 PowerShell](https://docs.microsoft.com/office365/enterprise/powershell/assign-licenses-to-user-accounts-with-office-365-powershell).</span></span> 

<span data-ttu-id="c1bd2-116">Поддръжката на Microsoft не предоставя съдействие при създаването на скриптове, но документацията за даване на лиценз за Yammer е налична.</span><span class="sxs-lookup"><span data-stu-id="c1bd2-116">Microsoft Support does not provide assistance with creating scripts, but documentation on Yammer license assignment is available.</span></span> <span data-ttu-id="c1bd2-117">За повече информация вижте [управление на лицензи за Yammer с помощта на Windows PowerShell](https://docs.microsoft.com/yammer/manage-yammer-users/manage-yammer-licenses-in-office-365#manage-yammer-licenses-by-using-windows-powershell).</span><span class="sxs-lookup"><span data-stu-id="c1bd2-117">For more info, see [Manage Yammer licenses by using Windows PowerShell](https://docs.microsoft.com/yammer/manage-yammer-users/manage-yammer-licenses-in-office-365#manage-yammer-licenses-by-using-windows-powershell).</span></span>