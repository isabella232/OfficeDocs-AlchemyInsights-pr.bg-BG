---
title: Използване на инструмента Office разполагане
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "918"
- "2000022"
ms.assetid: 7ff7cc06-76d0-468f-bd66-3f2760750d04
ms.openlocfilehash: 39a011d4b121492d222ff620e70d9860231b7bcfe0d7fd2ecfd93de1ef502f5f
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: bg-BG
ms.lasthandoff: 08/05/2021
ms.locfileid: "54083759"
---
# <a name="using-the-office-deployment-tool-odt"></a>Използване на Office за разполагане (ODT)

Можете да използвате Office за разполагане (ODT), за да разположите Office 365 версии на Office. Инструментът Office разполагане (setup.exe) се изпълнява от командния ред и използва XML файл за конфигуриране, за да определи какви настройки да се прилагат при разполагане на Office.
  
1. Изтеглете най-новата версия на инструмента Office разполагане от центъра [на Microsoft за изтегляния.](https://go.microsoft.com/fwlink/p/?LinkID=626065)

2. Използвайте инструмента [Office за персонализиране (OCT), за](https://config.office.com) да изберете предпочитанията си за разполагане и да създадете XML файла за конфигуриране. Експортирайте конфигурационния файл и го поставете локално в същата папка, където setup.exe се намира.

    **Забележка:** Office често възникват проблеми при инсталиране поради неправилно конфигурирани или малформатирани конфигурационни файлове. За да избегнете подобни проблеми, ви препоръчваме да използвате инструмента Office персонализиране, за да създадете конфигурационния файл. Можете също да импортирате съществуващи конфигурационни файлове в инструмента Office персонализиране.

3. От команден прозорец с повишени права превключете към местоположението, където setup.exe се намира, и изпълнете инструмента за разполагане на Office в режим на изтегляне и задайте конфигурационния файл, който току-що записахте. В този пример конфигурационният файл се нарича Configuration.xml:

```setup.exe /download Configuration.xml```

4.Изпълнете инструмента Office разполагане в режим на конфигуриране и задайте конфигурационния файл.

```setup.exe /configure Configuration.xml```

**Забележка:** Трябва да изпълните тази стъпка от клиентския компютър, на който искате да инсталирате Office и трябва да имате разрешения на локален администратор на този компютър.

За да научите повече за използването Office за разполагане на Приложения на Microsoft 365 за предприятия сценарии за разполагане, вижте Общ [преглед на Office за разполагане.](https://docs.microsoft.com/deployoffice/overview-office-deployment-tool) За повече подробности как да използвате инструмента Office персонализиране вижте Общ [преглед на инструмента за Office персонализиране.](https://docs.microsoft.com/DeployOffice/overview-of-the-office-customization-tool-for-click-to-run)
