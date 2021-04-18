---
title: Управление на достъпа до публични папки чрез Outlook
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "3500007"
- "3462"
ms.openlocfilehash: f528044ca7f6f2ee2812f9f831093c44eca26fe1
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: HT
ms.contentlocale: bg-BG
ms.lasthandoff: 04/15/2021
ms.locfileid: "51816729"
---
# <a name="control-access-to-public-folders-using-outlook"></a><span data-ttu-id="bc5fd-102">Управление на достъпа до публични папки чрез Outlook</span><span class="sxs-lookup"><span data-stu-id="bc5fd-102">Control access to public folders using Outlook</span></span>

<span data-ttu-id="bc5fd-103">За да определите кои потребители имат достъп до публични папки чрез Outlook:</span><span class="sxs-lookup"><span data-stu-id="bc5fd-103">To control which users can access public folders using Outlook:</span></span>

1. <span data-ttu-id="bc5fd-104">Използване на `Set-CASMailbox <mailboxname> -PublicFolderClientAccess $true or $false`</span><span class="sxs-lookup"><span data-stu-id="bc5fd-104">Use `Set-CASMailbox <mailboxname> -PublicFolderClientAccess $true or $false`</span></span>

<span data-ttu-id="bc5fd-105">$true: Позволяване на потребителите да имат достъп до публични папки в Outlook</span><span class="sxs-lookup"><span data-stu-id="bc5fd-105">$true: Allow users access public folders in Outlook</span></span>  
<span data-ttu-id="bc5fd-106">$false: Забраняване на потребителите да имат достъп до публични папки в Outlook.</span><span class="sxs-lookup"><span data-stu-id="bc5fd-106">$false: Prevent user access to public folders in Outlook.</span></span> <span data-ttu-id="bc5fd-107">Това е стойността по подразбиране.</span><span class="sxs-lookup"><span data-stu-id="bc5fd-107">This is the default value.</span></span>  

2. `Set-OrganizationConfig -PublicFolderShowClientControl $true`

<span data-ttu-id="bc5fd-108">Забележка: Тази процедура може да управлява връзките само с настолната версия на Outlook за клиенти с Windows.</span><span class="sxs-lookup"><span data-stu-id="bc5fd-108">Note: This procedure can only control connections with Outlook desktop for Windows clients.</span></span> <span data-ttu-id="bc5fd-109">Потребителите могат да продължат да имат достъп до публични папки с помощта на OWA или Outlook for Mac.</span><span class="sxs-lookup"><span data-stu-id="bc5fd-109">Users can continue accessing public folders using OWA or Outlook for Mac.</span></span>

<span data-ttu-id="bc5fd-110">За повече информация вж. [Управляеми връзки към публични папки в Outlook](https://aka.ms/controlpf).</span><span class="sxs-lookup"><span data-stu-id="bc5fd-110">For more information, see [Controlled Connections to Public Folders in Outlook](https://aka.ms/controlpf) for more information.</span></span>
