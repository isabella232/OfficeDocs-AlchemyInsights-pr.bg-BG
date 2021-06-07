---
title: Управление на регистрацията на уебинар
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 06/02/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "11512"
- "9006672"
ms.openlocfilehash: c5b0721d286b07d7e0f84199885b6f527a2b42a2
ms.sourcegitcommit: f7a9e97d04b7b6cbb633b32094d40f1874bf0fce
ms.translationtype: HT
ms.contentlocale: bg-BG
ms.lasthandoff: 06/06/2021
ms.locfileid: "52793566"
---
# <a name="manage-webinar-registration"></a><span data-ttu-id="3791a-102">Управление на регистрацията на уебинар</span><span class="sxs-lookup"><span data-stu-id="3791a-102">Manage webinar registration</span></span>

<span data-ttu-id="3791a-103">Можете да управлявате кой може да се регистрира Teams уебинари с помощта на Teams команди на Powershell.</span><span class="sxs-lookup"><span data-stu-id="3791a-103">You manage who can register for Teams Webinars by using Teams Powershell commands.</span></span> <span data-ttu-id="3791a-104">За да инсталирате Teams Powershell, [вижте Teams PowerShell](/microsoftteams/teams-powershell-install).</span><span class="sxs-lookup"><span data-stu-id="3791a-104">To install Teams Powershell, see [Teams PowerShell](/microsoftteams/teams-powershell-install).</span></span> 

<span data-ttu-id="3791a-105">По подразбиране *WhoCanRegister е разрешен* и настроен на **EveryoneInCompany**.</span><span class="sxs-lookup"><span data-stu-id="3791a-105">By default, *WhoCanRegister* is enabled and set to **EveryoneInCompany**.</span></span> <span data-ttu-id="3791a-106">За да позволите на всеки, включително анонимни потребители, да се регистрира, трябва да зададете правилата за събрание на **всеки** с помощта на командата Powershell:</span><span class="sxs-lookup"><span data-stu-id="3791a-106">To allow anyone, including anonymous users, to register, you must set the Meeting Policy to **Everyone** by using the Powershell command:</span></span>

`Set-CsTeamsMeetingPolicy -WhoCanRegister Everyone`

<span data-ttu-id="3791a-107">**Забележка:** Ако анонимното присъединяване е изключено в настройките на събранието, анонимните потребители не могат да се присъединят към уебинари.</span><span class="sxs-lookup"><span data-stu-id="3791a-107">**Note**: If anonymous join is turned off in meeting settings, anonymous users can't join webinars.</span></span> <span data-ttu-id="3791a-108">За да научите повече и да разрешите тази настройка, вижте [Управление на настройките на събранието Microsoft Teams](/microsoftteams/meeting-settings-in-teams).</span><span class="sxs-lookup"><span data-stu-id="3791a-108">To learn more and enable this setting, see [Manage meeting settings in Microsoft Teams](/microsoftteams/meeting-settings-in-teams).</span></span>

<span data-ttu-id="3791a-109">Ако искате да изключите регистрирането на събрание, *задайте AllowMeetingRegistration на* **False**.</span><span class="sxs-lookup"><span data-stu-id="3791a-109">If you want to turn off meeting registration, set *AllowMeetingRegistration* to **False**.</span></span>

<span data-ttu-id="3791a-110">За да научите повече за конфигурирането кой може да се регистрира за уебинари, вижте [Конфигуриране кой може да се регистрира за уебинари](/microsoftteams/set-up-webinars?source=docs#configure-who-can-register-for-webinars).</span><span class="sxs-lookup"><span data-stu-id="3791a-110">To learn more about configuring who can register for webinars, see [Configure who can register for webinars](/microsoftteams/set-up-webinars?source=docs#configure-who-can-register-for-webinars).</span></span> <span data-ttu-id="3791a-111">За повече информация относно настройките за списъци на Microsoft вижте Управление [на настройките за списъци на Microsoft](/sharepoint/control-lists).</span><span class="sxs-lookup"><span data-stu-id="3791a-111">For more information about settings for Microsoft Lists, see [Control settings for Microsoft Lists](/sharepoint/control-lists).</span></span>
