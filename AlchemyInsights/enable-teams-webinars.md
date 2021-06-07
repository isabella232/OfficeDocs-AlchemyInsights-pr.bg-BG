---
title: Разрешаване Teams уебинари
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
- "11513"
- "9006672"
ms.openlocfilehash: 5a732e6746e9fd23e54a0b2ffeabb59623012a0e
ms.sourcegitcommit: 9de78b30602f917d58705057cdcce31fec349969
ms.translationtype: MT
ms.contentlocale: bg-BG
ms.lasthandoff: 06/04/2021
ms.locfileid: "52793532"
---
# <a name="enable-teams-webinars"></a><span data-ttu-id="cca8d-102">Разрешаване Teams уебинари</span><span class="sxs-lookup"><span data-stu-id="cca8d-102">Enable Teams Webinars</span></span>

<span data-ttu-id="cca8d-103">Уебинарите са разрешени по подразбиране.</span><span class="sxs-lookup"><span data-stu-id="cca8d-103">Webinars are enabled by default.</span></span> <span data-ttu-id="cca8d-104">Можете да управлявате кой може да планира и да се регистрира за Teams уебинари, като използвате Teams команди на PowerShell.</span><span class="sxs-lookup"><span data-stu-id="cca8d-104">You can manage who can schedule and register for Teams Webinars by using Teams PowerShell commands.</span></span>

- <span data-ttu-id="cca8d-105">Всички потребители, които могат да създадат събрание, също могат да създадат събрание на уебинар.</span><span class="sxs-lookup"><span data-stu-id="cca8d-105">All users who can create a meeting can also create a webinar meeting.</span></span> <span data-ttu-id="cca8d-106">Ако искате да управлявате кой може да планира Teams уебинари, използвайте *AllowMeetingRegistration*.</span><span class="sxs-lookup"><span data-stu-id="cca8d-106">If you want to manage who can schedule Teams Webinars, use *AllowMeetingRegistration*.</span></span> 
- <span data-ttu-id="cca8d-107">По подразбиране *WhoCanRegister е* разрешен и зададен на **Всеки**.</span><span class="sxs-lookup"><span data-stu-id="cca8d-107">By default, *WhoCanRegister* is enabled and set to **Everyone**.</span></span> <span data-ttu-id="cca8d-108">Ако искате да изключите регистрирането на събрание, *задайте AllowMeetingRegistration на* **False**.</span><span class="sxs-lookup"><span data-stu-id="cca8d-108">If you want to turn off meeting registration, set *AllowMeetingRegistration* to **False**.</span></span>

<span data-ttu-id="cca8d-109">За да промените тези настройки, трябва да [инсталирате Teams PowerShell](/microsoftteams/teams-powershell-install).</span><span class="sxs-lookup"><span data-stu-id="cca8d-109">To change these settings, you must install [Teams PowerShell](/microsoftteams/teams-powershell-install).</span></span> <span data-ttu-id="cca8d-110">Освен това правилата за събранията се прилагат Teams уебинари.</span><span class="sxs-lookup"><span data-stu-id="cca8d-110">Also, Meeting Policies are enforced on Teams Webinars.</span></span> <span data-ttu-id="cca8d-111">Ако например анонимното присъединяване е изключено в настройките на събранието, анонимните потребители не могат да се присъединят към уебинари.</span><span class="sxs-lookup"><span data-stu-id="cca8d-111">For example, if anonymous join is turned off in meeting settings, anonymous users can't join webinars.</span></span>

<span data-ttu-id="cca8d-112">За да научите повече за конфигурирането кой може да се регистрира за уебинари, вижте [Конфигуриране кой може да се регистрира за уебинари](/microsoftteams/set-up-webinars?source=docs#configure-who-can-register-for-webinars).</span><span class="sxs-lookup"><span data-stu-id="cca8d-112">To learn more about configuring who can register for webinars, see [Configure who can register for webinars](/microsoftteams/set-up-webinars?source=docs#configure-who-can-register-for-webinars).</span></span> <span data-ttu-id="cca8d-113">За повече информация относно настройките за списъци на Microsoft вижте Управление [на настройките за списъци на Microsoft](/sharepoint/control-lists).</span><span class="sxs-lookup"><span data-stu-id="cca8d-113">For more information about settings for Microsoft Lists, see [Control settings for Microsoft Lists](/sharepoint/control-lists).</span></span>