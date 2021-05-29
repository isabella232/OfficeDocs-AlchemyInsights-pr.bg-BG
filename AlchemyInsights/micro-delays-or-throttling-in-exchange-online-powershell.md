---
title: Микро закъснения или ограничаване на PowerShell в Exchange Online
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "3500011"
- "5106"
ms.openlocfilehash: 204e0248bc2f07f14fa789d1d2999495910ee034
ms.sourcegitcommit: d2108b13acc44e26b65f9a2739cbce9bf98959a5
ms.translationtype: MT
ms.contentlocale: bg-BG
ms.lasthandoff: 05/28/2021
ms.locfileid: "52702115"
---
# <a name="micro-delays-or-throttling-in-exchange-online-powershell"></a>Микро закъснения или ограничаване на PowerShell в Exchange Online

Възможно е да видите предупреждения за "Приложено микро забавяне" или закъснения, когато изпълнявате скриптове и кратки команди в Exchange Online. Ето няколко предложения как да решите това:

- Изпълнете нашата диагностика, за да отпуснете правилата за ограничаване на PowerShell на вашия клиент. Това решение ще реши проблема за повечето.
- Ако проблемът все още не е решен, използвайте [модула Exchange Online v2 PowerShell](/powershell/exchange/exchange-online/exchange-online-powershell-v2/exchange-online-powershell-v2?view=exchange-ps&preserve-view=true), който включва CMDlets, които са базирани на REST API и са значително по-изпълняващи. Това може да бъде чудесно решение за много от често използваните кратки команди.
- Ако трябва да използвате КРАТКИ КОМАНДИ, които не са включени в модула v2, вижте Изпълняване на кратки команди на PowerShell за голям брой потребители в Office 365 , което говори как да заобиколите ограниченията за ограничаване на [PowerShell](https://techcommunity.microsoft.com/t5/exchange-team-blog/updated-running-powershell-cmdlets-for-large-numbers-of-users-in/ba-p/1000628#)в Exchange Online.
