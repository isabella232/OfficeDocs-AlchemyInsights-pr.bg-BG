---
title: Прикрепвам проблеми с имейл доставка с активирана поща публични папки
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: ''
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1956"
- "3500007"
ms.assetid: ''
ms.openlocfilehash: e24a4db2deb3f691209a1634d932ed277a79c868
ms.sourcegitcommit: 5fb7a4b28859690020efdea630d03e70cc0e6334
ms.translationtype: MT
ms.contentlocale: bg-BG
ms.lasthandoff: 06/28/2019
ms.locfileid: "35387694"
---
# <a name="fix-email-delivery-issues-to-mail-enabled-public-folders"></a>Прикрепвам проблеми с имейл доставка с активирана поща публични папки

Ако външни податели не може да изпращате съобщения до вашите публични папки с активирана поща, и податели появи грешка: **не можа да се намери (550 5.4.1)**, проверка на имейл домейн за публичната папка е конфигуриран като домейн за вътрешно препредаване вместо достоверен домейн:

1. Отворете [центъра за администриране на Exchange (EAC)](https://docs.microsoft.com/Exchange/exchange-admin-center).

2. Отидете на **потока от поща** \> **приети домейни**, изберете приетият домейн и след това щракнете върху **Редактиране**.

3. В свойствата на страница това отваря, ако типът на домейна е зададен на **авторитетни**, променете стойността за **вътрешно препредаване** и след това щракнете върху **Запиши**.

Ако външни податели грешка **нямате разрешение (550 5.7.13)**, изпълнете следната команда в [Exchange Online PowerShell](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell) да видите разрешенията за анонимни потребители в публичната папка:

`Get-PublicFolderClientPermission -Identity "<PublicFolderIdentity>" -User Anonymous`За пример `Get-PublicFolderClientPermission -Identity "\Customer Discussion" -User Anonymous`.

За да позволите на външни потребители да изпращат имейл до тази публична папка, добавете CreateItems достъп право на потребителя анонимен. За пример `Add-PublicFolderClientPermission -Identity "\Customer Discussion" -User Anonymous -AccessRights CreateItems`.
