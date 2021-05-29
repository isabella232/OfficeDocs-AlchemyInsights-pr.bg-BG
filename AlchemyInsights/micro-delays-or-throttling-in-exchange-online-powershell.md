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
# <a name="micro-delays-or-throttling-in-exchange-online-powershell"></a><span data-ttu-id="f8418-102">Микро закъснения или ограничаване на PowerShell в Exchange Online</span><span class="sxs-lookup"><span data-stu-id="f8418-102">Micro delays or throttling in Exchange Online PowerShell</span></span>

<span data-ttu-id="f8418-103">Възможно е да видите предупреждения за "Приложено микро забавяне" или закъснения, когато изпълнявате скриптове и кратки команди в Exchange Online.</span><span class="sxs-lookup"><span data-stu-id="f8418-103">You might see "Micro delay applied" warnings or delays when you run scripts and cmdlets in Exchange Online.</span></span> <span data-ttu-id="f8418-104">Ето няколко предложения как да решите това:</span><span class="sxs-lookup"><span data-stu-id="f8418-104">Here are a few suggestions how to solve this:</span></span>

- <span data-ttu-id="f8418-105">Изпълнете нашата диагностика, за да отпуснете правилата за ограничаване на PowerShell на вашия клиент.</span><span class="sxs-lookup"><span data-stu-id="f8418-105">Please run our diagnostics to relax your tenant's PowerShell throttling policies.</span></span> <span data-ttu-id="f8418-106">Това решение ще реши проблема за повечето.</span><span class="sxs-lookup"><span data-stu-id="f8418-106">This solution will solve the problem for most.</span></span>
- <span data-ttu-id="f8418-107">Ако проблемът все още не е решен, използвайте [модула Exchange Online v2 PowerShell](/powershell/exchange/exchange-online/exchange-online-powershell-v2/exchange-online-powershell-v2?view=exchange-ps&preserve-view=true), който включва CMDlets, които са базирани на REST API и са значително по-изпълняващи.</span><span class="sxs-lookup"><span data-stu-id="f8418-107">If issue still not solved, use the [Exchange Online v2 PowerShell module](/powershell/exchange/exchange-online/exchange-online-powershell-v2/exchange-online-powershell-v2?view=exchange-ps&preserve-view=true), which includes CMDlets that are based on REST API and are significantly more performant.</span></span> <span data-ttu-id="f8418-108">Това може да бъде чудесно решение за много от често използваните кратки команди.</span><span class="sxs-lookup"><span data-stu-id="f8418-108">This might be a great solution for a lot of Get- CMDlets that are frequently used.</span></span>
- <span data-ttu-id="f8418-109">Ако трябва да използвате КРАТКИ КОМАНДИ, които не са включени в модула v2, вижте Изпълняване на кратки команди на PowerShell за голям брой потребители в Office 365 , което говори как да заобиколите ограниченията за ограничаване на [PowerShell](https://techcommunity.microsoft.com/t5/exchange-team-blog/updated-running-powershell-cmdlets-for-large-numbers-of-users-in/ba-p/1000628#)в Exchange Online.</span><span class="sxs-lookup"><span data-stu-id="f8418-109">If you need to use CMDlets that are not covered in the v2 module, please see [Running PowerShell cmdlets for large numbers of users in Office 365](https://techcommunity.microsoft.com/t5/exchange-team-blog/updated-running-powershell-cmdlets-for-large-numbers-of-users-in/ba-p/1000628#), which talks about how to get around PowerShell throttling limits in Exchange Online.</span></span>
