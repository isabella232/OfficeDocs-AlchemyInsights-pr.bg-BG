---
title: Отстраняване на проблеми с помощта на Open with Explorer
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
ms.openlocfilehash: 0cbcfb506295d5732f7109be7a103bbdef530a529c7408c6d9d45a7b38a89915
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: bg-BG
ms.lasthandoff: 08/05/2021
ms.locfileid: "54048145"
---
# <a name="fix-problems-with-open-with-explorer"></a>Коригиране на проблеми с "Отвори с Explorer"

Коригиране на често срещани проблеми с отварянето на библиотека с документи SharePoint или OneDrive с помощта **на командата Отвори с Explorer:** 
  
- Използвайте Internet Explorer 10 или Internet Explorer 11. **Отварянето с Explorer** не е съвместимо с Microsoft Edge, Google Chrome, Firefox и други. **Отварянето с Explorer** е забранено във всички браузъри, с изключение на Internet Explorer. 
    
- **Отварянето с Explorer** не е налично в модерната работа за SharePoint библиотеки. Вместо **това използвайте изглед във файловия** мениджър. Изберете **Преглед на** \> **опциите Изглед във файловия мениджър**. Изгледът във Файловия мениджър не е съвместим с Microsoft Edge, Google Chrome, Firefox и други. **Преглед във файловия мениджър,** наличен само в Internet Explorer. 
    
- Уверете се, че се изпълнява услугата WebClient. В полето Windows за търсене въведете изпълнение, изберете приложението Изпълнение на работния плот, въведете services.msc и след това натиснете Enter. Превъртете надолу до услугата WebClient и се уверете, **че колоната Състояние** показва "Изпълнява се". Ако това не стане, щракнете двукратно върху услугата, щракнете върху **Старт** и след това щракнете върху **OK**. (Може да се наложи първо да разрешите услугата, като изберете Ръчно **или** **Автоматично** в полето **Тип стартиране.)** 
    
> [!NOTE]
> Отварянето на библиотека във файловия мениджър е удобно, ако трябва да копирате или преместите няколко файла и папки веднъж, но ако искате редовно да работите в библиотеката, ви препоръчваме да я синхронизирате. За отстраняване на проблеми при отваряне във файловия мениджър вижте [Отваряне в Explorer](https://go.microsoft.com/fwlink/?linkid=871665). За информация относно настройването на синхронизирането вижте [Синхронизиране SharePoint файлове с новия OneDrive Sync клиент.](https://go.microsoft.com/fwlink/?linkid=871666)
  
Вижте статията Как [да използвате командата "Отвори с Explorer", за](https://docs.microsoft.com/sharepoint/support/lists-and-libraries/troubleshoot-issues-using-open-with-explorer) да отстранявате проблеми в SharePoint онлайн за повече информация. 
  

