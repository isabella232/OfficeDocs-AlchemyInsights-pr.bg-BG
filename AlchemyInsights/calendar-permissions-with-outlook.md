---
title: Разрешения за календар
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
- "3800009"
- "611"
ms.openlocfilehash: cfee520e26587c0a649c08084853c31232d027f8
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: bg-BG
ms.lasthandoff: 09/14/2020
ms.locfileid: "47748782"
---
# <a name="calendar-permissions"></a>Разрешения за календар

Потребителите могат да променят собствения си разрешения за календар с Outlook в уеб или други клиенти, но като администратор може да се наложи и да проучите.  
С кратката команда на PowerShell на Exchange ще ви покаже разрешение за календара на потребител:

`Get-MailboxFolderPermission <SMTPAddress>:\Calendar | FT -a`

За да видите повече информация, вижте следното:

- [Get-MailboxFolderPermission](https://docs.microsoft.com/powershell/module/exchange/get-mailboxfolderpermission?view=exchange-ps)

- [Set-MailboxFolderPermission](https://docs.microsoft.com/powershell/module/exchange/set-mailboxfolderpermission?view=exchange-ps)

- [Add-MailboxFolderPermission](https://office.visualstudio.com/DefaultCollection/MAX/_queries/query/Add-MailboxFolderPermission)

Разрешения за календар се използват в споделянето на календари, за да видите повече информация за споделянето на календар на Outlook, вижте следните статии:

- [Споделяне на календара на Outlook с други хора](https://support.office.com/article/353ed2c1-3ec5-449d-8c73-6931a0adab88)
- [Споделяне на календара в Outlook в уеб за фирми](https://support.office.com/article/7ecef8ae-139c-40d9-bae2-a23977ee58d5)

За отстраняване на проблеми с разрешенията за календар можете да използвате инструмента за [помощник за поддръжка и възстановяване](https://support.microsoft.com/office/e90bb691-c2a7-4697-a94f-88836856c72f) .