---
title: Конвертиране на пощенска кутия на потребител в споделената пощенска кутия?
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: reference
ms.service: o365-administration
localization_priority: Normal
ROBOTS: NOINDEX, NOFOLLOW
description: ''
ms.openlocfilehash: ab34b8939b95b29bedb797f640dd744bc783adef
ms.sourcegitcommit: 1d98db8acb9959aba3b5e308a567ade6b62da56c
ms.translationtype: MT
ms.contentlocale: bg-BG
ms.lasthandoff: 08/22/2019
ms.locfileid: "36496388"
---
# <a name="convert-a-user-mail-box-into-a-shared-mailbox"></a>Конвертиране на потребител пощенска кутия в споделена пощенска кутия

Можете да преобразувате само потребителска пощенска кутия към споделена пощенска кутия, ако потребителят има лиценз за обмен. След като пощенската кутия се конвертира, тя ще продължи да се появи в списъка на активните потребители, защото този списък включва споделени пощенски кутии. Обаче преобразувания пощенската кутия ще се появи в списъка на споделена пощенска кутия. 
  
Ако се опитате да преобразувате пощенска кутия в Exchange административната конзола и конвертирането не успее, изчистете кеша на браузъра и бисквитки и опитайте отново. Ако тя все още не работи, опитайте конвертиране на пощенската кутия в размяната управление на Шел като пуснете следната команда:
  
```
Set-Mailbox -Type Shared
```

Повече информация за преобразуване на пощенската кутия е наличен в [Конвертиране на потребителска пощенска кутия към споделена пощенска кутия](https://docs.microsoft.com/office365/admin/email/convert-user-mailbox-to-shared-mailbox).
  
