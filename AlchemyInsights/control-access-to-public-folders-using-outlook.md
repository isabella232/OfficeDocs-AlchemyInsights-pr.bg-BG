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
ms.openlocfilehash: 1386b97f804e63455094abf64b9d9e2541d57dafa36535813b0d7689e0ce2966
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: bg-BG
ms.lasthandoff: 08/05/2021
ms.locfileid: "54032547"
---
# <a name="control-access-to-public-folders-using-outlook"></a>Управление на достъпа до публични папки чрез Outlook

За да определите кои потребители имат достъп до публични папки чрез Outlook:

1. Използване на `Set-CASMailbox <mailboxname> -PublicFolderClientAccess $true or $false`

$true: Позволяване на потребителите да имат достъп до публични папки в Outlook  
$false: Забраняване на потребителите да имат достъп до публични папки в Outlook. Това е стойността по подразбиране.  

2. `Set-OrganizationConfig -PublicFolderShowClientControl $true`

Забележка: Тази процедура може да управлява връзките само с настолната версия на Outlook за клиенти с Windows. Потребителите могат да продължат да имат достъп до публични папки с помощта на OWA или Outlook for Mac.

За повече информация вж. [Управляеми връзки към публични папки в Outlook](https://aka.ms/controlpf).
