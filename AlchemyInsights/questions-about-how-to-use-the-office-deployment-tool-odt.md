---
title: Въпроси как да използвате инструмента за разполагане на Office (ODT)
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 3e88e0f3-c86d-4ab8-b076-59d0552318f9
ms.openlocfilehash: e9f7581fd21cf5ca2d712038c4b73b67d08f3a76
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: bg-BG
ms.lasthandoff: 09/15/2020
ms.locfileid: "47774880"
---
# <a name="questions-about-how-to-use-the-office-deployment-tool-odt"></a>Въпроси как да използвате инструмента за разполагане на Office (ODT)

Изтеглете инструмента за разполагане на Office от [центъра на Microsoft за изтегляния](https://go.microsoft.com/fwlink/p/?LinkID=626065).
  
След изтеглянето на файла изпълнете самостоятелно извлечения изпълним файл, който съдържа изпълнимия инструмент за разполагане на Office (setup.exe) и примерен конфигурационен файл (configuration.xml).
  
 **За да изключите или премахнете приложенията на Microsoft 365 за корпоративни продукти от клиентски компютри:**
  
Когато инсталирате приложения на Microsoft 365 за Enterprise, можете да изключвате определени продукти. За да направите това, следвайте стъпките за инсталиране на Office със ODT, но включете елемента ExcludeApp във вашия конфигурационен файл. Например този конфигурационен файл инсталира всички приложения на Microsoft 365 за корпоративни продукти, с изключение на Publisher:
  
```
<Add SourcePath="\\Server\share" Version="15.1.2.3" OfficeClientEdition="32">
    <Product ID="O365ProPlusRetail" >
      <Language ID="en-us" />
      <ExcludeApp ID="Publisher" />
    </Product>
</Add>
```

[Общ преглед на инструмента за разполагане на Office](https://docs.microsoft.com/deployoffice/overview-office-deployment-tool)
  

