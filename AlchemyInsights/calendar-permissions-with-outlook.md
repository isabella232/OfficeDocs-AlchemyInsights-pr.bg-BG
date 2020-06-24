---
title: Разрешения за календар
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3800009"
- "611"
ms.openlocfilehash: 78f27014c60badc801212177dd455ef2a0de5a9e
ms.sourcegitcommit: 722e9a0ed058cb1eab2dd053be2418b60f7d4aac
ms.translationtype: MT
ms.contentlocale: bg-BG
ms.lasthandoff: 06/23/2020
ms.locfileid: "44862030"
---
# <a name="calendar-permissions"></a><span data-ttu-id="cc54d-102">Разрешения за календар</span><span class="sxs-lookup"><span data-stu-id="cc54d-102">Calendar Permissions</span></span>

<span data-ttu-id="cc54d-103">Потребителите могат да променят собствените си разрешения за календар с Outlook в мрежата или други клиенти, но като администратор може да се наложи да проучи, както и.</span><span class="sxs-lookup"><span data-stu-id="cc54d-103">Users can change their own Calendar Permissions with Outlook on the Web or other clients, but as an admin you may need to investigate as well.</span></span>  
<span data-ttu-id="cc54d-104">С Exchange PowerShell команда ще ви покаже разрешение в календара на потребителя:</span><span class="sxs-lookup"><span data-stu-id="cc54d-104">With Exchange PowerShell cmdlet will show you the permission on a user’s calendar:</span></span>

`Get-MailboxFolderPermission <SMTPAddress>:\Calendar | FT -a`

<span data-ttu-id="cc54d-105">За повече информация вижте следното:</span><span class="sxs-lookup"><span data-stu-id="cc54d-105">To see more information see the following:</span></span>

- [<span data-ttu-id="cc54d-106">Прекъсване на пощенска кутия</span><span class="sxs-lookup"><span data-stu-id="cc54d-106">Get-MailboxFolderPermission</span></span>](https://docs.microsoft.com/powershell/module/exchange/get-mailboxfolderpermission?view=exchange-ps)

- [<span data-ttu-id="cc54d-107">Папка за сет-пощенска кутия</span><span class="sxs-lookup"><span data-stu-id="cc54d-107">Set-MailboxFolderPermission</span></span>](https://docs.microsoft.com/powershell/module/exchange/set-mailboxfolderpermission?view=exchange-ps)

- [<span data-ttu-id="cc54d-108">Добавяне на пощенска кутия</span><span class="sxs-lookup"><span data-stu-id="cc54d-108">Add-MailboxFolderPermission</span></span>](https://office.visualstudio.com/DefaultCollection/MAX/_queries/query/Add-MailboxFolderPermission)

<span data-ttu-id="cc54d-109">Разрешенията за календар се използват в споделянето на календари, за да видите повече информация за споделяне на календар на Outlook, вижте следните статии:</span><span class="sxs-lookup"><span data-stu-id="cc54d-109">Calendar Permissions are used in the sharing of calendars, to see more information about sharing an Outlook calendar, see these articles:</span></span>

- [<span data-ttu-id="cc54d-110">Споделяне на календара на Outlook с други хора</span><span class="sxs-lookup"><span data-stu-id="cc54d-110">Share an Outlook calendar with other people</span></span>](https://support.office.com/article/353ed2c1-3ec5-449d-8c73-6931a0adab88)
- [<span data-ttu-id="cc54d-111">Споделяне на календара в Outlook в интернет за бизнеса</span><span class="sxs-lookup"><span data-stu-id="cc54d-111">Share your calendar in Outlook on the web for business</span></span>](https://support.office.com/article/7ecef8ae-139c-40d9-bae2-a23977ee58d5)

<span data-ttu-id="cc54d-112">За отстраняване на разрешение за календар можете да използвате инструмента [за поддръжка и възстановяване на помощника.](https://support.microsoft.com/office/e90bb691-c2a7-4697-a94f-88836856c72f)</span><span class="sxs-lookup"><span data-stu-id="cc54d-112">To troubleshoot Calendar Permission you can use the [Support and Recovery Assistant](https://support.microsoft.com/office/e90bb691-c2a7-4697-a94f-88836856c72f) tool.</span></span>