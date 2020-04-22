---
title: Отваряне с Explorer не работи
ms.author: toresing
author: tomresing
manager: scotv
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: b8f07022-69fe-4112-a2f6-d3a6cedb966c
ms.openlocfilehash: dc939a3451ff4fe95e4aa5a999839a2c532b398c
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: bg-BG
ms.lasthandoff: 04/22/2020
ms.locfileid: "43713023"
---
# <a name="open-with-explorer-isnt-working"></a>Отваряне с Explorer не работи

Ако **отворете с Explorer** или изглед във **файловия мениджър** не работи уверете се, че уебклиент услугата е настроена на **изпълнява,** като следвате стъпките по-долу. Например може да отнеме много време, за да отворите библиотека на SharePoint или OneDrive, когато услугата не се изпълнява. 
  
1. В полето за търсене на Windows въведете изпълнение, изберете изпълнение на десктоп приложение, въведете services.mscи след това изберете **Enter**.
    
2. Превъртете надолу до услугата WebClient и проверете **колоната състояние.** Ако състоянието на услугата WebClient не се **изпълнява**, щракнете двукратно върху услугата, щракнете върху **Старт**и след това щракнете върху **OK**. Активирайте услугата, ако е необходимо, като изберете **ръчно** или **автоматично** в полето **Тип стартиране** . 
    
> [!NOTE]
> За отстраняване на проблеми при отваряне във файловия мениджър, вижте [Отвори в Explorer](https://go.microsoft.com/fwlink/?linkid=871665). Разгледайте синхронизирането като по-добра алтернатива: [Синхронизиране на SharePoint файлове с новия oneDrive синхронизиране клиент](https://go.microsoft.com/fwlink/?linkid=871666). 
  

