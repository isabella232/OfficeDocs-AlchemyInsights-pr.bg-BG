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
# <a name="messages-sent-to-a-microsoft-365-group-are-not-received-by-all-members"></a><span data-ttu-id="db2ca-102">Съобщенията, изпратени до група на Microsoft 365, не са получени от всички членове</span><span class="sxs-lookup"><span data-stu-id="db2ca-102">Messages sent to a Microsoft 365 group are not received by all members</span></span>

<span data-ttu-id="db2ca-103">Уверете се, че всички членове на групата са се абонирали за получаване на имейлите.</span><span class="sxs-lookup"><span data-stu-id="db2ca-103">Make sure that all group members have subscribed to receive the emails.</span></span> <span data-ttu-id="db2ca-104">Вижте [Следвайте група в Outlook](https://support.microsoft.com/office/e147fc19-f548-4cd2-834f-80c6235b7c36).</span><span class="sxs-lookup"><span data-stu-id="db2ca-104">See [Follow a group in Outlook](https://support.microsoft.com/office/e147fc19-f548-4cd2-834f-80c6235b7c36).</span></span>  

<span data-ttu-id="db2ca-105">За да проверите състоянието на съобщението на членовете, които са се абонирали за група имейли, изпълнете следната команда [exO PowerShell](https://docs.microsoft.com/powershell/exchange/connect-to-exchange-online-powershell?view=exchange-ps):</span><span class="sxs-lookup"><span data-stu-id="db2ca-105">To check the message status of members who have subscribed to group emails, run the following command on [EXO PowerShell](https://docs.microsoft.com/powershell/exchange/connect-to-exchange-online-powershell?view=exchange-ps):</span></span>

`Get-UnifiedGroup <GroupName> | Get-UnifiedGroupLinks -LinkType Subscribers`