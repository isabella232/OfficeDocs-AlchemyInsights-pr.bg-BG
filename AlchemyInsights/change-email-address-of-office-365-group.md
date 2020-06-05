---
title: Промяна на имейл адреса на група на Microsoft 365
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "1200024"
- "4704"
ms.openlocfilehash: 32968f085a4e9d49f60ef88e4e78bf6c67629556
ms.sourcegitcommit: f28dafa0f727870038f72bc904da926daf4ec07b
ms.translationtype: HT
ms.contentlocale: bg-BG
ms.lasthandoff: 06/05/2020
ms.locfileid: "44580646"
---
# <a name="change-email-address-of-a-microsoft-365-group"></a><span data-ttu-id="d0115-102">Промяна на имейл адреса на група на Microsoft 365</span><span class="sxs-lookup"><span data-stu-id="d0115-102">Change email address of a Microsoft 365 group</span></span>

<span data-ttu-id="d0115-103">Можете да промените имейл адреса на група на Microsoft 365 с помощта на центъра за администриране.</span><span class="sxs-lookup"><span data-stu-id="d0115-103">You can change the email address of a Microsoft 365 group by using the admin center.</span></span> <span data-ttu-id="d0115-104">Просто изберете групата и изберете @edit имейл адрес.</span><span class="sxs-lookup"><span data-stu-id="d0115-104">Just select the group and select @edit email address.</span></span>

<span data-ttu-id="d0115-105">Можете да използвате и следната команда EXO PowerShell да промените основния SMTP адрес на група на Microsoft 365:</span><span class="sxs-lookup"><span data-stu-id="d0115-105">You can also use following the EXO PowerShell command to change the primary SMTP address of a Microsoft 365 group:</span></span>

<span data-ttu-id="d0115-106">Групи за задаване <Group Name> – основен адрес<new SMTP Address></span><span class="sxs-lookup"><span data-stu-id="d0115-106">Set-UnifiedGroup <Group Name> -PrimarySmtpAddress <new SMTP Address></span></span>

<span data-ttu-id="d0115-107">Пример:</span><span class="sxs-lookup"><span data-stu-id="d0115-107">Example:</span></span>

```
    Set-UnifiedGroup Marketing -PrimarySmtpAddress marketing@contoso.com
```
