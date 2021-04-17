---
title: Няма достъп до публични папки
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
- "3500007"
- "3462"
ms.openlocfilehash: af5bd57512ee917d6e22d3838d55a2a1d62750d4
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: bg-BG
ms.lasthandoff: 04/15/2021
ms.locfileid: "51819501"
---
# <a name="outlook-cannot-connect-to-public-folders"></a><span data-ttu-id="f5140-102">Outlook не може да се свърже с публични папки</span><span class="sxs-lookup"><span data-stu-id="f5140-102">Outlook cannot connect to public folders</span></span>

<span data-ttu-id="f5140-103">Ако достъпът до публична папка не работи за някои потребители, опитайте следното:</span><span class="sxs-lookup"><span data-stu-id="f5140-103">If public folder access isn't working for some users, try the following:</span></span>

<span data-ttu-id="f5140-104">Свържете се с EXO PowerShell и конфигурирайте параметъра DefaultPublicFolderMailbox на проблемния потребителски акаунт, така че да съответства на параметъра в работещ потребителски акаунт.</span><span class="sxs-lookup"><span data-stu-id="f5140-104">Connect to EXO PowerShell and configure the DefaultPublicFolderMailbox parameter on the problem user account to match the parameter on a working user account.</span></span>

<span data-ttu-id="f5140-105">Пример:</span><span class="sxs-lookup"><span data-stu-id="f5140-105">Example:</span></span>

<span data-ttu-id="f5140-106">Get-Mailbox работаИзползване на | ft DefaultPublicFolderMailbox,EffectivePublicFolderMailbox</span><span class="sxs-lookup"><span data-stu-id="f5140-106">Get-Mailbox WorkingUser | ft DefaultPublicFolderMailbox,EffectivePublicFolderMailbox</span></span>

<span data-ttu-id="f5140-107">Set-Mailbox ProblemUser -DefaultPublicFolderMailbox \<value from previous command></span><span class="sxs-lookup"><span data-stu-id="f5140-107">Set-Mailbox ProblemUser -DefaultPublicFolderMailbox \<value from previous command></span></span>

<span data-ttu-id="f5140-108">Изчакайте поне един час, за да в сила промяната.</span><span class="sxs-lookup"><span data-stu-id="f5140-108">Wait at least one hour for the change to take effect.</span></span>

<span data-ttu-id="f5140-109">Ако проблемът остане, следвайте тази процедура, за [да отстраните](https://aka.ms/pfcte) проблеми с достъпа до публична папка с помощта на Outlook.</span><span class="sxs-lookup"><span data-stu-id="f5140-109">If the issue remains, please follow [this procedure](https://aka.ms/pfcte) to troubleshoot public folder access issues using Outlook.</span></span>
 
<span data-ttu-id="f5140-110">**За да контролирате кои потребители имат достъп до публични папки с помощта на Outlook:**</span><span class="sxs-lookup"><span data-stu-id="f5140-110">**To control which users can access public folders using Outlook**:</span></span>

1.  <span data-ttu-id="f5140-111">Използване Set-CASMailbox <mailboxname> -PublicFolderClientAccess $true или $false</span><span class="sxs-lookup"><span data-stu-id="f5140-111">Use Set-CASMailbox <mailboxname> -PublicFolderClientAccess $true or $false</span></span>  
      
    <span data-ttu-id="f5140-112">$true: Разрешаване на потребителите да имат достъп до публични папки в Outlook</span><span class="sxs-lookup"><span data-stu-id="f5140-112">$true: Allow users access public folders in Outlook</span></span>  
      
    <span data-ttu-id="f5140-113">$false: Предотвратяване на достъпа на потребителите до публични папки в Outlook.</span><span class="sxs-lookup"><span data-stu-id="f5140-113">$false: Prevent user access to public folders in Outlook.</span></span> <span data-ttu-id="f5140-114">Това е стойността по подразбиране.</span><span class="sxs-lookup"><span data-stu-id="f5140-114">This is the default value.</span></span>  
        
2.  <span data-ttu-id="f5140-115">Set-OrganizationConfig -PublicFolderShowClientControl $true</span><span class="sxs-lookup"><span data-stu-id="f5140-115">Set-OrganizationConfig -PublicFolderShowClientControl $true</span></span>   
      
<span data-ttu-id="f5140-116">**Забележка** Тази процедура може да управлява връзки само с настолната версия на Outlook за клиенти на Windows.</span><span class="sxs-lookup"><span data-stu-id="f5140-116">**Note** This procedure can control connections only with Outlook desktop for Windows clients.</span></span> <span data-ttu-id="f5140-117">Потребителят може да продължи достъпа до публични папки с помощта на OWA или Outlook for Mac.</span><span class="sxs-lookup"><span data-stu-id="f5140-117">A user can continue accessing public folders using OWA or Outlook for Mac.</span></span>
 
<span data-ttu-id="f5140-118">За повече информация вижте [Обявяване на поддръжка за контролирани връзки към публични папки в Outlook.](https://aka.ms/controlpf)</span><span class="sxs-lookup"><span data-stu-id="f5140-118">For more info, see [Announcing Support for Controlled Connections to Public Folders in Outlook](https://aka.ms/controlpf).</span></span>