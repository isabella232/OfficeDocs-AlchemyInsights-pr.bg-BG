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
# <a name="outlook-cannot-connect-to-public-folders"></a>Outlook не може да се свърже с публични папки

Ако достъпът до публични папки не работи за някои потребители, опитайте следното:

Свързване към ЕКСО PowerShell и конфигуриране на параметъра DefaultPublicFolderMailbox на потребителския акаунт за проблем, за да съответства на параметъра на работен потребителски акаунт.

Например

Получаване на пощенска кутия WorkingUser | Ft DefaultPublicFolderMailbox, EffectivePublicFolderMailbox

Set-пощенска кутия ProblemUser-DefaultPublicFolderMailbox \<value from previous command>

Изчакайте поне един час, за да влезе в сила промяната.

Ако проблемът остава, следвайте [тази процедура](https://aka.ms/pfcte) , за да отстраните проблеми с достъпа до публични папки, като използвате Outlook.
 
**За да контролирате кои потребители да имат достъп до публични папки чрез Outlook**:

1.  Използвайте Set-CASMailbox <mailboxname> -PublicFolderClientAccess $TRUE или $FALSE  
      
    $true: Позволяване на достъп на потребителите до публични папки в Outlook  
      
    $false: предотвратяване на достъпа на потребителите до публични папки в Outlook. Това е стойността по подразбиране.  
        
2.  Set-OrganizationConfig-PublicFolderShowClientControl $true   
      
**Забележка** Тази процедура може да управлява връзките само с настолната версия на Outlook за клиенти на Windows. Потребителят може да продължи да отваря публични папки, като използва OWA или Outlook for Mac.
 
За повече информация вижте [обявяване на поддръжката за контролирани връзки с публични папки в Outlook](https://aka.ms/controlpf).