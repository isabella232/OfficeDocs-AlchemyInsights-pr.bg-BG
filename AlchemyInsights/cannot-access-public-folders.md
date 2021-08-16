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
ms.openlocfilehash: f129da8731877aa00fd9b1dcf20905d353a4895303390ce7ff5642a8ff3ccbc2
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: bg-BG
ms.lasthandoff: 08/05/2021
ms.locfileid: "53996619"
---
# <a name="outlook-cannot-connect-to-public-folders"></a>Outlook не може да се свърже с публични папки

Ако достъпът до публична папка не работи за някои потребители, опитайте следното:

Свързване към EXO PowerShell и конфигурирайте параметъра DefaultPublicFolderMailbox на проблемния потребителски акаунт, така че да съответства на параметъра на работещ потребителски акаунт.

Пример:

Get-Mailbox работаИзползване на | ft DefaultPublicFolderMailbox,EffectivePublicFolderMailbox

Set-Mailbox ProblemUser -DefaultPublicFolderMailbox \<value from previous command>

Изчакайте поне един час, за да в сила промяната.

Ако проблемът остане, следвайте тази процедура, за [да отстраните](https://aka.ms/pfcte) проблеми с достъпа до публична папка чрез Outlook.
 
**За да управлявате кои потребители имат достъп до публични папки с помощта Outlook:**

1.  Използване Set-CASMailbox <mailboxname> -PublicFolderClientAccess $true или $false  
      
    $true: Позволяване на потребителите да имат достъп до публични папки в Outlook  
      
    $false: Забраняване на потребителите да имат достъп до публични папки в Outlook. Това е стойността по подразбиране.  
        
2.  Set-OrganizationConfig -PublicFolderShowClientControl $true   
      
**Забележка** Тази процедура може да управлява връзки само с Outlook работен плот за Windows клиенти. Потребителят може да продължи достъпа до публични папки с помощта на OWA или Outlook for Mac.
 
За повече информация вижте [Обявяване на поддръжка за контролирани връзки към публични папки в Outlook.](https://aka.ms/controlpf)