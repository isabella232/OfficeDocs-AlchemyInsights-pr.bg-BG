---
title: Отказан достъп при преглед на работен поток
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 47ceb983-f9a4-4c55-a40c-03d5c3d75dc9
ms.openlocfilehash: 710775e8b2dee98969df7a4c8410a3e61181aaf6
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: bg-BG
ms.lasthandoff: 09/14/2020
ms.locfileid: "47688791"
---
# <a name="access-denied-when-viewing-a-workflow"></a>Отказан достъп при преглед на работен поток

Работните потоци на SharePoint 2013, които се опитват да изпратят имейл до група на SharePoint, може да не успеят с съобщение за грешка "отказан достъп", ако членството в групата на SharePoint не е зададено на всеки.
  
 **За да отстраните този проблем, изпълнете следните стъпки:**
  
 1. Позволете на всички да виждат членовете на групата на SharePoint.
  
 2. Премахнете групата на SharePoint от реда "до" или "Як" на имейла.
  
 3. Изрично добавете потребителите към реда "до" или "Як", ако видимостта на членството не може да бъде променена за групата на SharePoint.
  
За да видите повече подробности, вижте [http неоторизирани за/_vti_bin/client.SVC/SP.Utilities.Utility.SendEmail](https://go.microsoft.com/fwlink/?linkid=2044694&amp;clcid=0x409).
  