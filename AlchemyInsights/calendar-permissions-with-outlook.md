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
ms.openlocfilehash: bbd49134bd4a4451649b76bb5f60b19065910cae
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: bg-BG
ms.lasthandoff: 04/15/2021
ms.locfileid: "51819897"
---
# <a name="calendar-permissions"></a>Разрешения за календар

Потребителите могат да променят свои собствени разрешения за календар с Outlook в уеб или други клиенти, но като администратор може да се наложи да проучите и вас.  
С кратката команда на Exchange PowerShell ще ви покаже разрешението в календара на потребителя:

`Get-MailboxFolderPermission <SMTPAddress>:\Calendar | FT -a`

За да видите повече информация, вижте следното:

- [Get-MailboxFolderPermission](https://docs.microsoft.com/powershell/module/exchange/get-mailboxfolderpermission?view=exchange-ps)

- [Set-MailboxFolderPermission](https://docs.microsoft.com/powershell/module/exchange/set-mailboxfolderpermission?view=exchange-ps)

- [Add-MailboxFolderPermission](https://office.visualstudio.com/DefaultCollection/MAX/_queries/query/Add-MailboxFolderPermission)

Разрешенията за календар се използват в споделянето на календари, за да видите повече информация за споделянето на календар на Outlook, вижте следните статии:

- [Споделяне на календара на Outlook с други хора](https://support.office.com/article/353ed2c1-3ec5-449d-8c73-6931a0adab88)
- [Споделяне на вашия календар в Outlook в уеб за бизнеса](https://support.office.com/article/7ecef8ae-139c-40d9-bae2-a23977ee58d5)

За отстраняване на неизправности с разрешение за календар можете да използвате [инструмента помощник за поддръжка и](https://support.microsoft.com/office/e90bb691-c2a7-4697-a94f-88836856c72f) възстановяване.