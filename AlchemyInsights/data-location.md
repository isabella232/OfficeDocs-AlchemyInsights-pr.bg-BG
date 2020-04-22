---
title: Местоположение на данните
ms.author: pebaum
author: pebaum
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "945"
- "5300023"
ms.assetid: 3bab036c-dbaa-406a-8b73-1e5f31993436
ms.openlocfilehash: c769c17796d805f88afb4d5b32adb7d4a9bb3ce0
ms.sourcegitcommit: 6bf1d945b4fd6a1fe37d00c5ea99adea7eef9910
ms.translationtype: MT
ms.contentlocale: bg-BG
ms.lasthandoff: 04/21/2020
ms.locfileid: "43655271"
---
# <a name="data-location"></a>Местоположение на данните

Можете да видите местоположението на вашия клиент в центъра за администриране или чрез свързване към Exchange Online чрез PowerShell.


**Център за администриране:**
1. Влезте в [центъра за администриране](https://admin.microsoft.com/Adminportal/Home).
2. Изберете **Настройки на** > **организацията профил**.
3. Под **Местоположение на данните**изберете Преглед на подробни **данни**.


**Powershell:**
1. Свързване с Exchange Online чрез Windows PowerShell.
2. Изпълнение на кратката команда [Get-OrganizationalUnit](https://docs.microsoft.com/powershell/module/exchange/active-directory/get-organizationalunit) да покаже списък на свойствата на вашия клиент. 
3. Погледнете свойството OrganizationId.

Когато имате местоположението на данните за EXO и SPO, можете да определите местоположението на данните за други услуги, които можете да използвате от [Мястото, където се намират данните ви](https://products.office.com/where-is-your-data-located).