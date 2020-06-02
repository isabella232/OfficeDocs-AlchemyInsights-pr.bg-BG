---
title: Възстановяване на изтрити елементи с команда
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "1800008"
- "5718"
ms.openlocfilehash: 86744d92a44096991079d1da3bdf4e95e58c55b7
ms.sourcegitcommit: 2afad0b107d03cd8c4de0b85b5bee38a13a7960d
ms.translationtype: MT
ms.contentlocale: bg-BG
ms.lasthandoff: 05/26/2020
ms.locfileid: "44492922"
---
# <a name="recover-deleted-items-with-cmdlet"></a><span data-ttu-id="46271-102">Възстановяване на изтрити елементи с команда</span><span class="sxs-lookup"><span data-stu-id="46271-102">Recover deleted items with cmdlet</span></span>

- <span data-ttu-id="46271-103">Използвайте [кратката команда Get-RecoverAbleItems](https://docs.microsoft.com/powershell/module/exchange/get-recoverableitems?view=exchange-ps) да видите изтритите елементи в пощенски кутии.</span><span class="sxs-lookup"><span data-stu-id="46271-103">Use the [Get-RecoverableItems](https://docs.microsoft.com/powershell/module/exchange/get-recoverableitems?view=exchange-ps) cmdlet to view deleted items in mailboxes.</span></span> <span data-ttu-id="46271-104">След като намерите изтрити елементи, можете да използвате [командата възстановяване recoverableItems](https://docs.microsoft.com/powershell/module/exchange/Restore-RecoverableItems?view=exchange-ps) да ги възстановите.</span><span class="sxs-lookup"><span data-stu-id="46271-104">After you find the deleted items, you use the [Restore-RecoverableItems](https://docs.microsoft.com/powershell/module/exchange/Restore-RecoverableItems?view=exchange-ps) cmdlet to restore them.</span></span>

- <span data-ttu-id="46271-105">Вижте пълните подробности в [Get-RecoverableItems](https://docs.microsoft.com/powershell/module/exchange/get-recoverableitems?view=exchange-ps).</span><span class="sxs-lookup"><span data-stu-id="46271-105">See full details in [Get-RecoverableItems](https://docs.microsoft.com/powershell/module/exchange/get-recoverableitems?view=exchange-ps).</span></span>

- <span data-ttu-id="46271-106">Трябва да бъде присвоена ролята за експортиране на пощенска кутия, преди да изпълните тази команда.</span><span class="sxs-lookup"><span data-stu-id="46271-106">You need to be assigned the Mailbox Import Export role before you can run this cmdlet.</span></span> <span data-ttu-id="46271-107">Вижте [Get-RecoverableItems](https://docs.microsoft.com/powershell/module/exchange/get-recoverableitems?view=exchange-ps) за повече информация.</span><span class="sxs-lookup"><span data-stu-id="46271-107">Please see [Get-RecoverableItems](https://docs.microsoft.com/powershell/module/exchange/get-recoverableitems?view=exchange-ps) for more information.</span></span>
