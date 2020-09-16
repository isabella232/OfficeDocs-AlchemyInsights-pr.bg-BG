---
title: Приветствено съобщение в Microsoft 365 Groups
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "1200024"
- "5685"
ms.openlocfilehash: de16ca6021441bf6cb781106b7f3da8eed86b0f1
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: bg-BG
ms.lasthandoff: 09/14/2020
ms.locfileid: "47725828"
---
# <a name="welcome-message-in-microsoft-365-groups"></a><span data-ttu-id="244e3-102">Приветствено съобщение в Microsoft 365 Groups</span><span class="sxs-lookup"><span data-stu-id="244e3-102">Welcome message in Microsoft 365 Groups</span></span>

<span data-ttu-id="244e3-103">Новите потребители, които се присъединяват към Microsoft 365 Group, ще получат приветствен имейл, ако свойството "UnifiedGroupWelcomeMessageEnabled" е истина.</span><span class="sxs-lookup"><span data-stu-id="244e3-103">New users joining Microsoft 365 group will receive welcome email if the "UnifiedGroupWelcomeMessageEnabled" property is True.</span></span>

<span data-ttu-id="244e3-104">В случай че искате да забраните приветственото съобщение, [Използвайте следната команда](https://docs.microsoft.com/powershell/exchange/exchange-online/exchange-online-powershell-v2/exchange-online-powershell-v2?view=exchange-ps) за командата "за".</span><span class="sxs-lookup"><span data-stu-id="244e3-104">In case you want to disable the welcome message, use the following [EXO PowerShell](https://docs.microsoft.com/powershell/exchange/exchange-online/exchange-online-powershell-v2/exchange-online-powershell-v2?view=exchange-ps) command:</span></span>

`
Set-UnifiedGroup <groupname> -UnifiedGroupWelcomeMessageEnabled:$False
`
