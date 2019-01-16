---
title: Въпроси за това как да използвате Office разгръщане оръдие (ODT)
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 4/26/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.assetid: 3e88e0f3-c86d-4ab8-b076-59d0552318f9
ms.openlocfilehash: c16b7ac7d79794307fa33ed1039305ed5b842cf6
ms.sourcegitcommit: d6ea5e9458a2b8ceaab3ac4bd483e1130b9a398a
ms.translationtype: MT
ms.contentlocale: bg-BG
ms.lasthandoff: 01/15/2019
ms.locfileid: "28275526"
---
# <a name="questions-about-how-to-use-the-office-deployment-tool-odt"></a>Въпроси за това как да използвате Office разгръщане оръдие (ODT)

Изтеглете инструмента за внедряване на Office от [Microsoft Download център](http://go.microsoft.com/fwlink/p/?LinkID=626065).
  
След свалянето на файла, стартирайте самоизвличащия изпълнимия файл, който съдържа Office разгръщане оръдие изпълним (setup.exe) и примерен конфигурационен файл (configuration.xml).
  
 **За да изключите или премахнете Office 365 подпора продукти от клиентските компютри:**
  
Когато инсталирате Office 365 подпора, можете да изключите специфични продукти. За да направите това, следвайте стъпките за инсталиране на Office с ODT, но включват ExcludeApp елемент в конфигурационния файл. За пример този конфигурационен файл се инсталира всички Office 365 подпора продукти с изключение на Издател:
  
```
<Add SourcePath="\\Server\share" Version="15.1.2.3" OfficeClientEdition="32">
    <Product ID="O365ProPlusRetail" >
      <Language ID="en-us" />
      <ExcludeApp ID="Publisher" />
    </Product>
</Add>
```

[Обзор на инструмента за разполагане на Office](https://docs.microsoft.com/deployoffice/overview-of-the-office-2016-deployment-tool)
  

