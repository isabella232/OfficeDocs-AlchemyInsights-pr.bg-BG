---
title: Използване на инструмента за разполагане на Office
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "918"
- "2000022"
ms.assetid: 7ff7cc06-76d0-468f-bd66-3f2760750d04
ms.openlocfilehash: f3a5dbfc6b64ccd4f0b19a5f86236336e78838d4
ms.sourcegitcommit: 35e2c122d8a838d98d1f0851c29b16282261580f
ms.translationtype: MT
ms.contentlocale: bg-BG
ms.lasthandoff: 11/17/2020
ms.locfileid: "49085821"
---
# <a name="using-the-office-deployment-tool-odt"></a><span data-ttu-id="c5b6b-102">Използване на инструмента за разполагане на Office (ODT)</span><span class="sxs-lookup"><span data-stu-id="c5b6b-102">Using the Office Deployment Tool (ODT)</span></span>

<span data-ttu-id="c5b6b-103">Можете да използвате инструмента за разполагане на Office (ODT), за да разположите версии на Office 365 на Office.</span><span class="sxs-lookup"><span data-stu-id="c5b6b-103">You use the Office Deployment Tool (ODT) to deploy Office 365 versions of Office.</span></span> <span data-ttu-id="c5b6b-104">Инструментът за разполагане на Office (setupodt.exe) се изпълнява от командния ред и използва конфигурационен XML файл, за да определи какви настройки да се прилагат при разполагането на Office.</span><span class="sxs-lookup"><span data-stu-id="c5b6b-104">The Office Deployment Tool (setupodt.exe) is run from the command line and uses a configuration XML file to determine what settings to apply when deploying Office.</span></span>
  
1. <span data-ttu-id="c5b6b-105">Изтеглете най-новата версия на инструмента за разполагане на Office от [центъра на Microsoft за изтегляния](https://go.microsoft.com/fwlink/p/?LinkID=626065).</span><span class="sxs-lookup"><span data-stu-id="c5b6b-105">Download the latest version of the Office Deployment Tool from the [Microsoft Download Center](https://go.microsoft.com/fwlink/p/?LinkID=626065).</span></span>

2. <span data-ttu-id="c5b6b-106">Използвайте [инструмента за персонализиране на Office (Oct)](https://config.office.com) , за да изберете своите предпочитания за разполагане и да създадете конфигурационен XML файл.</span><span class="sxs-lookup"><span data-stu-id="c5b6b-106">Use the [Office Customization Tool (OCT)](https://config.office.com) to select your deployment preferences and create the configuration XML file.</span></span> <span data-ttu-id="c5b6b-107">Експортирайте конфигурационния файл и го заместете локално в същата папка, където се намира setupodt.exe.</span><span class="sxs-lookup"><span data-stu-id="c5b6b-107">Export the configuration file and place it locally on the same folder where the setupodt.exe resides.</span></span>

    <span data-ttu-id="c5b6b-108">**Забележка:** Проблемите с инсталирането на Office често възникват поради неправилни конфигурирани или malformatted конфигурационни файлове.</span><span class="sxs-lookup"><span data-stu-id="c5b6b-108">**Note:** Office installation issues commonly occur due to misconfigured or malformatted configuration files.</span></span> <span data-ttu-id="c5b6b-109">За да избегнете такива проблеми, ви препоръчваме да използвате инструмента за персонализиране на Office, за да създадете конфигурационен файл.</span><span class="sxs-lookup"><span data-stu-id="c5b6b-109">To avoid such issues, we recommend that you use the Office Customization Tool to create the configuration file.</span></span> <span data-ttu-id="c5b6b-110">Можете също да импортирате съществуващи конфигурационни файлове в инструмента за персонализиране на Office.</span><span class="sxs-lookup"><span data-stu-id="c5b6b-110">You can also import existing configuration files into the Office Customization Tool.</span></span>

3. <span data-ttu-id="c5b6b-111">От команден прозорец с повишени стойности превключете на мястото, където се намира setupodt.exe, и изпълнете инструмента за разполагане на Office в режим на изтегляне и задайте конфигурационния файл, който току-що сте записали.</span><span class="sxs-lookup"><span data-stu-id="c5b6b-111">From an elevated command prompt, switch to the location where setupodt.exe resides and run the Office Deployment Tool in download mode and specify the configuration file you just saved.</span></span> <span data-ttu-id="c5b6b-112">В този пример Конфигурационният файл се нарича Configuration.xml:</span><span class="sxs-lookup"><span data-stu-id="c5b6b-112">In this example, the configuration file is named Configuration.xml:</span></span>

```setupodt.exe /download Configuration.xml```

<span data-ttu-id="c5b6b-113">4. Стартирайте инструмента за разполагане на Office в режим на конфигуриране и задайте конфигурационен файл.</span><span class="sxs-lookup"><span data-stu-id="c5b6b-113">4.Run the Office Deployment Tool in configure mode and specify the configuration file.</span></span>

```setupodt.exe /configure Configuration.xml```

<span data-ttu-id="c5b6b-114">**Забележка:** Трябва да изпълните тази стъпка от клиентския компютър, на който искате да инсталирате Office, и трябва да имате разрешения на локален администратор на този компютър.</span><span class="sxs-lookup"><span data-stu-id="c5b6b-114">**Note:** You must run this step from the client computer on which you want to install Office and you must have local administrator permissions on that computer.</span></span>

<span data-ttu-id="c5b6b-115">За да научите повече за това как да използвате инструмента за разполагане на Office за сценарии на Microsoft 365 за разработване на корпоративни приложения, вижте [общ преглед на инструмента за разполагане на Office](https://docs.microsoft.com/deployoffice/overview-office-deployment-tool).</span><span class="sxs-lookup"><span data-stu-id="c5b6b-115">To learn more about using Office Deployment Tool for your Microsoft 365 Apps for enterprise deployment scenarios, see [Overview of the Office Deployment Tool](https://docs.microsoft.com/deployoffice/overview-office-deployment-tool).</span></span> <span data-ttu-id="c5b6b-116">За повече информация как да използвате инструмента за персонализиране на Office, вижте [общ преглед на инструмента за персонализиране на Office](https://docs.microsoft.com/DeployOffice/overview-of-the-office-customization-tool-for-click-to-run).</span><span class="sxs-lookup"><span data-stu-id="c5b6b-116">For more details on how to use the Office Customization Tool, see [Overview of the Office Customization Tool](https://docs.microsoft.com/DeployOffice/overview-of-the-office-customization-tool-for-click-to-run).</span></span>
