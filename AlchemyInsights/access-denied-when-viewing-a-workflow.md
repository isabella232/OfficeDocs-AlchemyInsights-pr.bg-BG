---
title: Достъпът е отказан, когато преглеждате работен поток
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 47ceb983-f9a4-4c55-a40c-03d5c3d75dc9
ms.openlocfilehash: 2b076ec5dca070555ce51b88631fb6bd619ed9269e59ccc799b23b8b95547c16
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: bg-BG
ms.lasthandoff: 08/05/2021
ms.locfileid: "53955190"
---
# <a name="access-denied-when-viewing-a-workflow"></a>Достъпът е отказан, когато преглеждате работен поток

SharePoint 2013 работни потоци, които се опитват да изпратят имейл до група на SharePoint, могат да не успеят със съобщение за грешка "Отказан достъп", ако членството в групата SharePoint не е зададено на "Всеки".
  
 **За да разрешите този проблем, изпълнете следните стъпки:**
  
 1. Позволете на всички да виждат членовете на SharePoint група.
  
 2. Премахнете групата SharePoint от реда До или ЯК на имейла.
  
 3. Изрично добавете потребителите към реда До или ЯК, ако видимостта на членството не може да бъде променена за SharePoint група.
  
За да видите повече подробности, вижте HTTP Неупълномощено на [/_vti_bin/client.svc/sp.utilities.utility.SendEmail](https://go.microsoft.com/fwlink/?linkid=2044694&amp;clcid=0x409).
  