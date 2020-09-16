---
title: Изпращане като Microsoft 365 Group
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 08/19/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9003200"
ms.openlocfilehash: 51bd8a10c3da23941cc16d7ba860406f8477044a
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: bg-BG
ms.lasthandoff: 09/14/2020
ms.locfileid: "47740140"
---
# <a name="send-as-microsoft-365-group"></a>Изпращане като Microsoft 365 Group

Можете да присвоите разрешения "Изпрати като", за да разрешите на определени потребители да изпращат съобщения като група на Microsoft 365:  

1. Свързване към PowerShell на Exchange Online.  

2. Изпълнете следната команда:  

    Add-RecipientPermission `<GroupName>` - `<MailboxName>` AccessRights SendAs

За повече информация вижте [Разрешаване на членовете да изпращат или изпращат от името на групата](https://docs.microsoft.com/microsoft-365/admin/create-groups/allow-members-to-send-as-or-send-on-behalf-of-group?view=o365-worldwide).