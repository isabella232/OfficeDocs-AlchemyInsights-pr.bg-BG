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
# <a name="outlook-cannot-connect-to-public-folders"></a>Outlook не може да се свърже с публични папки

Ако достъпът до публична папка не работи за някои потребители, опитайте следното:

Свържете се с EXO PowerShell и конфигурирайте параметъра DefaultPublicFolderMailbox на проблемния потребителски акаунт, така че да съответства на параметъра в работещ потребителски акаунт.

Пример:

Get-Mailbox работаИзползване на | ft DefaultPublicFolderMailbox,EffectivePublicFolderMailbox

Set-Mailbox ProblemUser -DefaultPublicFolderMailbox \<value from previous command>

Изчакайте поне един час, за да в сила промяната.

Ако проблемът остане, следвайте тази процедура, за [да отстраните](https://aka.ms/pfcte) проблеми с достъпа до публична папка с помощта на Outlook.
 
**За да контролирате кои потребители имат достъп до публични папки с помощта на Outlook:**

1.  Използване Set-CASMailbox <mailboxname> -PublicFolderClientAccess $true или $false  
      
    $true: Разрешаване на потребителите да имат достъп до публични папки в Outlook  
      
    $false: Предотвратяване на достъпа на потребителите до публични папки в Outlook. Това е стойността по подразбиране.  
        
2.  Set-OrganizationConfig -PublicFolderShowClientControl $true   
      
**Забележка** Тази процедура може да управлява връзки само с настолната версия на Outlook за клиенти на Windows. Потребителят може да продължи достъпа до публични папки с помощта на OWA или Outlook for Mac.
 
За повече информация вижте [Обявяване на поддръжка за контролирани връзки към публични папки в Outlook.](https://aka.ms/controlpf)