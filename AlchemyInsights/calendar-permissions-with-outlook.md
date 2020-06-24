---
title: Разрешения за календар
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3800009"
- "611"
ms.openlocfilehash: 78f27014c60badc801212177dd455ef2a0de5a9e
ms.sourcegitcommit: 722e9a0ed058cb1eab2dd053be2418b60f7d4aac
ms.translationtype: MT
ms.contentlocale: bg-BG
ms.lasthandoff: 06/23/2020
ms.locfileid: "44862030"
---
# <a name="calendar-permissions"></a>Разрешения за календар

Потребителите могат да променят собствените си разрешения за календар с Outlook в мрежата или други клиенти, но като администратор може да се наложи да проучи, както и.  
С Exchange PowerShell команда ще ви покаже разрешение в календара на потребителя:

`Get-MailboxFolderPermission <SMTPAddress>:\Calendar | FT -a`

За повече информация вижте следното:

- [Прекъсване на пощенска кутия](https://docs.microsoft.com/powershell/module/exchange/get-mailboxfolderpermission?view=exchange-ps)

- [Папка за сет-пощенска кутия](https://docs.microsoft.com/powershell/module/exchange/set-mailboxfolderpermission?view=exchange-ps)

- [Добавяне на пощенска кутия](https://office.visualstudio.com/DefaultCollection/MAX/_queries/query/Add-MailboxFolderPermission)

Разрешенията за календар се използват в споделянето на календари, за да видите повече информация за споделяне на календар на Outlook, вижте следните статии:

- [Споделяне на календара на Outlook с други хора](https://support.office.com/article/353ed2c1-3ec5-449d-8c73-6931a0adab88)
- [Споделяне на календара в Outlook в интернет за бизнеса](https://support.office.com/article/7ecef8ae-139c-40d9-bae2-a23977ee58d5)

За отстраняване на разрешение за календар можете да използвате инструмента [за поддръжка и възстановяване на помощника.](https://support.microsoft.com/office/e90bb691-c2a7-4697-a94f-88836856c72f)