---
title: Отваряне с Explorer не работи
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
ms.openlocfilehash: 5bf28982533d8ca9998605cf3592f317c0ef99b0
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: bg-BG
ms.lasthandoff: 09/14/2020
ms.locfileid: "47694445"
---
# <a name="open-with-explorer-isnt-working"></a>Отваряне с Explorer не работи

Ако **отворен с Explorer** или **изглед във File Explorer** не работи, уверете се, че услугата WebClient е настроена да се **изпълнява** , като следвате стъпките по-долу. Например може да отнеме много време, за да отворите библиотека на SharePoint или OneDrive, когато услугата не се изпълнява. 
  
1. В полето за търсене на Windows въведете Run, изберете изпълнение на настолното приложение, въведете Services. msc и след това изберете **Enter**.
    
2. Превъртете надолу до WebClient услугата и проверете колоната **състояние** . Ако състоянието на услугата WebClient не се **изпълнява**, щракнете двукратно върху услугата, изберете **Старт**и след това щракнете върху **OK**. Разрешете услугата, ако е необходимо, като изберете **ръчна** или **Автоматична** в полето **тип на стартиране** . 
    
> [!NOTE]
> За отстраняване на проблеми при отваряне във File Explorer вижте [Отваряне в Explorer](https://go.microsoft.com/fwlink/?linkid=871665). Изследвайте синхронизирането като по-добра алтернатива: [Синхронизиране на файлове на SharePoint с новия клиент за синхронизиране на OneDrive](https://go.microsoft.com/fwlink/?linkid=871666). 
  

