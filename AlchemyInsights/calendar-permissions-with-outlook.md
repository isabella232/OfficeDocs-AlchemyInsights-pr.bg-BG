---
title: Разрешения за календар
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3800009"
- "611"
ms.openlocfilehash: cfee520e26587c0a649c08084853c31232d027f8
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: bg-BG
ms.lasthandoff: 09/14/2020
ms.locfileid: "47748782"
---
# <a name="calendar-permissions"></a><span data-ttu-id="e319c-102">Разрешения за календар</span><span class="sxs-lookup"><span data-stu-id="e319c-102">Calendar Permissions</span></span>

<span data-ttu-id="e319c-103">Потребителите могат да променят собствения си разрешения за календар с Outlook в уеб или други клиенти, но като администратор може да се наложи и да проучите.</span><span class="sxs-lookup"><span data-stu-id="e319c-103">Users can change their own Calendar Permissions with Outlook on the Web or other clients, but as an admin you may need to investigate as well.</span></span>  
<span data-ttu-id="e319c-104">С кратката команда на PowerShell на Exchange ще ви покаже разрешение за календара на потребител:</span><span class="sxs-lookup"><span data-stu-id="e319c-104">With Exchange PowerShell cmdlet will show you the permission on a user’s calendar:</span></span>

`Get-MailboxFolderPermission <SMTPAddress>:\Calendar | FT -a`

<span data-ttu-id="e319c-105">За да видите повече информация, вижте следното:</span><span class="sxs-lookup"><span data-stu-id="e319c-105">To see more information see the following:</span></span>

- [<span data-ttu-id="e319c-106">Get-MailboxFolderPermission</span><span class="sxs-lookup"><span data-stu-id="e319c-106">Get-MailboxFolderPermission</span></span>](https://docs.microsoft.com/powershell/module/exchange/get-mailboxfolderpermission?view=exchange-ps)

- [<span data-ttu-id="e319c-107">Set-MailboxFolderPermission</span><span class="sxs-lookup"><span data-stu-id="e319c-107">Set-MailboxFolderPermission</span></span>](https://docs.microsoft.com/powershell/module/exchange/set-mailboxfolderpermission?view=exchange-ps)

- [<span data-ttu-id="e319c-108">Add-MailboxFolderPermission</span><span class="sxs-lookup"><span data-stu-id="e319c-108">Add-MailboxFolderPermission</span></span>](https://office.visualstudio.com/DefaultCollection/MAX/_queries/query/Add-MailboxFolderPermission)

<span data-ttu-id="e319c-109">Разрешения за календар се използват в споделянето на календари, за да видите повече информация за споделянето на календар на Outlook, вижте следните статии:</span><span class="sxs-lookup"><span data-stu-id="e319c-109">Calendar Permissions are used in the sharing of calendars, to see more information about sharing an Outlook calendar, see these articles:</span></span>

- [<span data-ttu-id="e319c-110">Споделяне на календара на Outlook с други хора</span><span class="sxs-lookup"><span data-stu-id="e319c-110">Share an Outlook calendar with other people</span></span>](https://support.office.com/article/353ed2c1-3ec5-449d-8c73-6931a0adab88)
- [<span data-ttu-id="e319c-111">Споделяне на календара в Outlook в уеб за фирми</span><span class="sxs-lookup"><span data-stu-id="e319c-111">Share your calendar in Outlook on the web for business</span></span>](https://support.office.com/article/7ecef8ae-139c-40d9-bae2-a23977ee58d5)

<span data-ttu-id="e319c-112">За отстраняване на проблеми с разрешенията за календар можете да използвате инструмента за [помощник за поддръжка и възстановяване](https://support.microsoft.com/office/e90bb691-c2a7-4697-a94f-88836856c72f) .</span><span class="sxs-lookup"><span data-stu-id="e319c-112">To troubleshoot Calendar Permission you can use the [Support and Recovery Assistant](https://support.microsoft.com/office/e90bb691-c2a7-4697-a94f-88836856c72f) tool.</span></span>