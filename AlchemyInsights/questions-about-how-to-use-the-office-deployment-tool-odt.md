---
title: Въпроси как да използвате инструмента за разполагане на Office (ODT)
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 3e88e0f3-c86d-4ab8-b076-59d0552318f9
ms.openlocfilehash: 20e0b6aa3c298ee0a4291c3da6ae46978177e81f
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: bg-BG
ms.lasthandoff: 04/15/2021
ms.locfileid: "51790321"
---
# <a name="questions-about-how-to-use-the-office-deployment-tool-odt"></a><span data-ttu-id="71137-102">Въпроси как да използвате инструмента за разполагане на Office (ODT)</span><span class="sxs-lookup"><span data-stu-id="71137-102">Questions about how to use the Office Deployment Tool (ODT)</span></span>

<span data-ttu-id="71137-103">Изтеглете инструмента за разполагане на Office от центъра [на Microsoft за изтегляния.](https://go.microsoft.com/fwlink/p/?LinkID=626065)</span><span class="sxs-lookup"><span data-stu-id="71137-103">Download the Office Deployment Tool from the [Microsoft Download Center](https://go.microsoft.com/fwlink/p/?LinkID=626065).</span></span>
  
<span data-ttu-id="71137-104">След като изтеглите файла, изпълнете саморазархивиране на изпълнимия файл, който съдържа изпълнимия файл на инструмента за разполагане на Office (setup.exe) и примерен конфигурационен файл (configuration.xml).</span><span class="sxs-lookup"><span data-stu-id="71137-104">After downloading the file, run the self-extracting executable file, which contains the Office Deployment Tool executable (setup.exe) and a sample configuration file (configuration.xml).</span></span>
  
 <span data-ttu-id="71137-105">**За да изключите или премахнете приложенията на Microsoft 365 за корпоративни продукти от клиентски компютри:**</span><span class="sxs-lookup"><span data-stu-id="71137-105">**To exclude or remove Microsoft 365 Apps for enterprise products from client computers:**</span></span>
  
<span data-ttu-id="71137-106">Когато инсталирате Приложения на Microsoft 365 за предприятия, можете да изключите определени продукти.</span><span class="sxs-lookup"><span data-stu-id="71137-106">When installing Microsoft 365 Apps for enterprise, you can exclude specific products.</span></span> <span data-ttu-id="71137-107">За да направите това, следвайте стъпките за инсталиране на Office с ODT, но включете елемента ExcludeApp във вашия конфигурационен файл.</span><span class="sxs-lookup"><span data-stu-id="71137-107">To do so, follow the steps for installing Office with the ODT, but include the ExcludeApp element in your configuration file.</span></span> <span data-ttu-id="71137-108">Например този конфигурационен файл инсталира всички приложения на Microsoft 365 за корпоративни продукти с изключение на Publisher:</span><span class="sxs-lookup"><span data-stu-id="71137-108">For example, this configuration file installs all the Microsoft 365 Apps for enterprise products except Publisher:</span></span>
  
```
<Add SourcePath="\\Server\share" Version="15.1.2.3" OfficeClientEdition="32">
    <Product ID="O365ProPlusRetail" >
      <Language ID="en-us" />
      <ExcludeApp ID="Publisher" />
    </Product>
</Add>
```

[<span data-ttu-id="71137-109">Общ преглед на инструмента за разполагане на Office</span><span class="sxs-lookup"><span data-stu-id="71137-109">Overview of the Office Deployment Tool</span></span>](https://docs.microsoft.com/deployoffice/overview-office-deployment-tool)
  

