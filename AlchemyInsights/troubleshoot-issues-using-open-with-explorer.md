---
title: Отстраняване на проблеми с помощта на "отваряне с Explorer"
ms.author: toresing
author: tomresing
manager: scotv
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: ed852342-e33f-4450-8400-63d30df09476
ms.openlocfilehash: e7fe59b94d216d89c2f2f7100a3d8bf7a0b0196e
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: bg-BG
ms.lasthandoff: 09/14/2020
ms.locfileid: "47659047"
---
# <a name="fix-problems-with-open-with-explorer"></a>Отстраняване на проблеми с "отваряне с Explorer"

Коригиране на често срещани проблеми при отваряне на библиотека с документи в SharePoint или OneDrive с помощта на командата " **Отваряне с Explorer** ": 
  
- Използвайте Internet Explorer 10 или Internet Explorer 11. **Отварянето с Explorer** не е съвместимо с Microsoft Edge, Google Chrome, Firefox и други. **Отваряне с Explorer** е забранено във всички браузъри, с изключение на Internet Explorer. 
    
- Опцията " **Отваряне с Explorer** " не е налична в съвременната среда за библиотеки на SharePoint. Вместо това използвайте **изгледа във File Explorer** . Изберете изглед на **Опции** \> **за преглед във файловия мениджър**. Изгледът във File Explorer не е съвместим с Microsoft Edge, Google Chrome, Firefox и други. Можете да **преглеждате файловия мениджър** само в Internet Explorer. 
    
- Уверете се, че услугата WebClient се изпълнява. В полето за търсене на Windows въведете Run, изберете изпълнение на настолното приложение, въведете Services. msc и след това натиснете клавиша ENTER. Превъртете надолу до услугата WebClient и се уверете, че колоната **състояние** показва "изпълнява се." Ако не е, щракнете двукратно върху услугата, щракнете върху **Старт**, след което щракнете върху **OK**. (Може да се наложи първо да разрешите услугата, като изберете **ръчна** или **Автоматична** в полето **тип стартиране** .) 
    
> [!NOTE]
> Отварянето на библиотека във файловия мениджър е удобно, ако трябва да копирате или да местите няколко файла и папки веднъж, но ако искате да работите редовно в библиотеката, ви препоръчваме да го синхронизирате. За отстраняване на проблеми при отваряне във File Explorer вижте [Отваряне в Explorer](https://go.microsoft.com/fwlink/?linkid=871665). За информация относно настройването на синхронизирането вижте [Синхронизиране на файлове на SharePoint с новия клиент за синхронизиране на OneDrive](https://go.microsoft.com/fwlink/?linkid=871666).
  
Вижте статията [как да използвате командата "отваряне с Explorer", за да отстранявате проблеми в SharePoint online](https://docs.microsoft.com/sharepoint/support/lists-and-libraries/troubleshoot-issues-using-open-with-explorer) за повече информация. 
  

