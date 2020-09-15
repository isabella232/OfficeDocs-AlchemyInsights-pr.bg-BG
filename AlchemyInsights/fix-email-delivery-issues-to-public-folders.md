---
title: Отстраняване на проблеми с доставянето на имейл до публични папки с активирана поща
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1956"
- "3500007"
ms.assetid: ''
ms.openlocfilehash: da35ae4bd911fb75f23cc1c99aacbaa2392425dd
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: bg-BG
ms.lasthandoff: 09/14/2020
ms.locfileid: "47677917"
---
# <a name="fix-email-delivery-issues-to-mail-enabled-public-folders"></a>Отстраняване на проблеми с доставянето на имейл до публични папки с активирана поща

Ако външни податели не могат да изпращат съобщения до вашите публични папки с активиран имейл и подателите получат грешката: **не може да се намери (550 5.4.1)**, проверете дали домейнът за имейла за публичната папка е конфигуриран като вътрешен домейн за препращане, а не за достоверен домейн:

1. Отворете [центъра за администриране на Exchange (EAC)](https://docs.microsoft.com/Exchange/exchange-admin-center).

2. Отидете на **Mail flow** \> **приеманите домейни**"поща", изберете приетия домейн и след това щракнете върху **Редактиране**.

3. В страницата свойства, която се отваря, ако типът на домейна е зададен като **достоверен**, променете стойността на **вътрешно препращане** и след това щракнете върху **Запиши**.

Ако външни податели получат грешката, **която нямате разрешение (550 5.7.13)**, изпълнете следната команда в [Exchange Online PowerShell](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell) , за да видите разрешенията за анонимни потребители в публичната папка:

`Get-PublicFolderClientPermission -Identity "<PublicFolderIdentity>" -User Anonymous` Например `Get-PublicFolderClientPermission -Identity "\Customer Discussion" -User Anonymous` .

За да разрешите на външни потребители да изпращат имейли до тази публична папка, добавете CreateItems Access направо към анонимния потребител. Например `Add-PublicFolderClientPermission -Identity "\Customer Discussion" -User Anonymous -AccessRights CreateItems` .
