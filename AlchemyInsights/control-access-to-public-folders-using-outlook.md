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
# <a name="control-access-to-public-folders-using-outlook"></a>Управление на достъпа до публични папки чрез Outlook

За да определите кои потребители имат достъп до публични папки чрез Outlook:

1. Използване на `Set-CASMailbox <mailboxname> -PublicFolderClientAccess $true or $false`

$true: Позволяване на потребителите да имат достъп до публични папки в Outlook  
$false: Забраняване на потребителите да имат достъп до публични папки в Outlook. Това е стойността по подразбиране.  

2. `Set-OrganizationConfig -PublicFolderShowClientControl $true`

Забележка: Тази процедура може да управлява връзките само с настолната версия на Outlook за клиенти с Windows. Потребителите могат да продължат да имат достъп до публични папки с помощта на OWA или Outlook for Mac.

За повече информация вж. [Управляеми връзки към публични папки в Outlook](https://aka.ms/controlpf).
