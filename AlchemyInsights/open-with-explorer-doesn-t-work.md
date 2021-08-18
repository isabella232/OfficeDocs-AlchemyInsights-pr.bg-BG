---
title: Отварянето с Explorer не работи
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
ms.assetid: b8f07022-69fe-4112-a2f6-d3a6cedb966c
ms.openlocfilehash: 2ba6f08b40dd194bf1ffd9a455a134a2fc553b51
ms.sourcegitcommit: ab75f66355116e995b3cb5505465b31989339e28
ms.translationtype: MT
ms.contentlocale: bg-BG
ms.lasthandoff: 08/13/2021
ms.locfileid: "58321850"
---
# <a name="open-with-explorer-isnt-working"></a>Отварянето с Explorer не работи

Ако **Отваряне с Explorer или** Изглед във **файловия мениджър** не работи, уверете се, че услугата WebClient е зададена на **Изпълняване,** като следвате стъпките по-долу. Например може да отнеме много време, за да отворите SharePoint или OneDrive, когато услугата не се изпълнява. 
  
1. В полето Windows за търсене въведете изпълнение, изберете изпълни настолното приложение, въведете services.msc и след това **изберете Enter**.
    
2. Превъртете надолу до услугата WebClient и проверете **колоната** Състояние. Ако състоянието на услугата WebClient не се **изпълнява**, щракнете двукратно върху услугата, щракнете **върху Старт** и след това щракнете върху **OK**. Разрешете услугата, ако е необходимо, като изберете **Ръчно** или **Автоматично** в **полето Тип стартиране.** 
    
**Забележка:** За отстраняване на проблеми при отваряне във файловия мениджър вижте [Отваряне в Explorer](https://go.microsoft.com/fwlink/?linkid=871665). Разгледайте синхронизирането като по-добра [алтернатива: Синхронизиране SharePoint файлове с новия OneDrive Sync клиент.](https://go.microsoft.com/fwlink/?linkid=871666) 
  

