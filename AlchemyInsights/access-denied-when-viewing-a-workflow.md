---
title: Достъпът е отказан при преглед на работен поток
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 47ceb983-f9a4-4c55-a40c-03d5c3d75dc9
ms.openlocfilehash: c576bf88225582f2577e0b59506a7482cf9f38d5
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: bg-BG
ms.lasthandoff: 04/22/2020
ms.locfileid: "43687319"
---
# <a name="access-denied-when-viewing-a-workflow"></a>Достъпът е отказан при преглед на работен поток

SharePoint 2013 работни потоци, които се опитват да изпратите имейл до група на SharePoint може да се провали с съобщение за грешка "Достъпът е отказан", ако членството на групата на SharePoint не е зададена на всеки.
  
 **За да разрешите този проблем, направете следните стъпки:**
  
 1. Позволявана на всички да виждат членовете на групата на SharePoint.
  
 2. Премахнете групата на SharePoint от реда до или як на имейла.
  
 3. Изрично добавете потребителите към или як ред, ако не може да се промени членството за SharePoint група.
  
За да видите повече подробности, моля, вижте [HTTP Неоторизиран достъп до /_vti_bin/client.svc/sp.utilities.utility.SendEmail](https://go.microsoft.com/fwlink/?linkid=2044694&amp;clcid=0x409).
  