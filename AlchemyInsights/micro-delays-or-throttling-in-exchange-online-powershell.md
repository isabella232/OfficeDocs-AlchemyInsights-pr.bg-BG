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
ms.openlocfilehash: cb97aa790264c23aae15fed49c353c7fb0d6209d9492c6881f1b1091fe80d7b8
ms.sourcegitcommit: 920051182781bd97ce4d4d6fbd268cb37b84d239
ms.translationtype: MT
ms.contentlocale: bg-BG
ms.lasthandoff: 08/11/2021
ms.locfileid: "57868523"
---
# <a name="micro-delays-or-throttling-in-exchange-online-powershell"></a>Микро закъснения или ограничаване на PowerShell в Exchange Online

Възможно е да видите предупреждения за "Приложено микро забавяне" или закъснения, когато изпълнявате скриптове и кратки команди в Exchange Online. Ето няколко предложения как да решите това:

- Изпълнете нашата диагностика, за да отпуснете правилата за ограничаване на PowerShell на вашия клиент. Това решение ще реши проблема за повечето.
- Ако проблемът все още не е решен, използвайте [модула Exchange Online v2 PowerShell](https://docs.microsoft.com/powershell/exchange/exchange-online/exchange-online-powershell-v2/exchange-online-powershell-v2?view=exchange-ps&preserve-view=true), който включва CMDlets, които са базирани на REST API и са значително по-изпълняващи. Това може да бъде чудесно решение за много от често използваните кратки команди.
- Ако трябва да използвате КРАТКИ КОМАНДИ, които не са включени в модула v2, вижте Изпълняване на кратки команди на PowerShell за голям брой потребители в Office 365 , което говори как да заобиколите ограниченията за ограничаване на [PowerShell](https://techcommunity.microsoft.com/t5/exchange-team-blog/updated-running-powershell-cmdlets-for-large-numbers-of-users-in/ba-p/1000628#)в Exchange Online.
