---
title: Пенсиониране на услугите за достъп
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
ms.openlocfilehash: 977bd5887ef58b328463a9befcd6b47ac55f5a85
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: bg-BG
ms.lasthandoff: 04/22/2020
ms.locfileid: "43687247"
---
# <a name="access-services-retirement"></a><span data-ttu-id="289da-102">Пенсиониране на услугите за достъп</span><span class="sxs-lookup"><span data-stu-id="289da-102">Access services retirement</span></span>

<span data-ttu-id="289da-103">Както първоначално обявихме в MC97576, през март 2017 г. и продължида комуникира през изминалата година Услугите за достъп се пенсионират.</span><span class="sxs-lookup"><span data-stu-id="289da-103">As we originally announced in MC97576, in March 2017, and continued to communicate over the past year Access Services are being retired.</span></span> <span data-ttu-id="289da-104">Следващата фаза в този процес ще бъде премахването на уеб бази данни на Access, които използват списъци на SharePoint като тяхна основна съхранение на данни.</span><span class="sxs-lookup"><span data-stu-id="289da-104">The next phase in this process will be the removal of Access Web Databases that use SharePoint lists as their underlying data storage.</span></span>

<span data-ttu-id="289da-105">**Как се отразява това на мен?**</span><span class="sxs-lookup"><span data-stu-id="289da-105">**How does this affect me?**</span></span>

<span data-ttu-id="289da-106">От юни 2019, ние ще спре създаването на нови бази данни на Access в SharePoint Online и изключване на услугата и всички останали приложения до април 2020.</span><span class="sxs-lookup"><span data-stu-id="289da-106">Starting June 2019, we will stop creation of new Access databases in SharePoint Online and shut down the service and any remaining apps by April 2020.</span></span>

<span data-ttu-id="289da-107">**Какво трябва да направя, за да се подготвя за тази промяна?**</span><span class="sxs-lookup"><span data-stu-id="289da-107">**What do I need to do to prepare for this change?**</span></span>

<span data-ttu-id="289da-108">Препоръчваме ви да създадете план за преход за уеб базите данни на вашата организация.</span><span class="sxs-lookup"><span data-stu-id="289da-108">We encourage you to create a transition plan for your organization's Access web databases.</span></span> <span data-ttu-id="289da-109">Администраторите могат да използват скенера на [приложението SharePoint Access,](https://github.com/SharePoint/PnP-Tools/tree/master/Solutions/SharePoint.AccessApp.Scanner) за да получите списък на приложенията на Access, които се използват от сайтовете.</span><span class="sxs-lookup"><span data-stu-id="289da-109">Admins can use the [SharePoint Access app scanner](https://github.com/SharePoint/PnP-Tools/tree/master/Solutions/SharePoint.AccessApp.Scanner) to obtain an inventory of the Access apps that sites are using.</span></span>

<span data-ttu-id="289da-110">Има няколко начина за мигриране на данни за уеб бази данни за Access:</span><span class="sxs-lookup"><span data-stu-id="289da-110">There are several ways to migrate Access web databases data:</span></span>

- <span data-ttu-id="289da-111">Импортиране в локална база данни на Access (. accdb) или към файл в Excel.</span><span class="sxs-lookup"><span data-stu-id="289da-111">Importing to a local Access database (.ACCDB) or to an Excel file.</span></span>
- <span data-ttu-id="289da-112">Препоръчваме също да проучите Microsoft PowerApps като алтернативна платформа за създаване на бизнес решения без код за уеб и мобилни устройства.</span><span class="sxs-lookup"><span data-stu-id="289da-112">We also recommend exploring Microsoft PowerApps as an alternative platform to create no-code business solutions for web and mobile devices.</span></span>