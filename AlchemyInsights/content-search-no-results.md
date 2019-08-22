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
ms.openlocfilehash: 09cdbc3cb0465e0e0bc08872c49e283081ad3e92
ms.sourcegitcommit: 1d98db8acb9959aba3b5e308a567ade6b62da56c
ms.translationtype: MT
ms.contentlocale: bg-BG
ms.lasthandoff: 08/22/2019
ms.locfileid: "36516768"
---
# <a name="no-results-from-content-searchexports"></a>Няма резултати от съдържание търсене/износ

Проблеми със съдържание търсене/износ не връща никакви данни може да се дължи филтър за защита някои съответствието, който е настройка от един определен администратор и не се свързва към всички администратори.

За да разрешите този проблем, проверете да видите дали има някакви съответствие защитни филтри, които могат да се причинява това:
1. Свързване към сигурността и съответствието център Powershell
2. Изпълнете следните кратки команди:
<br>$org = "yourdomain.com"
<br>Get-ComplianceSecurityFilter-организация $org