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
# <a name="using-the-office-deployment-tool-odt"></a>С помощта на Office разполагане инструмент (ODT)

Използвайте Office разгръщане оръдие (ODT) да разположат Office 365 версии на Office. Инструмент за разгръщане служба (setup.exe) се управлява от командния ред и използва конфигурация XML файл, за да определи кои настройки да приложите при разполагането на Office.
  
1. Изтеглете най-новата версия на инструмента за разполагане на Office от [Microsoft Download център](http://go.microsoft.com/fwlink/p/?LinkID=626065).

2. Използвайте [Office Customization Tool (OCT)](https://config.office.com) да изберете предпочитанията си за разполагане и създаване на конфигурационния XML файл. Експортиране на конфигурационния файл и го поставете локално в същата папка, където пребивава setup.exe.

    **Забележка:** Инсталирането на Office, често възникнат проблеми поради на липсващ или malformatted конфигурационни файлове. За да се избегнат такива проблеми, ви препоръчваме да използвате инструмента за персонализиране на Office за създаване на конфигурационния файл. Също така можете да импортирате съществуващи конфигурационни файлове в Office Customization Tool.

3. От издигам заповядвам бърз шибалка към мястото, където пребивава setup.exe и изпълнение на инструмента за разполагане на Office в режим на изтегляне и зададете в конфигурационния файл, който току-що записахте. В този пример конфигурационния файл е с име Configuration.xml:
    
  ```
  setup.exe /download Configuration.xml  
  ```

4. Изпълнете инструмента за разполагане на Office в режим на конфигуриране и задайте конфигурационния файл.
    
  ```
  setup.exe /configure Configuration.xml
  ```

    **Забележка:** Трябва да изпълните тази стъпка от на клиентския компютър, на който искате да инсталирате Office и трябва да имате разрешения на локален администратор на този компютър.

За да научите повече за използването на инструмента за внедряване на Office вашите Office 365 подпора за сценарии за разгръщане, вижте [Обзор на инструмента за разполагане на Office](https://docs.microsoft.com/deployoffice/overview-of-the-office-2016-deployment-tool). За повече подробности за това как да използвате инструмента за персонализиране на Office вижте [Обзор на инструмента за персонализиране на Office](https://docs.microsoft.com/DeployOffice/overview-of-the-office-customization-tool-for-click-to-run).
