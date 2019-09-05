---
title: Разрешаване на проверка на пощенската кутия
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 4/5/2018
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: 19997b0a-394f-4943-8908-c601696a332c
ms.openlocfilehash: 73517f46935a67a4a8a3e4770090ac897fe67979
ms.sourcegitcommit: a256e8680379c006287ae30996763051c4d9ff85
ms.translationtype: MT
ms.contentlocale: bg-BG
ms.lasthandoff: 09/04/2019
ms.locfileid: "36736242"
---
# <a name="enable-mailbox-auditing"></a>Разрешаване на проверка на пощенската кутия

За да разрешите проверка на пощенската кутия за един потребител или цяла организация следните кратки команди трябва да се изпълняват от отдалечената Power Shell:
  
 **Единичен потребител**
  
Set-пощенска кутия-идентичност "Jane Dow"-Аудиоled $true
  
 **Организация**
  
Get-пощенска кутия Резултитразмер неограничен-филтър {РеЦипиенттипедетаилс-EQ "UserMailbox кутия"} | Set-пощенска кутия-Аудиоled $true
  
[Научете повече](https://docs.microsoft.com/office365/securitycompliance/enable-mailbox-auditing)
  

