---
title: Съобщенията, изпратени до група на Microsoft 365, не се получават от всички членове
ms.author: pebaum
author: pebaum
manager: mnirkhe
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9003200"
- "5995"
ms.openlocfilehash: d222eb92d806bad52264139a8ddba72f323b3783
ms.sourcegitcommit: 10cfd9d552b0d8a096bcef34e82c04a4c166a13a
ms.translationtype: HT
ms.contentlocale: bg-BG
ms.lasthandoff: 03/05/2021
ms.locfileid: "50479442"
---
# <a name="messages-sent-to-a-microsoft-365-group-are-not-received-by-all-members"></a>Съобщенията, изпратени до група на Microsoft 365, не се получават от всички членове

Уверете се, че всички членове на групата са се абонирали за получаване на имейлите. Вижте [Следване на група в Outlook](https://support.microsoft.com/office/e147fc19-f548-4cd2-834f-80c6235b7c36).  

За да проверите състоянието на съобщенията на членовете, които са се абонирали за имейли на групата, изпълнете следната команда на [EXO PowerShell](https://docs.microsoft.com/powershell/exchange/connect-to-exchange-online-powershell?view=exchange-ps&preserve-view=true):

`Get-UnifiedGroup <GroupName> | Get-UnifiedGroupLinks -LinkType Subscribers`

Използвайте следната команда на EXO PowerShell, за да конфигурирате всички членове на групата да получават имейлите, изпратени до група на Microsoft 365, в папката им "Входящи":

`$Group = "Address of [Microsoft 365 Groups]"Get-UnifiedGroupLinks $Group -LinkType Member | % {Add-UnifiedGroupLinks -Identity $Group -LinkType subscriber -Links $_.Guid.toString() -Confirm:$false}`

Например:

`$Group = "testg@contoso.onmicrosoft.com"Get-UnifiedGroupLinks $Group -LinkType Member | % {Add-UnifiedGroupLinks -Identity $Group -LinkType subscriber -Links $_.Guid.toString() -Confirm:$false}`