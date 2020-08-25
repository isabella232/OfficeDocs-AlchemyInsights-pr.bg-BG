---
title: Изпращане като Microsoft 365 Group
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 08/19/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9003200"
ms.openlocfilehash: cfb4bd5ce59eeccdd0812d013b8a444aebeb1d4c
ms.sourcegitcommit: 9818d3c8e6b10f23244e51286e2463caf48fffd5
ms.translationtype: MT
ms.contentlocale: bg-BG
ms.lasthandoff: 08/21/2020
ms.locfileid: "46871610"
---
# <a name="send-as-microsoft-365-group"></a><span data-ttu-id="160c0-102">Изпращане като Microsoft 365 Group</span><span class="sxs-lookup"><span data-stu-id="160c0-102">Send As Microsoft 365 group</span></span>

<span data-ttu-id="160c0-103">Можете да присвоите разрешения "Изпрати като", за да разрешите на определени потребители да изпращат съобщения като група на Microsoft 365:</span><span class="sxs-lookup"><span data-stu-id="160c0-103">You can assign Send As permissions to allow specific users to send messages as a Microsoft 365 group:</span></span>  

1. <span data-ttu-id="160c0-104">Свързване към PowerShell на Exchange Online.</span><span class="sxs-lookup"><span data-stu-id="160c0-104">Connect to Exchange Online PowerShell.</span></span>  

2. <span data-ttu-id="160c0-105">Изпълнете следната команда:</span><span class="sxs-lookup"><span data-stu-id="160c0-105">Run the following command:</span></span>  

    <span data-ttu-id="160c0-106">Add-RecipientPermission `<GroupName>` - `<MailboxName>` AccessRights SendAs</span><span class="sxs-lookup"><span data-stu-id="160c0-106">Add-RecipientPermission `<GroupName>` -Trustee `<MailboxName>` -AccessRights SendAs</span></span>

<span data-ttu-id="160c0-107">За повече информация вижте [Разрешаване на членовете да изпращат или изпращат от името на групата](https://docs.microsoft.com/microsoft-365/admin/create-groups/allow-members-to-send-as-or-send-on-behalf-of-group?view=o365-worldwide).</span><span class="sxs-lookup"><span data-stu-id="160c0-107">For more information, see [Allow members to send as or send on behalf of a group](https://docs.microsoft.com/microsoft-365/admin/create-groups/allow-members-to-send-as-or-send-on-behalf-of-group?view=o365-worldwide).</span></span>