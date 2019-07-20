---
title: Няма резултати от търсене на съдържание
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000661"
- "2527"
ms.openlocfilehash: 9f2c0273762f1a4a2b905487f461dc1d05db9209
ms.sourcegitcommit: 8f97342d8b46ab05f1e89018473caad9d35431df
ms.translationtype: MT
ms.contentlocale: bg-BG
ms.lasthandoff: 07/19/2019
ms.locfileid: "35800186"
---
# <a name="no-results-from-content-searchexports"></a>Няма резултати от съдържание търсене/износ

Проблеми със съдържание търсене/износ не връща никакви данни може да се дължи филтър за защита някои съответствието, който е настройка от един определен администратор и не се свързва към всички администратори.

За да разрешите този проблем, проверете да видите дали има някакви съответствие защитни филтри, които могат да се причинява това:
1. Свързване към сигурността и съответствието център Powershell
2. Изпълнете следните кратки команди:
<br>$org = "yourdomain.com"
<br>Get-ComplianceSecurityFilter-организация $org