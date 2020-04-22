---
title: Въпроси относно използването на инструмента за разполагане на Office (ODT)
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 3e88e0f3-c86d-4ab8-b076-59d0552318f9
ms.openlocfilehash: 96d3f70f554f71c43d6458ec8debc099cd9fb040
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: bg-BG
ms.lasthandoff: 04/22/2020
ms.locfileid: "43698047"
---
# <a name="questions-about-how-to-use-the-office-deployment-tool-odt"></a><span data-ttu-id="8d145-102">Въпроси относно използването на инструмента за разполагане на Office (ODT)</span><span class="sxs-lookup"><span data-stu-id="8d145-102">Questions about how to use the Office Deployment Tool (ODT)</span></span>

<span data-ttu-id="8d145-103">Изтеглете инструмента за разполагане на Office от центъра на [Microsoft за изтегляния](https://go.microsoft.com/fwlink/p/?LinkID=626065).</span><span class="sxs-lookup"><span data-stu-id="8d145-103">Download the Office Deployment Tool from the [Microsoft Download Center](https://go.microsoft.com/fwlink/p/?LinkID=626065).</span></span>
  
<span data-ttu-id="8d145-104">След изтеглянето на файла изпълнете саморазархивиращия се изпълним файл, който съдържа изпълнимия файл на инструмента за разполагане на Office (setup.exe) и примерен конфигурационен файл (configuration.xml).</span><span class="sxs-lookup"><span data-stu-id="8d145-104">After downloading the file, run the self-extracting executable file, which contains the Office Deployment Tool executable (setup.exe) and a sample configuration file (configuration.xml).</span></span>
  
 <span data-ttu-id="8d145-105">**За да изключите или премахнете Microsoft 365 приложения за корпоративни продукти от клиентски компютри:**</span><span class="sxs-lookup"><span data-stu-id="8d145-105">**To exclude or remove Microsoft 365 Apps for enterprise products from client computers:**</span></span>
  
<span data-ttu-id="8d145-106">Когато инсталирате приложенията на Microsoft 365 за предприятие, можете да изключите конкретни продукти.</span><span class="sxs-lookup"><span data-stu-id="8d145-106">When installing Microsoft 365 Apps for enterprise, you can exclude specific products.</span></span> <span data-ttu-id="8d145-107">За да направите това, следвайте стъпките за инсталиране на Office с ODT, но включете excludeApp елемент в конфигурационния файл.</span><span class="sxs-lookup"><span data-stu-id="8d145-107">To do so, follow the steps for installing Office with the ODT, but include the ExcludeApp element in your configuration file.</span></span> <span data-ttu-id="8d145-108">Например този конфигурационен файл инсталира всички приложения на Microsoft 365 за корпоративни продукти с изключение на Издателя:</span><span class="sxs-lookup"><span data-stu-id="8d145-108">For example, this configuration file installs all the Microsoft 365 Apps for enterprise products except Publisher:</span></span>
  
```
<Add SourcePath="\\Server\share" Version="15.1.2.3" OfficeClientEdition="32">
    <Product ID="O365ProPlusRetail" >
      <Language ID="en-us" />
      <ExcludeApp ID="Publisher" />
    </Product>
</Add>
```

[<span data-ttu-id="8d145-109">Преглед на инструмента за разполагане на Office</span><span class="sxs-lookup"><span data-stu-id="8d145-109">Overview of the Office Deployment Tool</span></span>](https://docs.microsoft.com/deployoffice/overview-of-the-office-2016-deployment-tool)
  

