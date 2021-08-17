---
title: Разрешения за календар
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
- "3800009"
- "611"
ms.openlocfilehash: 4bf7680a422f096401f0a87bccd1b8dd11f4489f882bcc06864e37d6a248438c
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: bg-BG
ms.lasthandoff: 08/05/2021
ms.locfileid: "54046093"
---
# <a name="calendar-permissions"></a>Разрешения за календар

Потребителите могат да променят свои собствени разрешения за календар с Outlook в уеб или други клиенти, но като администратор може да се наложи също да проучите.  
С Exchange кратката команда на PowerShell ще ви покаже разрешението в календара на потребителя:

`Get-MailboxFolderPermission <SMTPAddress>:\Calendar | FT -a`

За да видите повече информация, вижте следното:

- [Get-MailboxFolderPermission](https://docs.microsoft.com/powershell/module/exchange/get-mailboxfolderpermission?view=exchange-ps)

- [Set-MailboxFolderPermission](https://docs.microsoft.com/powershell/module/exchange/set-mailboxfolderpermission?view=exchange-ps)

- [Add-MailboxFolderPermission](https://office.visualstudio.com/DefaultCollection/MAX/_queries/query/Add-MailboxFolderPermission)

Разрешенията за календар се използват в споделянето на календари, за да видите повече информация за споделянето на Outlook календар, вижте следните статии:

- [Споделяне на календара на Outlook с други хора](https://support.office.com/article/353ed2c1-3ec5-449d-8c73-6931a0adab88)
- [Споделяне на вашия календар в Outlook в уеб за бизнеса](https://support.office.com/article/7ecef8ae-139c-40d9-bae2-a23977ee58d5)

За отстраняване на неизправности с разрешението за календар можете [да използвате Помощник за поддръжка и възстановяване](https://support.microsoft.com/office/e90bb691-c2a7-4697-a94f-88836856c72f) инструмент.