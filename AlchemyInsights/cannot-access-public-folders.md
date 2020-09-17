---
title: Нямате достъп до публични папки
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
- "3500007"
- "3462"
ms.openlocfilehash: 272918b38f6019cb2bdcaa4013baebaa5f04fe85
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: bg-BG
ms.lasthandoff: 09/15/2020
ms.locfileid: "47812536"
---
# <a name="outlook-cannot-connect-to-public-folders"></a><span data-ttu-id="cb29a-102">Outlook не може да се свърже с публични папки</span><span class="sxs-lookup"><span data-stu-id="cb29a-102">Outlook cannot connect to public folders</span></span>

<span data-ttu-id="cb29a-103">Ако достъпът до публични папки не работи за някои потребители, опитайте следното:</span><span class="sxs-lookup"><span data-stu-id="cb29a-103">If public folder access isn't working for some users, try the following:</span></span>

<span data-ttu-id="cb29a-104">Свързване към ЕКСО PowerShell и конфигуриране на параметъра DefaultPublicFolderMailbox на потребителския акаунт за проблем, за да съответства на параметъра на работен потребителски акаунт.</span><span class="sxs-lookup"><span data-stu-id="cb29a-104">Connect to EXO PowerShell and configure the DefaultPublicFolderMailbox parameter on the problem user account to match the parameter on a working user account.</span></span>

<span data-ttu-id="cb29a-105">Например</span><span class="sxs-lookup"><span data-stu-id="cb29a-105">Example:</span></span>

<span data-ttu-id="cb29a-106">Получаване на пощенска кутия WorkingUser | Ft DefaultPublicFolderMailbox, EffectivePublicFolderMailbox</span><span class="sxs-lookup"><span data-stu-id="cb29a-106">Get-Mailbox WorkingUser | ft DefaultPublicFolderMailbox,EffectivePublicFolderMailbox</span></span>

<span data-ttu-id="cb29a-107">Set-пощенска кутия ProblemUser-DefaultPublicFolderMailbox \<value from previous command></span><span class="sxs-lookup"><span data-stu-id="cb29a-107">Set-Mailbox ProblemUser -DefaultPublicFolderMailbox \<value from previous command></span></span>

<span data-ttu-id="cb29a-108">Изчакайте поне един час, за да влезе в сила промяната.</span><span class="sxs-lookup"><span data-stu-id="cb29a-108">Wait at least one hour for the change to take effect.</span></span>

<span data-ttu-id="cb29a-109">Ако проблемът остава, следвайте [тази процедура](https://aka.ms/pfcte) , за да отстраните проблеми с достъпа до публични папки, като използвате Outlook.</span><span class="sxs-lookup"><span data-stu-id="cb29a-109">If the issue remains, please follow [this procedure](https://aka.ms/pfcte) to troubleshoot public folder access issues using Outlook.</span></span>
 
<span data-ttu-id="cb29a-110">**За да контролирате кои потребители да имат достъп до публични папки чрез Outlook**:</span><span class="sxs-lookup"><span data-stu-id="cb29a-110">**To control which users can access public folders using Outlook**:</span></span>

1.  <span data-ttu-id="cb29a-111">Използвайте Set-CASMailbox <mailboxname> -PublicFolderClientAccess $TRUE или $FALSE</span><span class="sxs-lookup"><span data-stu-id="cb29a-111">Use Set-CASMailbox <mailboxname> -PublicFolderClientAccess $true or $false</span></span>  
      
    <span data-ttu-id="cb29a-112">$true: Позволяване на достъп на потребителите до публични папки в Outlook</span><span class="sxs-lookup"><span data-stu-id="cb29a-112">$true: Allow users access public folders in Outlook</span></span>  
      
    <span data-ttu-id="cb29a-113">$false: предотвратяване на достъпа на потребителите до публични папки в Outlook.</span><span class="sxs-lookup"><span data-stu-id="cb29a-113">$false: Prevent user access to public folders in Outlook.</span></span> <span data-ttu-id="cb29a-114">Това е стойността по подразбиране.</span><span class="sxs-lookup"><span data-stu-id="cb29a-114">This is the default value.</span></span>  
        
2.  <span data-ttu-id="cb29a-115">Set-OrganizationConfig-PublicFolderShowClientControl $true</span><span class="sxs-lookup"><span data-stu-id="cb29a-115">Set-OrganizationConfig -PublicFolderShowClientControl $true</span></span>   
      
<span data-ttu-id="cb29a-116">**Забележка** Тази процедура може да управлява връзките само с настолната версия на Outlook за клиенти на Windows.</span><span class="sxs-lookup"><span data-stu-id="cb29a-116">**Note** This procedure can control connections only with Outlook desktop for Windows clients.</span></span> <span data-ttu-id="cb29a-117">Потребителят може да продължи да отваря публични папки, като използва OWA или Outlook for Mac.</span><span class="sxs-lookup"><span data-stu-id="cb29a-117">A user can continue accessing public folders using OWA or Outlook for Mac.</span></span>
 
<span data-ttu-id="cb29a-118">За повече информация вижте [обявяване на поддръжката за контролирани връзки с публични папки в Outlook](https://aka.ms/controlpf).</span><span class="sxs-lookup"><span data-stu-id="cb29a-118">For more info, see [Announcing Support for Controlled Connections to Public Folders in Outlook](https://aka.ms/controlpf).</span></span>