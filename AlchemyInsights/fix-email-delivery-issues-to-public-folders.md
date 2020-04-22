---
title: Отстраняване на проблеми с доставката на имейли до публични папки с разрешен за поща
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1956"
- "3500007"
ms.assetid: ''
ms.openlocfilehash: e261fe60843555fa45927b0a6b36e1ccf79fb028
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: bg-BG
ms.lasthandoff: 04/22/2020
ms.locfileid: "43716341"
---
# <a name="fix-email-delivery-issues-to-mail-enabled-public-folders"></a>Отстраняване на проблеми с доставката на имейли до публични папки с разрешен за поща

Ако външни податели не могат да изпращат съобщения до вашата поща разрешени публични папки и податели получават грешка: **не може да бъде намерен (550 5.4.1)**, проверете имейл домейн за публичната папка е конфигуриран като вътрешен препращане домейн вместо авторитетен домейн:

1. Отворете центъра за администриране на [Exchange (EAC)](https://docs.microsoft.com/Exchange/exchange-admin-center).

2. Отидете на **Пощенски поток** \> **Приети домейни**, изберете приетия домейн и след това щракнете върху **Редактиране**.

3. В страницата със свойства, която се отваря, ако типът домейн е зададен на **авторитетен**, променете стойността **на вътрешно реле** и след това щракнете върху **Запиши**.

Ако външни податели получите **грешка, нямате разрешение (550 5.7.13),** изпълнете следната команда в [Exchange Online PowerShell](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell) да видите разрешенията за анонимни потребители в публичната папка:

`Get-PublicFolderClientPermission -Identity "<PublicFolderIdentity>" -User Anonymous`Например , `Get-PublicFolderClientPermission -Identity "\Customer Discussion" -User Anonymous`.

За да разрешите на външни потребители да изпращат имейл до тази публична папка, добавете правото createItems достъп до анонимен потребител. Например , `Add-PublicFolderClientPermission -Identity "\Customer Discussion" -User Anonymous -AccessRights CreateItems`.
