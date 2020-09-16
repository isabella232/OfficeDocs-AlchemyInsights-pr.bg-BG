---
title: Възстановяване на изтрити елементи с кратка команда
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
- "1800008"
- "5718"
ms.openlocfilehash: 91a9bcf75b13881b903a1d3b6f2da53f65811c9c
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: bg-BG
ms.lasthandoff: 09/14/2020
ms.locfileid: "47741292"
---
# <a name="recover-deleted-items-with-cmdlet"></a><span data-ttu-id="0e58a-102">Възстановяване на изтрити елементи с кратка команда</span><span class="sxs-lookup"><span data-stu-id="0e58a-102">Recover deleted items with cmdlet</span></span>

- <span data-ttu-id="0e58a-103">Използвайте кратката команда [get-RecoverableItems](https://docs.microsoft.com/powershell/module/exchange/get-recoverableitems?view=exchange-ps) , за да прегледате изтритите елементи в пощенските кутии.</span><span class="sxs-lookup"><span data-stu-id="0e58a-103">Use the [Get-RecoverableItems](https://docs.microsoft.com/powershell/module/exchange/get-recoverableitems?view=exchange-ps) cmdlet to view deleted items in mailboxes.</span></span> <span data-ttu-id="0e58a-104">След като намерите изтритите елементи, използвайте кратката команда [възстановяване-RecoverableItems](https://docs.microsoft.com/powershell/module/exchange/Restore-RecoverableItems?view=exchange-ps) , за да ги възстановите.</span><span class="sxs-lookup"><span data-stu-id="0e58a-104">After you find the deleted items, you use the [Restore-RecoverableItems](https://docs.microsoft.com/powershell/module/exchange/Restore-RecoverableItems?view=exchange-ps) cmdlet to restore them.</span></span>

- <span data-ttu-id="0e58a-105">Вижте пълните данни в [get-RecoverableItems](https://docs.microsoft.com/powershell/module/exchange/get-recoverableitems?view=exchange-ps).</span><span class="sxs-lookup"><span data-stu-id="0e58a-105">See full details in [Get-RecoverableItems](https://docs.microsoft.com/powershell/module/exchange/get-recoverableitems?view=exchange-ps).</span></span>

- <span data-ttu-id="0e58a-106">За да можете да изпълните тази кратка команда, трябва да ви е присвоена ролята за импортиране на експортираната пощенска кутия.</span><span class="sxs-lookup"><span data-stu-id="0e58a-106">You need to be assigned the Mailbox Import Export role before you can run this cmdlet.</span></span> <span data-ttu-id="0e58a-107">Вижте [получаване на RecoverableItems](https://docs.microsoft.com/powershell/module/exchange/get-recoverableitems?view=exchange-ps) за повече информация.</span><span class="sxs-lookup"><span data-stu-id="0e58a-107">Please see [Get-RecoverableItems](https://docs.microsoft.com/powershell/module/exchange/get-recoverableitems?view=exchange-ps) for more information.</span></span>
