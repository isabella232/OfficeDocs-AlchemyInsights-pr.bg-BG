---
title: Използване на инструмента за разполагане на Office
ms.author: pebaum
author: pebaum
ms.date: 12/17/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "918"
- "2000022"
ms.assetid: 7ff7cc06-76d0-468f-bd66-3f2760750d04
ms.openlocfilehash: 998f914f38fa9d1925f7003e634d7f11550f47da
ms.sourcegitcommit: 5fb7a4b28859690020efdea630d03e70cc0e6334
ms.translationtype: MT
ms.contentlocale: bg-BG
ms.lasthandoff: 06/28/2019
ms.locfileid: "35365514"
---
# <a name="using-the-office-deployment-tool-odt"></a><span data-ttu-id="e1746-102">С помощта на Office разполагане инструмент (ODT)</span><span class="sxs-lookup"><span data-stu-id="e1746-102">Using the Office Deployment Tool (ODT)</span></span>

<span data-ttu-id="e1746-103">Използвайте Office разгръщане оръдие (ODT) да разположат Office 365 версии на Office.</span><span class="sxs-lookup"><span data-stu-id="e1746-103">You use the Office Deployment Tool (ODT) to deploy Office 365 versions of Office.</span></span> <span data-ttu-id="e1746-104">Инструмент за разгръщане служба (setup.exe) се управлява от командния ред и използва конфигурация XML файл, за да определи кои настройки да приложите при разполагането на Office.</span><span class="sxs-lookup"><span data-stu-id="e1746-104">The Office Deployment Tool (setup.exe) is run from the command line and uses a configuration XML file to determine what settings to apply when deploying Office.</span></span>
  
1. <span data-ttu-id="e1746-105">Изтеглете най-новата версия на инструмента за разполагане на Office от [Microsoft Download център](http://go.microsoft.com/fwlink/p/?LinkID=626065).</span><span class="sxs-lookup"><span data-stu-id="e1746-105">Download the latest version of the Office Deployment Tool from the [Microsoft Download Center](http://go.microsoft.com/fwlink/p/?LinkID=626065).</span></span>

2. <span data-ttu-id="e1746-106">Използвайте [Office Customization Tool (OCT)](https://config.office.com) да изберете предпочитанията си за разполагане и създаване на конфигурационния XML файл.</span><span class="sxs-lookup"><span data-stu-id="e1746-106">Use the [Office Customization Tool (OCT)](https://config.office.com) to select your deployment preferences and create the configuration XML file.</span></span> <span data-ttu-id="e1746-107">Експортиране на конфигурационния файл и го поставете локално в същата папка, където пребивава setup.exe.</span><span class="sxs-lookup"><span data-stu-id="e1746-107">Export the configuration file and place it locally on the same folder where the setup.exe resides.</span></span>

    <span data-ttu-id="e1746-108">**Забележка:** Инсталирането на Office, често възникнат проблеми поради на липсващ или malformatted конфигурационни файлове.</span><span class="sxs-lookup"><span data-stu-id="e1746-108">**Note:** Office installation issues commonly occur due to misconfigured or malformatted configuration files.</span></span> <span data-ttu-id="e1746-109">За да се избегнат такива проблеми, ви препоръчваме да използвате инструмента за персонализиране на Office за създаване на конфигурационния файл.</span><span class="sxs-lookup"><span data-stu-id="e1746-109">To avoid such issues, we recommend that you use the Office Customization Tool to create the configuration file.</span></span> <span data-ttu-id="e1746-110">Също така можете да импортирате съществуващи конфигурационни файлове в Office Customization Tool.</span><span class="sxs-lookup"><span data-stu-id="e1746-110">You can also import existing configuration files into the Office Customization Tool.</span></span>

3. <span data-ttu-id="e1746-111">От издигам заповядвам бърз шибалка към мястото, където пребивава setup.exe и изпълнение на инструмента за разполагане на Office в режим на изтегляне и зададете в конфигурационния файл, който току-що записахте.</span><span class="sxs-lookup"><span data-stu-id="e1746-111">From an elevated command prompt, switch to the location where setup.exe resides and run the Office Deployment Tool in download mode and specify the configuration file you just saved.</span></span> <span data-ttu-id="e1746-112">В този пример конфигурационния файл е с име Configuration.xml:</span><span class="sxs-lookup"><span data-stu-id="e1746-112">In this example, the configuration file is named Configuration.xml:</span></span>
    
  ```
  setup.exe /download Configuration.xml  
  ```

4. <span data-ttu-id="e1746-113">Изпълнете инструмента за разполагане на Office в режим на конфигуриране и задайте конфигурационния файл.</span><span class="sxs-lookup"><span data-stu-id="e1746-113">Run the Office Deployment Tool in configure mode and specify the configuration file.</span></span>
    
  ```
  setup.exe /configure Configuration.xml
  ```

    <span data-ttu-id="e1746-114">**Забележка:** Трябва да изпълните тази стъпка от на клиентския компютър, на който искате да инсталирате Office и трябва да имате разрешения на локален администратор на този компютър.</span><span class="sxs-lookup"><span data-stu-id="e1746-114">**Note:** You must run this step from the client computer on which you want to install Office and you must have local administrator permissions on that computer.</span></span>

<span data-ttu-id="e1746-115">За да научите повече за използването на инструмента за внедряване на Office вашите Office 365 подпора за сценарии за разгръщане, вижте [Обзор на инструмента за разполагане на Office](https://docs.microsoft.com/deployoffice/overview-of-the-office-2016-deployment-tool).</span><span class="sxs-lookup"><span data-stu-id="e1746-115">To learn more about using Office Deployment Tool for your Office 365 ProPlus deployment scenarios, see [Overview of the Office Deployment Tool](https://docs.microsoft.com/deployoffice/overview-of-the-office-2016-deployment-tool).</span></span> <span data-ttu-id="e1746-116">За повече подробности за това как да използвате инструмента за персонализиране на Office вижте [Обзор на инструмента за персонализиране на Office](https://docs.microsoft.com/DeployOffice/overview-of-the-office-customization-tool-for-click-to-run).</span><span class="sxs-lookup"><span data-stu-id="e1746-116">For more details on how to use the Office Customization Tool, see [Overview of the Office Customization Tool](https://docs.microsoft.com/DeployOffice/overview-of-the-office-customization-tool-for-click-to-run).</span></span>
