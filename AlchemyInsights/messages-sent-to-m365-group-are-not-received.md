---
title: Съобщенията, изпратени до microsoft 365 група, не са получени от всички членове
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9003200"
- "5995"
ms.openlocfilehash: 2c98841aaa278c1bc18b3ec9007240b1e856f41e
ms.sourcegitcommit: 743a9e4967993c5463272240280c22e27a8dc5b6
ms.contentlocale: bg-BG
ms.lasthandoff: 07/06/2020
ms.locfileid: "45051484"
---
# <a name="messages-sent-to-a-microsoft-365-group-are-not-received-by-all-members"></a>Съобщенията, изпратени до група на Microsoft 365, не са получени от всички членове

Уверете се, че всички членове на групата са се абонирали за получаване на имейлите. Вижте [Следвайте група в Outlook](https://support.microsoft.com/office/e147fc19-f548-4cd2-834f-80c6235b7c36).  

За да проверите състоянието на съобщението на членовете, които са се абонирали за група имейли, изпълнете следната команда [exO PowerShell](https://docs.microsoft.com/powershell/exchange/connect-to-exchange-online-powershell?view=exchange-ps):

`Get-UnifiedGroup <GroupName> | Get-UnifiedGroupLinks -LinkType Subscribers`