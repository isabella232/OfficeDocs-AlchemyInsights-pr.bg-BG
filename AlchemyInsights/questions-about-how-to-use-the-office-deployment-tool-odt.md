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
# <a name="questions-about-how-to-use-the-office-deployment-tool-odt"></a>Въпроси как да използвате инструмента за разполагане на Office (ODT)

Изтеглете инструмента за разполагане на Office от центъра [на Microsoft за изтегляния.](https://go.microsoft.com/fwlink/p/?LinkID=626065)
  
След като изтеглите файла, изпълнете саморазархивиране на изпълнимия файл, който съдържа изпълнимия файл на инструмента за разполагане на Office (setup.exe) и примерен конфигурационен файл (configuration.xml).
  
 **За да изключите или премахнете приложенията на Microsoft 365 за корпоративни продукти от клиентски компютри:**
  
Когато инсталирате Приложения на Microsoft 365 за предприятия, можете да изключите определени продукти. За да направите това, следвайте стъпките за инсталиране на Office с ODT, но включете елемента ExcludeApp във вашия конфигурационен файл. Например този конфигурационен файл инсталира всички приложения на Microsoft 365 за корпоративни продукти с изключение на Publisher:
  
```
<Add SourcePath="\\Server\share" Version="15.1.2.3" OfficeClientEdition="32">
    <Product ID="O365ProPlusRetail" >
      <Language ID="en-us" />
      <ExcludeApp ID="Publisher" />
    </Product>
</Add>
```

[Общ преглед на инструмента за разполагане на Office](https://docs.microsoft.com/deployoffice/overview-office-deployment-tool)
  

