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
ms.sourcegitcommit: e2864efcfb493b6e46b662b746661a61232bdba7
ms.translationtype: MT
ms.contentlocale: bg-BG
ms.lasthandoff: 01/24/2019
ms.locfileid: "29500271"
---
# <a name="enable-mailbox-auditing"></a>Разреши проверка на пощенска кутия

За да разрешите проверка на пощенска кутия за единичен потребител или цялата организация следните кратки команди трябва да се управлява от дистанционно Power Shell:
  
 **Единичен потребител**
  
Set-пощенска кутия - идентичност "Джейн Доу" - AuditEnabled на $true
  
 Organization
  
Махни-пощенска кутия - ResultSize неограничен - филтър {RecipientTypeDetails - eq "UserMailbox"} | Set-пощенска кутия - AuditEnabled $true
  
Научете повече
  

