---
title: Разрешения за календар
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3800009"
- "611"
ms.openlocfilehash: bbd49134bd4a4451649b76bb5f60b19065910cae
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: bg-BG
ms.lasthandoff: 04/15/2021
ms.locfileid: "51819897"
---
# <a name="calendar-permissions"></a><span data-ttu-id="48ed9-102">Разрешения за календар</span><span class="sxs-lookup"><span data-stu-id="48ed9-102">Calendar Permissions</span></span>

<span data-ttu-id="48ed9-103">Потребителите могат да променят свои собствени разрешения за календар с Outlook в уеб или други клиенти, но като администратор може да се наложи да проучите и вас.</span><span class="sxs-lookup"><span data-stu-id="48ed9-103">Users can change their own Calendar Permissions with Outlook on the Web or other clients, but as an admin you may need to investigate as well.</span></span>  
<span data-ttu-id="48ed9-104">С кратката команда на Exchange PowerShell ще ви покаже разрешението в календара на потребителя:</span><span class="sxs-lookup"><span data-stu-id="48ed9-104">With Exchange PowerShell cmdlet will show you the permission on a user’s calendar:</span></span>

`Get-MailboxFolderPermission <SMTPAddress>:\Calendar | FT -a`

<span data-ttu-id="48ed9-105">За да видите повече информация, вижте следното:</span><span class="sxs-lookup"><span data-stu-id="48ed9-105">To see more information see the following:</span></span>

- [<span data-ttu-id="48ed9-106">Get-MailboxFolderPermission</span><span class="sxs-lookup"><span data-stu-id="48ed9-106">Get-MailboxFolderPermission</span></span>](https://docs.microsoft.com/powershell/module/exchange/get-mailboxfolderpermission?view=exchange-ps)

- [<span data-ttu-id="48ed9-107">Set-MailboxFolderPermission</span><span class="sxs-lookup"><span data-stu-id="48ed9-107">Set-MailboxFolderPermission</span></span>](https://docs.microsoft.com/powershell/module/exchange/set-mailboxfolderpermission?view=exchange-ps)

- [<span data-ttu-id="48ed9-108">Add-MailboxFolderPermission</span><span class="sxs-lookup"><span data-stu-id="48ed9-108">Add-MailboxFolderPermission</span></span>](https://office.visualstudio.com/DefaultCollection/MAX/_queries/query/Add-MailboxFolderPermission)

<span data-ttu-id="48ed9-109">Разрешенията за календар се използват в споделянето на календари, за да видите повече информация за споделянето на календар на Outlook, вижте следните статии:</span><span class="sxs-lookup"><span data-stu-id="48ed9-109">Calendar Permissions are used in the sharing of calendars, to see more information about sharing an Outlook calendar, see these articles:</span></span>

- [<span data-ttu-id="48ed9-110">Споделяне на календара на Outlook с други хора</span><span class="sxs-lookup"><span data-stu-id="48ed9-110">Share an Outlook calendar with other people</span></span>](https://support.office.com/article/353ed2c1-3ec5-449d-8c73-6931a0adab88)
- [<span data-ttu-id="48ed9-111">Споделяне на вашия календар в Outlook в уеб за бизнеса</span><span class="sxs-lookup"><span data-stu-id="48ed9-111">Share your calendar in Outlook on the web for business</span></span>](https://support.office.com/article/7ecef8ae-139c-40d9-bae2-a23977ee58d5)

<span data-ttu-id="48ed9-112">За отстраняване на неизправности с разрешение за календар можете да използвате [инструмента помощник за поддръжка и](https://support.microsoft.com/office/e90bb691-c2a7-4697-a94f-88836856c72f) възстановяване.</span><span class="sxs-lookup"><span data-stu-id="48ed9-112">To troubleshoot Calendar Permission you can use the [Support and Recovery Assistant](https://support.microsoft.com/office/e90bb691-c2a7-4697-a94f-88836856c72f) tool.</span></span>