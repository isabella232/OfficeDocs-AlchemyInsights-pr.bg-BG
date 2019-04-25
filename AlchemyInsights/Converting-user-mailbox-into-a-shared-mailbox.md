---
title: Конвертиране на пощенска кутия на потребител в споделената пощенска кутия?
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: reference
ms.service: o365-administration
localization_priority: Normal
ROBOTS: NOINDEX, NOFOLLOW
description: ''
ms.openlocfilehash: 4da54121763fd33aa111f3bb3c26963cd271dc51
ms.sourcegitcommit: 9d78905c512192ffc4675468abd2efc5f2e4baf4
ms.translationtype: MT
ms.contentlocale: bg-BG
ms.lasthandoff: 04/23/2019
ms.locfileid: "32374312"
---
<span data-ttu-id="25f3e-102">Можете да преобразувате само потребителска пощенска кутия към споделена пощенска кутия, ако потребителят има лиценз за обмен.</span><span class="sxs-lookup"><span data-stu-id="25f3e-102">You can only convert a user mailbox to a shared mailbox if the user has an Exchange license.</span></span> <span data-ttu-id="25f3e-103">След като пощенската кутия се конвертира, тя ще продължи да се появи в списъка на активните потребители, защото този списък включва споделени пощенски кутии.</span><span class="sxs-lookup"><span data-stu-id="25f3e-103">After the mailbox is converted, it will continue to show up in the active users list because that list includes shared mailboxes.</span></span> <span data-ttu-id="25f3e-104">Обаче преобразувания пощенската кутия ще се появи в списъка на споделена пощенска кутия.</span><span class="sxs-lookup"><span data-stu-id="25f3e-104">However, the converted mailbox will also show up in the shared mailbox list.</span></span> 
  
<span data-ttu-id="25f3e-105">Ако се опитате да преобразувате пощенска кутия в Exchange административната конзола и конвертирането не успее, изчистете кеша на браузъра и бисквитки и опитайте отново.</span><span class="sxs-lookup"><span data-stu-id="25f3e-105">If you try to convert a mailbox in the Exchange Admin Console and the conversion fails, clear your browser cache and cookies and try again.</span></span> <span data-ttu-id="25f3e-106">Ако тя все още не работи, опитайте конвертиране на пощенската кутия в размяната управление на Шел като пуснете следната команда:</span><span class="sxs-lookup"><span data-stu-id="25f3e-106">If it still isn't working, try converting the mailbox in the Exchange Management Shell by running the following command:</span></span>
  
```
Set-Mailbox -Type Shared
```

<span data-ttu-id="25f3e-107">Повече информация за преобразуване на пощенската кутия е наличен в [Конвертиране на потребителска пощенска кутия към споделена пощенска кутия](https://support.office.com/client/2e122487-e1f5-4f26-ba41-5689249d93ba).</span><span class="sxs-lookup"><span data-stu-id="25f3e-107">More mailbox conversion information is available in [Convert a user mailbox to a shared mailbox](https://support.office.com/client/2e122487-e1f5-4f26-ba41-5689249d93ba).</span></span>
  
