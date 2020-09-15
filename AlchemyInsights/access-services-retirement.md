---
title: Пенсиониране в Access Services
ms.author: pebaum
author: pebaum
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "9000356"
- "2009"
ms.assetid: ''
ms.openlocfilehash: 943066d5ac76c0630554ee724bbab9a94086fae4
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: bg-BG
ms.lasthandoff: 09/14/2020
ms.locfileid: "47698635"
---
# <a name="access-services-retirement"></a><span data-ttu-id="a45d9-102">Пенсиониране в Access Services</span><span class="sxs-lookup"><span data-stu-id="a45d9-102">Access services retirement</span></span>

<span data-ttu-id="a45d9-103">Както първоначално обявихме в MC97576, през март 2017 и продължихме да комуникираме през изминалите услуги за достъп до години, се оттегляме.</span><span class="sxs-lookup"><span data-stu-id="a45d9-103">As we originally announced in MC97576, in March 2017, and continued to communicate over the past year Access Services are being retired.</span></span> <span data-ttu-id="a45d9-104">Следващият етап на този процес ще бъде премахването на уеб бази данни на Access, които използват списъци на SharePoint като тяхно място за съхранение на данни.</span><span class="sxs-lookup"><span data-stu-id="a45d9-104">The next phase in this process will be the removal of Access Web Databases that use SharePoint lists as their underlying data storage.</span></span>

<span data-ttu-id="a45d9-105">**Как става това?**</span><span class="sxs-lookup"><span data-stu-id="a45d9-105">**How does this affect me?**</span></span>

<span data-ttu-id="a45d9-106">Започвайки от юни 2019, ние ще спрем създаването на нови бази данни на Access в SharePoint online и изключете услугата и всички останали приложения от април 2020.</span><span class="sxs-lookup"><span data-stu-id="a45d9-106">Starting June 2019, we will stop creation of new Access databases in SharePoint Online and shut down the service and any remaining apps by April 2020.</span></span>

<span data-ttu-id="a45d9-107">**Какво трябва да направя, за да се подготвя за тази промяна?**</span><span class="sxs-lookup"><span data-stu-id="a45d9-107">**What do I need to do to prepare for this change?**</span></span>

<span data-ttu-id="a45d9-108">Насърчаваме ви да създадете преходен план за уеб бази данни на Access на вашата организация.</span><span class="sxs-lookup"><span data-stu-id="a45d9-108">We encourage you to create a transition plan for your organization's Access web databases.</span></span> <span data-ttu-id="a45d9-109">Администраторите могат да използват [скенера за приложения на Access на SharePoint](https://github.com/SharePoint/PnP-Tools/tree/master/Solutions/SharePoint.AccessApp.Scanner) , за да получат опис на приложенията на Access, които използват сайтовете.</span><span class="sxs-lookup"><span data-stu-id="a45d9-109">Admins can use the [SharePoint Access app scanner](https://github.com/SharePoint/PnP-Tools/tree/master/Solutions/SharePoint.AccessApp.Scanner) to obtain an inventory of the Access apps that sites are using.</span></span>

<span data-ttu-id="a45d9-110">Има няколко начина за мигриране на данните на уеб базите данни на Access:</span><span class="sxs-lookup"><span data-stu-id="a45d9-110">There are several ways to migrate Access web databases data:</span></span>

- <span data-ttu-id="a45d9-111">Импортиране в локална база данни на Access (. ACCDB) или към файл на Excel.</span><span class="sxs-lookup"><span data-stu-id="a45d9-111">Importing to a local Access database (.ACCDB) or to an Excel file.</span></span>
- <span data-ttu-id="a45d9-112">Препоръчваме също да изследвате Microsoft PowerApps като алтернативна платформа, за да създавате бизнес решения без кодове за уеб и мобилни устройства.</span><span class="sxs-lookup"><span data-stu-id="a45d9-112">We also recommend exploring Microsoft PowerApps as an alternative platform to create no-code business solutions for web and mobile devices.</span></span>