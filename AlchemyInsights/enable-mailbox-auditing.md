---
title: Разрешаване на проверка на пощенска кутия
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: 19997b0a-394f-4943-8908-c601696a332c
ms.openlocfilehash: ae11d6be0789a5662d202b85268480a3d42922c4
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: bg-BG
ms.lasthandoff: 04/22/2020
ms.locfileid: "43703560"
---
# <a name="enable-mailbox-auditing"></a>Разрешаване на проверка на пощенска кутия

За да разрешите проверка на пощенска кутия за един потребител или цялата организация, трябва да се изпълняват следните кратки команди от отдалечен power Shell:
  
 **Единичен потребител**
  
Задаване-пощенска кутия -самоличност "Джейн Доу" -auditEnabled $true
  
 **Организация**
  
Get-пощенска кутия -Резултат неограничен -Филтър {RecipientTypeDetails -eq "UserMailbox"} | Set-пощенска кутия -ПроверкаEnabled $true
  
[Научете повече](https://docs.microsoft.com/office365/securitycompliance/enable-mailbox-auditing)
  

