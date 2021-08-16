---
title: Коригиране на проблеми с доставянето на имейли в публични папки с активиран имейл
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
ms.openlocfilehash: ff1400f694ae037a8658356af068b4c20b8fa9d9908dafedb90db7bb6859530f
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: bg-BG
ms.lasthandoff: 08/05/2021
ms.locfileid: "54068801"
---
# <a name="fix-email-delivery-issues-to-mail-enabled-public-folders"></a>Коригиране на проблеми с доставянето на имейли в публични папки с активиран имейл

Ако външни податели не могат да изпращат съобщения до публични папки с разрешена поща, а подателите получават грешката: не може да бъде **намерена (550 5.4.1)**, проверете дали имейл домейнът за публичната папка е конфигуриран като вътрешен домейн на предаване вместо достоверен домейн:

1. Отворете центъра [Exchange администриране (EAC).](https://docs.microsoft.com/Exchange/exchange-admin-center)

2. Отидете на **Пощенски поток Приети** \> **домейни**, изберете приетия домейн и след това щракнете върху **Редактиране**.

3. В страницата със свойства, която се отваря, ако типът на домейна е зададен на Достовителен **,** променете стойността на **Вътрешно реле и** след това щракнете върху **Запиши**.

Ако външни податели получат грешката, която нямате разрешение **(550 5.7.13),** изпълнете следната команда [в Exchange Online PowerShell,](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell) за да видите разрешенията за анонимни потребители в публичната папка:

`Get-PublicFolderClientPermission -Identity "<PublicFolderIdentity>" -User Anonymous` Например `Get-PublicFolderClientPermission -Identity "\Customer Discussion" -User Anonymous` .

За да позволите на външни потребители да изпращат имейл до тази публична папка, добавете access CreateItems право на потребителя Анонимен. Например `Add-PublicFolderClientPermission -Identity "\Customer Discussion" -User Anonymous -AccessRights CreateItems` .
