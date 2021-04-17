---
title: Възстановяване на изтрити елементи с кратка команда
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
- "1800008"
- "5718"
ms.openlocfilehash: d8f2a50f39d7bcd321692ab093e2efa6613e9814
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: bg-BG
ms.lasthandoff: 04/15/2021
ms.locfileid: "51835800"
---
# <a name="recover-deleted-items-with-cmdlet"></a><span data-ttu-id="78cda-102">Възстановяване на изтрити елементи с кратка команда</span><span class="sxs-lookup"><span data-stu-id="78cda-102">Recover deleted items with cmdlet</span></span>

- <span data-ttu-id="78cda-103">Използвайте [кратката команда Get-RecoverableItems,](https://docs.microsoft.com/powershell/module/exchange/get-recoverableitems?view=exchange-ps) за да видите изтритите елементи в пощенските кутии.</span><span class="sxs-lookup"><span data-stu-id="78cda-103">Use the [Get-RecoverableItems](https://docs.microsoft.com/powershell/module/exchange/get-recoverableitems?view=exchange-ps) cmdlet to view deleted items in mailboxes.</span></span> <span data-ttu-id="78cda-104">След като намерите изтритите елементи, можете да използвате кратката команда [Restore-RecoverableItems,](https://docs.microsoft.com/powershell/module/exchange/Restore-RecoverableItems?view=exchange-ps) за да ги възстановите.</span><span class="sxs-lookup"><span data-stu-id="78cda-104">After you find the deleted items, you use the [Restore-RecoverableItems](https://docs.microsoft.com/powershell/module/exchange/Restore-RecoverableItems?view=exchange-ps) cmdlet to restore them.</span></span>

- <span data-ttu-id="78cda-105">Вижте пълните подробности [в Get-RecoverableItems](https://docs.microsoft.com/powershell/module/exchange/get-recoverableitems?view=exchange-ps).</span><span class="sxs-lookup"><span data-stu-id="78cda-105">See full details in [Get-RecoverableItems](https://docs.microsoft.com/powershell/module/exchange/get-recoverableitems?view=exchange-ps).</span></span>

- <span data-ttu-id="78cda-106">Трябва да ви бъде възложена ролята за експортиране на импортиране на пощенски кутии, за да можете да изпълните тази кратка команда.</span><span class="sxs-lookup"><span data-stu-id="78cda-106">You need to be assigned the Mailbox Import Export role before you can run this cmdlet.</span></span> <span data-ttu-id="78cda-107">Вижте [Get-RecoverableItems](https://docs.microsoft.com/powershell/module/exchange/get-recoverableitems?view=exchange-ps) за повече информация.</span><span class="sxs-lookup"><span data-stu-id="78cda-107">Please see [Get-RecoverableItems](https://docs.microsoft.com/powershell/module/exchange/get-recoverableitems?view=exchange-ps) for more information.</span></span>
