---
title: Отстраняване на проблеми с помощта на Open с Explorer
ms.author: toresing
author: tomresing
manager: scotv
ms.date: 12/10/2018
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: ed852342-e33f-4450-8400-63d30df09476
ms.openlocfilehash: a9ab7dd27e4dc1bd76c93cc81260616063e638ed
ms.sourcegitcommit: a256e8680379c006287ae30996763051c4d9ff85
ms.translationtype: MT
ms.contentlocale: bg-BG
ms.lasthandoff: 09/04/2019
ms.locfileid: "36742722"
---
# <a name="fix-problems-with-open-with-explorer"></a>Отстраняване на проблеми с Open с Explorer

Отстраняване на често срещани проблеми с отварянето на библиотека с документи в SharePoint или OneDrive с помощта на командата **Open с Explorer** : 
  
- Използвайте Internet Explorer 10 или Internet Explorer 11. **Open с Explorer** не е съвместим с Microsoft Edge, Google Chrome, Firefox и други. **Open с Explorer** е забранена във всички браузъри с изключение на Internet Explorer. 
    
- **Open с Explorer** не е наличен в съвременното преживяване за библиотеките на SharePoint. Вместо това използвайте **изглед във файловия мениджър** . Изберете изглед на **Опции** \> **за изглед във файловия мениджър**. Изгледът във файловия мениджър не е съвместим с Microsoft Edge, Google Chrome, Firefox и други. **Преглед във файловия мениджър** в наличен само в Internet Explorer. 
    
- Уверете се, че услугата WebClient се изпълнява. В полето за търсене на Windows въведете Run, изберете изпълнение на настолното приложение, въведете Services. msc и след това натиснете ENTER. Превъртете надолу до услугата WebClient и се уверете, че колоната **състояние** показва "изпълнение". Ако не, щракнете двукратно върху услугата, щракнете върху **старти**след това щракнете върху **OK**. (Може да се наложи първо да разрешите услугата, като изберете **ръчно** или **автоматично** в полето **тип стартиране** .) 
    
> [!NOTE]
> Отварянето на библиотека във файловия мениджър е удобно, ако трябва да копирате или премествате няколко файла и папки веднъж, но ако искате да работите редовно в библиотеката, ви препоръчваме да го синхронизирате. За отстраняване на проблеми при отваряне на файловия мениджър вижте [Отваряне в Explorer](https://go.microsoft.com/fwlink/?linkid=871665). За информация относно настройването на синхронизацията вижте [Синхронизиране на SharePoint файлове с новия OneDrive синхронизиране на клиента](https://go.microsoft.com/fwlink/?linkid=871666).
  
Моля, вижте статията [как да използвате командата "отвори с Explorer" за отстраняване на проблеми в SharePoint online](https://docs.microsoft.com/sharepoint/support/lists-and-libraries/troubleshoot-issues-using-open-with-explorer) за повече информация. 
  

