---
title: Отваряне с Explorer не работи
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
ms.assetid: b8f07022-69fe-4112-a2f6-d3a6cedb966c
ms.openlocfilehash: 73d33e50449345c312abdd39afcc36e0c95fd1c4
ms.sourcegitcommit: 9d78905c512192ffc4675468abd2efc5f2e4baf4
ms.translationtype: MT
ms.contentlocale: bg-BG
ms.lasthandoff: 04/23/2019
ms.locfileid: "32419851"
---
# <a name="open-with-explorer-isnt-working"></a>Отваряне с Explorer не работи

Ако **Отваряне с Explorer** или **мнение в File Explorer** не работи се уверете, че услугата на WebClient е настроен да **работи** като следвате стъпките по-долу. Например това може да отнеме дълго време за отваряне на SharePoint или OneDrive Библиотека, когато услугата не се изпълнява. 
  
1. В Windows полето за търсене въведете тичам, изберете Run работния плот ап, вид services.msc и след това изберете **Enter**.
    
2. Превъртете надолу до услугата на WebClient и проверете колоната **състояние** . Ако състоянието на WebClient услуга не се **изпълнява**, щракнете двукратно върху услугата, щракнете върху **Старт**и след това щракнете върху **OK**. Разреши услугата, ако е необходимо, избирайки или **ръчно** или **автоматично** в полето **тип на стартиране** . 
    
> [!NOTE]
> За да отстраните проблеми с отварянето в File Explorer, вижте [отворен in Изследовател](https://go.microsoft.com/fwlink/?linkid=871665). Разгледайте синхронизация като по-добра алтернатива: [файлове за синхронизиране на SharePoint с новия клиент, OneDrive синхронизиране](https://go.microsoft.com/fwlink/?linkid=871666). 
  

