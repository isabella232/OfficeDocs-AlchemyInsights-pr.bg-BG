---
title: Разреши проверка на пощенска кутия
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 4/5/2018
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom: Adm_O365
ms.assetid: 19997b0a-394f-4943-8908-c601696a332c
ms.openlocfilehash: bd94ec10f9df2e72ec6e3d8552d2eb80212a9d78
ms.sourcegitcommit: d6ea5e9458a2b8ceaab3ac4bd483e1130b9a398a
ms.translationtype: MT
ms.contentlocale: bg-BG
ms.lasthandoff: 01/15/2019
ms.locfileid: "28275519"
---
# <a name="enable-mailbox-auditing"></a>Разреши проверка на пощенска кутия

За да разрешите проверка на пощенска кутия за единичен потребител или цялата организация следните кратки команди трябва да се управлява от дистанционно Power Shell:
  
 **Единичен потребител**
  
Set-пощенска кутия - идентичност "Джейн Доу" - AuditEnabled на $true
  
 **Organization**
  
Махни-пощенска кутия - ResultSize неограничен - филтър {RecipientTypeDetails - eq "UserMailbox"} | Set-пощенска кутия - AuditEnabled $true
  
[Научете повече](https://support.office.com/article/aaca8987-5b62-458b-9882-c28476a66918)
  

