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
ms.openlocfilehash: b53534dd0666fa64e692910aa6800abab30169a97fbe567c815ce6b948381a63
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: bg-BG
ms.lasthandoff: 08/05/2021
ms.locfileid: "54057991"
---
# <a name="no-results-from-content-searchexports"></a>Няма резултати от търсене/експортиране на съдържание

Проблеми с търсенето/експортирането на съдържание, които не връщат никакви данни, може да се дължат на определен филтър за защита на съответствието, който е бил настроен от конкретен администратор и не го съобщава на всички администратори.

За да отстраните това, проверете дали има някакви филтри за защита на съответствието, които може да са причина за това:
1. Свързване центъра за защита и съответствие Powershell
2. Изпълнете следните команди:
<br>$org = "yourdomain.com"
<br>Get-ComplianceSecurityFilter -Organization $org