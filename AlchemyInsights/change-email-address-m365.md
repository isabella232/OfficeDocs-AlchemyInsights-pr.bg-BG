---
title: Промяна на имейл адреса на група на Microsoft 365 или Microsoft Teams
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
- "1200024"
- "4704"
ms.openlocfilehash: ff7abaf3d8e0ed977eba5712bdd19185738fa75c
ms.sourcegitcommit: 8be59778b7d39213a27a471802eae7fc006eb1ff
ms.translationtype: HT
ms.contentlocale: bg-BG
ms.lasthandoff: 01/05/2021
ms.locfileid: "49756546"
---
# <a name="change-email-address-of-a-microsoft-365-group-or-microsoft-teams"></a><span data-ttu-id="4dec3-102">Промяна на имейл адреса на група на Microsoft 365 или Microsoft Teams</span><span class="sxs-lookup"><span data-stu-id="4dec3-102">Change email address of a Microsoft 365 group or Microsoft Teams</span></span>

<span data-ttu-id="4dec3-103">Можете да промените имейл адреса на група на Microsoft 365 или на Microsoft Teams, като използвате [Център за администриране на Microsoft 365](https://admin.microsoft.com/).</span><span class="sxs-lookup"><span data-stu-id="4dec3-103">You can change the email address of a Microsoft 365 group or Microsoft Teams by using the [Microsoft 365 admin center](https://admin.microsoft.com/).</span></span> <span data-ttu-id="4dec3-104">Просто изберете групата и изберете @редактиране на имейл адрес.</span><span class="sxs-lookup"><span data-stu-id="4dec3-104">Just select the group and select @edit email address.</span></span>

<span data-ttu-id="4dec3-105">Можете също да използвате следната EXO PowerShell команда за промяна на основния SMTP адрес на група на Microsoft 365/Teams:</span><span class="sxs-lookup"><span data-stu-id="4dec3-105">You can also use the following EXO PowerShell command to change the primary SMTP address of a Microsoft 365 group/Teams:</span></span>

`Set-UnifiedGroup <Group Name> -PrimarySmtpAddress <new SMTP Address>`

<span data-ttu-id="4dec3-106">Пример:</span><span class="sxs-lookup"><span data-stu-id="4dec3-106">Example:</span></span>

`Set-UnifiedGroup Marketing -PrimarySmtpAddress marketing@contoso.com`
