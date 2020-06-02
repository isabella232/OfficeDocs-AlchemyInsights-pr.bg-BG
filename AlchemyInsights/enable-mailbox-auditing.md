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
ms.openlocfilehash: 2bcfb7cc174cd58b21e1bb0c82f0d7cdb25e2fdd
ms.sourcegitcommit: bc7d6f4f3c9f7060d073f5130e1ec856e248d020
ms.translationtype: MT
ms.contentlocale: bg-BG
ms.lasthandoff: 06/02/2020
ms.locfileid: "44506943"
---
# <a name="enable-mailbox-auditing"></a>Разрешаване на проверка на пощенска кутия

За да разрешите проверка на пощенска кутия за един потребител или цялата организация следните кратки команди трябва да се изпълняват от отдалечената обвивка на захранването:
  
 **Един потребител**
  
Задаване на пощенска кутия -самоличност "Джейн Дау" -ОдитEnabled $true
  
 **Организация**
  
Вземи-пощенска кутия -ResultSize неограничен -филтър {RecipientTypeДетайли-eq "UserMailbox"} | Задаване на пощенска кутия -Auditenabled $true
  
[Научете повече](https://docs.microsoft.com/microsoft-365/compliance/enable-mailbox-auditing)
  

