---
title: Използване на инструмента за разполагане на Office
ms.author: pebaum
author: pebaum
ms.date: 12/17/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 7ff7cc06-76d0-468f-bd66-3f2760750d04
ms.openlocfilehash: c7e0e96f225030590fdd516eaf3115c93a6335b6
ms.sourcegitcommit: dd43cc0a9470f98b8ef2a3787c823801d674c666
ms.translationtype: MT
ms.contentlocale: bg-BG
ms.lasthandoff: 02/12/2019
ms.locfileid: "29898635"
---
# <a name="using-the-office-deployment-tool-odt"></a><span data-ttu-id="5eeac-102">С помощта на Office разполагане инструмент (ODT)</span><span class="sxs-lookup"><span data-stu-id="5eeac-102">Using the Office Deployment Tool (ODT)</span></span>

<span data-ttu-id="5eeac-p101">Използвайте Office разгръщане оръдие (ODT) да разположат Office 365 версии на Office. Инструмент за разгръщане служба (setup.exe) се управлява от командния ред и използва конфигурация XML файл, за да определи кои настройки да приложите при разполагането на Office.</span><span class="sxs-lookup"><span data-stu-id="5eeac-p101">You use the Office Deployment Tool (ODT) to deploy Office 365 versions of Office. The Office Deployment Tool (setup.exe) is run from the command line and uses a configuration XML file to determine what settings to apply when deploying Office.</span></span>
  
1. <span data-ttu-id="5eeac-105">Изтеглете най-новата версия на инструмента за разполагане на Office от [Microsoft Download център](http://go.microsoft.com/fwlink/p/?LinkID=626065).</span><span class="sxs-lookup"><span data-stu-id="5eeac-105">Download the latest version of the Office Deployment Tool from the [Microsoft Download Center](http://go.microsoft.com/fwlink/p/?LinkID=626065).</span></span>
    
2. <span data-ttu-id="5eeac-p102">Използвайте [Office Customization Tool (OCT)](https://config.office.com) да изберете предпочитанията си за разполагане и създаване на конфигурационния XML файл. Експортиране на конфигурационния файл и го поставете локално в същата папка, където пребивава setup.exe.</span><span class="sxs-lookup"><span data-stu-id="5eeac-p102">Use the [Office Customization Tool (OCT)](https://config.office.com) to select your deployment preferences and create the configuration XML file. Export the configuration file and place it locally on the same folder where the setup.exe resides.</span></span> 
    
    <span data-ttu-id="5eeac-p103">**Забележка:** Инсталирането на Office, често възникнат проблеми поради на липсващ или malformatted конфигурационни файлове. За да се избегнат такива проблеми, ви препоръчваме да използвате инструмента за персонализиране на Office за създаване на конфигурационния файл. Също така можете да импортирате съществуващи конфигурационни файлове в Office Customization Tool.</span><span class="sxs-lookup"><span data-stu-id="5eeac-p103">**Note:** Office installation issues commonly occur due to misconfigured or malformatted configuration files. To avoid such issues, we recommend that you use the Office Customization Tool to create the configuration file. You can also import existing configuration files into the Office Customization Tool.</span></span> 
    
3. <span data-ttu-id="5eeac-p104">От издигам заповядвам бърз шибалка към мястото, където пребивава setup.exe и изпълнение на инструмента за разполагане на Office в режим на изтегляне и зададете в конфигурационния файл, който току-що записахте. В този пример конфигурационния файл е с име Configuration.xml:</span><span class="sxs-lookup"><span data-stu-id="5eeac-p104">From an elevated command prompt, switch to the location where setup.exe resides and run the Office Deployment Tool in download mode and specify the configuration file you just saved. In this example, the configuration file is named Configuration.xml:</span></span>
    
  ```
  setup.exe /download Configuration.xml  
  ```

4. <span data-ttu-id="5eeac-113">Изпълнете инструмента за разполагане на Office в режим на конфигуриране и задайте конфигурационния файл.</span><span class="sxs-lookup"><span data-stu-id="5eeac-113">Run the Office Deployment Tool in configure mode and specify the configuration file.</span></span>
    
  ```
  setup.exe /configure Configuration.xml
  ```

    <span data-ttu-id="5eeac-114">**Забележка:** Трябва да изпълните тази стъпка от на клиентския компютър, на който искате да инсталирате Office и трябва да имате разрешения на локален администратор на този компютър.</span><span class="sxs-lookup"><span data-stu-id="5eeac-114">**Note:** You must run this step from the client computer on which you want to install Office and you must have local administrator permissions on that computer.</span></span> 
    
<span data-ttu-id="5eeac-p105">За да научите повече за използването на инструмента за внедряване на Office вашите Office 365 подпора за сценарии за разгръщане, вижте [Обзор на инструмента за разполагане на Office](https://docs.microsoft.com/deployoffice/overview-of-the-office-2016-deployment-tool). За повече подробности за това как да използвате инструмента за персонализиране на Office вижте [Обзор на инструмента за персонализиране на Office](https://docs.microsoft.com/DeployOffice/overview-of-the-office-customization-tool-for-click-to-run).</span><span class="sxs-lookup"><span data-stu-id="5eeac-p105">To learn more about using Office Deployment Tool for your Office 365 ProPlus deployment scenarios, see [Overview of the Office Deployment Tool](https://docs.microsoft.com/deployoffice/overview-of-the-office-2016-deployment-tool). For more details on how to use the Office Customization Tool, see [Overview of the Office Customization Tool](https://docs.microsoft.com/DeployOffice/overview-of-the-office-customization-tool-for-click-to-run).</span></span>
  

