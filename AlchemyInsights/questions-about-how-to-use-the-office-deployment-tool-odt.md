---
title: Въпроси за това как да използвате Office разгръщане оръдие (ODT)
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 4/26/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 3e88e0f3-c86d-4ab8-b076-59d0552318f9
ms.openlocfilehash: e91d40f872dd401ee210ac05eb39d64b6fb88027
ms.sourcegitcommit: dd43cc0a9470f98b8ef2a3787c823801d674c666
ms.translationtype: MT
ms.contentlocale: bg-BG
ms.lasthandoff: 02/12/2019
ms.locfileid: "29925333"
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
  

