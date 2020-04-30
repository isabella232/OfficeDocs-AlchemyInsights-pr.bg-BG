---
title: Микро закъснения или ограничаване на PowerShell в Exchange Online
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "3500011"
- "5106"
ms.openlocfilehash: 7ab4e7f18b7b8edf08098af8fe9674f66b1b81f4
ms.sourcegitcommit: fbaa2ce2cfb4d56d8c4cf2fa2d95489bdfcb7ff0
ms.translationtype: HT
ms.contentlocale: bg-BG
ms.lasthandoff: 04/30/2020
ms.locfileid: "43947777"
---
# <a name="micro-delays-or-throttling-in-exchange-online-powershell"></a><span data-ttu-id="ac153-102">Микро закъснения или ограничаване на PowerShell в Exchange Online</span><span class="sxs-lookup"><span data-stu-id="ac153-102">Micro delays or throttling in Exchange Online PowerShell</span></span>

<span data-ttu-id="ac153-103">Възможно е да видите предупреждения за "Приложено микро забавяне" или закъснения, когато изпълнявате скриптове и кратки команди в Exchange Online.</span><span class="sxs-lookup"><span data-stu-id="ac153-103">You might see "Micro delay applied" warnings or delays when you run scripts and cmdlets in Exchange Online.</span></span> <span data-ttu-id="ac153-104">Ето две предложения, свързани с това:</span><span class="sxs-lookup"><span data-stu-id="ac153-104">Here are two suggestions related to this:</span></span>

- <span data-ttu-id="ac153-105">Може да поискате да се опитате да използвате [модула Exchange Online v2 PowerShell](https://docs.microsoft.com/powershell/exchange/exchange-online/exchange-online-powershell-v2/exchange-online-powershell-v2?view=exchange-ps), който включва кратки команди, които са базирани на REST API и са значително по-подходящи.</span><span class="sxs-lookup"><span data-stu-id="ac153-105">You might want to try using the [Exchange Online v2 PowerShell module](https://docs.microsoft.com/powershell/exchange/exchange-online/exchange-online-powershell-v2/exchange-online-powershell-v2?view=exchange-ps), which includes CMDlets that are based on REST API and are significantly more performant.</span></span> <span data-ttu-id="ac153-106">Това може да бъде чудесно решение за много от често използваните кратки команди.</span><span class="sxs-lookup"><span data-stu-id="ac153-106">This might be a great solution for a lot of Get- CMDlets that are frequently used.</span></span>
- <span data-ttu-id="ac153-107">Ако трябва да използвате кратки команди, които все още не са включени в модула V2, вижте [Изпълнение на кратки команди на PowerShell за голям брой потребители в Office 365](https://techcommunity.microsoft.com/t5/exchange-team-blog/updated-running-powershell-cmdlets-for-large-numbers-of-users-in/ba-p/1000628#), където се говори за това как да се ориентирате в очакваните ограничения при PowerShell в Exchange Online.</span><span class="sxs-lookup"><span data-stu-id="ac153-107">If you need to use CMDlets that are not covered in the v2 module yet, please see [Running PowerShell cmdlets for large numbers of users in Office 365](https://techcommunity.microsoft.com/t5/exchange-team-blog/updated-running-powershell-cmdlets-for-large-numbers-of-users-in/ba-p/1000628#), which talks about how to get around expected PowerShell throttling limits in Exchange Online.</span></span>
