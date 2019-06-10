---
title: Достъп до услуги за пенсиониране
ms.author: kirks
author: Techwriter40
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: ''
ms.openlocfilehash: f5a1e88e4443fdf43cdd4f07cf9e784810df7540
ms.sourcegitcommit: 136b8209c52c2a05d0f2fdaab93b2cd92253fa2c
ms.translationtype: MT
ms.contentlocale: bg-BG
ms.lasthandoff: 06/07/2019
ms.locfileid: "34769426"
---
# <a name="access-services-retirement"></a><span data-ttu-id="bb6f5-102">Достъп до услуги за пенсиониране</span><span class="sxs-lookup"><span data-stu-id="bb6f5-102">Access services retirement</span></span>

<span data-ttu-id="bb6f5-103">Тъй като ние първоначално обявени в MC97576, през март 2017 г. и продължава да комуникират през изминалата година достъп до услуги са се оттегля от Office 365.</span><span class="sxs-lookup"><span data-stu-id="bb6f5-103">As we originally announced in MC97576, in March 2017, and continued to communicate over the past year Access Services are being retired from Office 365.</span></span> <span data-ttu-id="bb6f5-104">Следващата фаза в този процес ще бъде премахването на Access уеб бази данни, които използват SharePoint списъци като техните основни данни съхранение.</span><span class="sxs-lookup"><span data-stu-id="bb6f5-104">The next phase in this process will be the removal of Access Web Databases that use SharePoint lists as their underlying data storage.</span></span>

<span data-ttu-id="bb6f5-105">**Как това влияе ми?**</span><span class="sxs-lookup"><span data-stu-id="bb6f5-105">**How does this affect me?**</span></span>

<span data-ttu-id="bb6f5-106">Започва юни 2019, ние ще спре създаването на нови бази данни на Access в SharePoint Online и затварям голо възвишение служба и всички останали приложения от април 2020.</span><span class="sxs-lookup"><span data-stu-id="bb6f5-106">Starting June 2019, we will stop creation of new Access databases in SharePoint Online and shut down the service and any remaining apps by April 2020.</span></span>

<span data-ttu-id="bb6f5-107">**Какво трябва да направя, за да се подготвят за тази промяна?**</span><span class="sxs-lookup"><span data-stu-id="bb6f5-107">**What do I need to do to prepare for this change?**</span></span>

<span data-ttu-id="bb6f5-108">Препоръчваме ви да създадете план на преход за уеб бази данни Access за вашата организация.</span><span class="sxs-lookup"><span data-stu-id="bb6f5-108">We encourage you to create a transition plan for your organization’s Access web databases.</span></span> <span data-ttu-id="bb6f5-109">Администраторите могат да използват [SharePoint достъп ап скенер](https://github.com/SharePoint/PnP-Tools/tree/master/Solutions/SharePoint.AccessApp.Scanner) да получи опис на достъп до приложения, които използват сайтове.</span><span class="sxs-lookup"><span data-stu-id="bb6f5-109">Admins can use the [SharePoint Access app scanner](https://github.com/SharePoint/PnP-Tools/tree/master/Solutions/SharePoint.AccessApp.Scanner) to obtain an inventory of the Access apps that sites are using.</span></span> 

<span data-ttu-id="bb6f5-110">Има няколко начина за мигриране на данни от Access уеб бази данни:</span><span class="sxs-lookup"><span data-stu-id="bb6f5-110">There are several ways to migrate Access web databases data:</span></span>

- <span data-ttu-id="bb6f5-111">Импортиране към местни достъп до база данни (. ACCDB) или към файл на Excel.</span><span class="sxs-lookup"><span data-stu-id="bb6f5-111">Importing to a local Access database (.ACCDB) or to an Excel file.</span></span>
- <span data-ttu-id="bb6f5-112">Ние също така препоръчват изследване Microsoft PowerApps като алтернативна платформа за създаване на некодирани бизнес решения за уеб и мобилни устройства.</span><span class="sxs-lookup"><span data-stu-id="bb6f5-112">We also recommend exploring Microsoft PowerApps as an alternative platform to create no-code business solutions for web and mobile devices.</span></span>