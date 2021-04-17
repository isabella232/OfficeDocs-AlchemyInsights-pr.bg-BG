---
title: Търсене на съдържание Без резултати
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
- "9000661"
- "2527"
ms.openlocfilehash: 0267286ca5967ee891e65343d49adf776f0322a6
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: bg-BG
ms.lasthandoff: 04/15/2021
ms.locfileid: "51816837"
---
# <a name="no-results-from-content-searchexports"></a>Няма резултати от търсене/експортиране на съдържание

Проблеми с търсенето/експортирането на съдържание, които не връщат никакви данни, може да се дължат на определен филтър за защита на съответствието, който е бил настроен от конкретен администратор и не го съобщава на всички администратори.

За да отстраните това, проверете дали има някакви филтри за защита на съответствието, които може да са причина за това:
1. Свързване към центъра за защита и съответствие Powershell
2. Изпълнете следните команди:
<br>$org = "yourdomain.com"
<br>Get-ComplianceSecurityFilter -Organization $org