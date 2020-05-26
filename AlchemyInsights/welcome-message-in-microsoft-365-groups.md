---
title: Приветствено съобщение в групи на Microsoft 365
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "1200024"
- "5685"
ms.openlocfilehash: d82931ae6978a09e674b00640d1dd413bcce7cfd
ms.sourcegitcommit: b196100759b29aecd62b693a2bfedbbd25a697c6
ms.translationtype: MT
ms.contentlocale: bg-BG
ms.lasthandoff: 05/19/2020
ms.locfileid: "44357322"
---
# <a name="welcome-message-in-microsoft-365-groups"></a>Приветствено съобщение в групи на Microsoft 365

Нови потребители присъединяване към Microsoft 365 група ще получите имейл, ако свойството "UnifiedGroupWelcomeMessageEnabled" е вярно.

В случай, че искате да забраните приветстваното съобщение, използвайте следната [команда EXO PowerShell:](https://docs.microsoft.com/powershell/exchange/exchange-online/exchange-online-powershell-v2/exchange-online-powershell-v2?view=exchange-ps)

`
Set-UnifiedGroup <groupname> -UnifiedGroupWelcomeMessageEnabled:$False
`
