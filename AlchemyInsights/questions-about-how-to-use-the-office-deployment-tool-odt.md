---
title: Въпроси как да използвате инструмента за Office разполагане (ODT)
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
ms.openlocfilehash: d38866647c7bf286b5b5b21e7fdcc94af72ea1850bc40391af077aa230b8b4fd
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: bg-BG
ms.lasthandoff: 08/05/2021
ms.locfileid: "53959672"
---
# <a name="questions-about-how-to-use-the-office-deployment-tool-odt"></a>Въпроси как да използвате инструмента за Office разполагане (ODT)

Изтеглете инструмента за Office разполагане от центъра [на Microsoft за изтегляния.](https://go.microsoft.com/fwlink/p/?LinkID=626065)
  
След като изтеглите файла, изпълнете саморазархивиране на изпълнимия файл, който съдържа изпълнимия файл на инструмента за разполагане на Office (setup.exe) и примерен конфигурационен файл (configuration.xml).
  
 **За да изключите или премахнете Приложения на Microsoft 365 за предприятия продукти от клиентски компютри:**
  
Когато инсталирате Приложения на Microsoft 365 за предприятия, можете да изключите определени продукти. За да направите това, следвайте стъпките за Office с ODT, но включете елемента ExcludeApp във вашия конфигурационен файл. Например този конфигурационен файл инсталира всички Приложения на Microsoft 365 за предприятия, с изключение Publisher:
  
```
<Add SourcePath="\\Server\share" Version="15.1.2.3" OfficeClientEdition="32">
    <Product ID="O365ProPlusRetail" >
      <Language ID="en-us" />
      <ExcludeApp ID="Publisher" />
    </Product>
</Add>
```

[Общ преглед на инструмента Office разполагане](https://docs.microsoft.com/deployoffice/overview-office-deployment-tool)
  

