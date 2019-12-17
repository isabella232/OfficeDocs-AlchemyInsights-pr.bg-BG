---
title: Достъп до услуги за пенсиониране
ms.author: pebaum
author: pebaum
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "9000356"
- "2009"
ms.assetid: ''
ms.openlocfilehash: cb8123583b68e945ef878fdbaf211fd1d8205bb3
ms.sourcegitcommit: 0f0186044a3597e42ad14c32ca58e7224344dcfa
ms.translationtype: MT
ms.contentlocale: bg-BG
ms.lasthandoff: 12/15/2019
ms.locfileid: "40050478"
---
# <a name="access-services-retirement"></a><span data-ttu-id="b9d6f-102">Достъп до услуги за пенсиониране</span><span class="sxs-lookup"><span data-stu-id="b9d6f-102">Access services retirement</span></span>

<span data-ttu-id="b9d6f-103">Както първоначално обяви през MC97576., през март 2017, и продължи да комуникира през изминалата година услугите за достъп се пенсионираха от Office 365.</span><span class="sxs-lookup"><span data-stu-id="b9d6f-103">As we originally announced in MC97576, in March 2017, and continued to communicate over the past year Access Services are being retired from Office 365.</span></span> <span data-ttu-id="b9d6f-104">Следващата фаза в този процес ще бъде премахването на Access Web бази данни, които използват списъците на SharePoint като основни данни за съхранение.</span><span class="sxs-lookup"><span data-stu-id="b9d6f-104">The next phase in this process will be the removal of Access Web Databases that use SharePoint lists as their underlying data storage.</span></span>

<span data-ttu-id="b9d6f-105">**Как се отразява това на мен?**</span><span class="sxs-lookup"><span data-stu-id="b9d6f-105">**How does this affect me?**</span></span>

<span data-ttu-id="b9d6f-106">От юни 2019, ние ще спрем създаването на нови бази данни на Access в SharePoint online и изключете услугата и всички останали приложения до април 2020.</span><span class="sxs-lookup"><span data-stu-id="b9d6f-106">Starting June 2019, we will stop creation of new Access databases in SharePoint Online and shut down the service and any remaining apps by April 2020.</span></span>

<span data-ttu-id="b9d6f-107">**Какво трябва да направя, за да се подготвя за тази промяна?**</span><span class="sxs-lookup"><span data-stu-id="b9d6f-107">**What do I need to do to prepare for this change?**</span></span>

<span data-ttu-id="b9d6f-108">Насърчаваме ви да създадете план за преход за уеб базите данни за Access на вашата организация.</span><span class="sxs-lookup"><span data-stu-id="b9d6f-108">We encourage you to create a transition plan for your organization’s Access web databases.</span></span> <span data-ttu-id="b9d6f-109">Администраторите могат да използват [сканиране на приложението на SharePoint Access](https://github.com/SharePoint/PnP-Tools/tree/master/Solutions/SharePoint.AccessApp.Scanner) , за да получите списък на приложенията на Access, които сайтовете използват.</span><span class="sxs-lookup"><span data-stu-id="b9d6f-109">Admins can use the [SharePoint Access app scanner](https://github.com/SharePoint/PnP-Tools/tree/master/Solutions/SharePoint.AccessApp.Scanner) to obtain an inventory of the Access apps that sites are using.</span></span>

<span data-ttu-id="b9d6f-110">Има няколко начина за мигриране на данните за уеб бази данни на Access:</span><span class="sxs-lookup"><span data-stu-id="b9d6f-110">There are several ways to migrate Access web databases data:</span></span>

- <span data-ttu-id="b9d6f-111">Импортиране в локална база данни на Access (. ACCDB) или към файл на Excel.</span><span class="sxs-lookup"><span data-stu-id="b9d6f-111">Importing to a local Access database (.ACCDB) or to an Excel file.</span></span>
- <span data-ttu-id="b9d6f-112">Също така препоръчваме да разгледате Microsoft PowerApps като алтернативна платформа, за да създадете некодови бизнес решения за уеб и мобилни устройства.</span><span class="sxs-lookup"><span data-stu-id="b9d6f-112">We also recommend exploring Microsoft PowerApps as an alternative platform to create no-code business solutions for web and mobile devices.</span></span>