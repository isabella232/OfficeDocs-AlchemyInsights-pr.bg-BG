---
title: Липсващ работен поток не успя да се активира
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: e46ae8c5-3d81-457e-8c77-f7c1cbe267c4
ms.openlocfilehash: d703e87f355f05bf4a1d71e5daddce96db988380bb48accc81c95f1ba91fbb2b
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: bg-BG
ms.lasthandoff: 08/05/2021
ms.locfileid: "54065417"
---
# <a name="missing-workflow-failed-to-activate"></a>Липсващ работен поток не успя да се активира

В колекция от SharePoint на Microsoft не можете да добавите глобално използваем работен поток (например "Одобрение – SharePoint 2010") към списък или библиотека.
  
За да разрешите този проблем, изпълнете следните стъпки: 
  
1. Отворете главния уеб сайт на колекцията от сайтове в SharePoint Designer 2013.
  
2. Под **Обекти на сайта** изберете Работни **потоци**. 
  
3. В **секцията Нов** на лентата **Работни потоци** изберете **Повторно използваем работен поток**. 
  
4. Във формуляра **Създаване на работен поток за многоизползване** въведете името ** *Поправка2010* **. За **Тип платформа** щракнете върху SharePoint **2010 работен поток** и след това щракнете върху **OK**. 
  
1. В **секцията Запиши** на лентата **на работния** поток изберете **Публикуване**. 
  
2. В **секцията** Управление на лентата **на работния** поток изберете **Публикуване глобално**. В диалоговия прозорец за потвърждение, който се появява, **изберете OK**. 
  
3. В уеб браузър намерете главния уеб сайт на колекцията от сайтове и след това достъп до функциите на **Настройки** \> **на колекция от сайтове**. След това превключвайте функцията **"Работни потоци":** 
  
· Ако функцията е  *активирана, щракнете върху*  Дезактивирай **и** след това щракнете **върху Активирай**. 
  
· Ако функцията е  *дезактивирана,*  щракнете върху **Активиране**. 
  
За повече информация вижте следната [статия.](https://go.microsoft.com/fwlink/?linkid=2047770&amp;clcid=0x409)
  

