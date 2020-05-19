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
ms.openlocfilehash: 0a07e6279f533a4c26a4e90c10651421a5df8860
ms.sourcegitcommit: 286000b588adef1bbbb28337a9d9e087ec783fa2
ms.translationtype: MT
ms.contentlocale: bg-BG
ms.lasthandoff: 04/27/2020
ms.locfileid: "44282563"
---
# <a name="change-email-address-of-an-microsoft-365-group"></a><span data-ttu-id="84f81-102">Промяна на имейл адреса на група на Microsoft 365</span><span class="sxs-lookup"><span data-stu-id="84f81-102">Change email address of an Microsoft 365 group</span></span>

<span data-ttu-id="84f81-103">Можете да промените имейл адреса на група на Microsoft 365 с помощта на центъра за администриране.</span><span class="sxs-lookup"><span data-stu-id="84f81-103">You can change the email address of an Microsoft 365 group by using the admin center.</span></span> <span data-ttu-id="84f81-104">Просто изберете групата и изберете @edit имейл адрес.</span><span class="sxs-lookup"><span data-stu-id="84f81-104">Just select the group and select @edit email address.</span></span>

<span data-ttu-id="84f81-105">Можете също да използвате exo PowerShell команда за промяна на основния SMTP адрес на microsoft 365 група:</span><span class="sxs-lookup"><span data-stu-id="84f81-105">You can also use following the EXO PowerShell command to change the primary SMTP address of an Microsoft 365 group:</span></span>

<span data-ttu-id="84f81-106">Задайте-унифицирана група <Group Name> -primarySmtpAddress<new SMTP Address></span><span class="sxs-lookup"><span data-stu-id="84f81-106">Set-UnifiedGroup <Group Name> -PrimarySmtpAddress <new SMTP Address></span></span>

<span data-ttu-id="84f81-107">Пример:</span><span class="sxs-lookup"><span data-stu-id="84f81-107">Example:</span></span>

```
    Set-UnifiedGroup Marketing -PrimarySmtpAddress marketing@contoso.com
```
