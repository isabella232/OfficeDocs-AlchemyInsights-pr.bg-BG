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
ms.openlocfilehash: ab34b8939b95b29bedb797f640dd744bc783adef
ms.sourcegitcommit: 1d98db8acb9959aba3b5e308a567ade6b62da56c
ms.translationtype: MT
ms.contentlocale: bg-BG
ms.lasthandoff: 08/22/2019
ms.locfileid: "36496388"
---
# <a name="convert-a-user-mail-box-into-a-shared-mailbox"></a><span data-ttu-id="92c5c-102">Конвертиране на потребител пощенска кутия в споделена пощенска кутия</span><span class="sxs-lookup"><span data-stu-id="92c5c-102">Convert a user mail box into a shared mailbox</span></span>

<span data-ttu-id="92c5c-103">Можете да преобразувате само потребителска пощенска кутия към споделена пощенска кутия, ако потребителят има лиценз за обмен.</span><span class="sxs-lookup"><span data-stu-id="92c5c-103">You can only convert a user mailbox to a shared mailbox if the user has an Exchange license.</span></span> <span data-ttu-id="92c5c-104">След като пощенската кутия се конвертира, тя ще продължи да се появи в списъка на активните потребители, защото този списък включва споделени пощенски кутии.</span><span class="sxs-lookup"><span data-stu-id="92c5c-104">After the mailbox is converted, it will continue to show up in the active users list because that list includes shared mailboxes.</span></span> <span data-ttu-id="92c5c-105">Обаче преобразувания пощенската кутия ще се появи в списъка на споделена пощенска кутия.</span><span class="sxs-lookup"><span data-stu-id="92c5c-105">However, the converted mailbox will also show up in the shared mailbox list.</span></span> 
  
<span data-ttu-id="92c5c-106">Ако се опитате да преобразувате пощенска кутия в Exchange административната конзола и конвертирането не успее, изчистете кеша на браузъра и бисквитки и опитайте отново.</span><span class="sxs-lookup"><span data-stu-id="92c5c-106">If you try to convert a mailbox in the Exchange Admin Console and the conversion fails, clear your browser cache and cookies and try again.</span></span> <span data-ttu-id="92c5c-107">Ако тя все още не работи, опитайте конвертиране на пощенската кутия в размяната управление на Шел като пуснете следната команда:</span><span class="sxs-lookup"><span data-stu-id="92c5c-107">If it still isn't working, try converting the mailbox in the Exchange Management Shell by running the following command:</span></span>
  
```
Set-Mailbox -Type Shared
```

<span data-ttu-id="92c5c-108">Повече информация за преобразуване на пощенската кутия е наличен в [Конвертиране на потребителска пощенска кутия към споделена пощенска кутия](https://docs.microsoft.com/office365/admin/email/convert-user-mailbox-to-shared-mailbox).</span><span class="sxs-lookup"><span data-stu-id="92c5c-108">More mailbox conversion information is available in [Convert a user mailbox to a shared mailbox](https://docs.microsoft.com/office365/admin/email/convert-user-mailbox-to-shared-mailbox).</span></span>
  
