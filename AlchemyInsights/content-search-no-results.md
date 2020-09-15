---
title: Търсене на съдържание няма резултати
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000661"
- "2527"
ms.openlocfilehash: 1e90c403556a317ff810971ccfa4a91694fb1171
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: bg-BG
ms.lasthandoff: 09/14/2020
ms.locfileid: "47680636"
---
# <a name="no-results-from-content-searchexports"></a>Няма резултати от търсенето/експортиране на съдържание

Проблемите при търсене/Експортиране на съдържание, които не връщат каквито и да е данни, може да се дължат на определен филтър за защита на съответствието, който е инсталирал от конкретен администратор и не го е информирал за всички администратори.

За да отстраните това, проверете дали има филтри за защита за съответствие, които може да причиняват това:
1. Свързване към центъра за сигурност и съответствие на PowerShell
2. Изпълнете следните кратки команди:
<br>$org = "yourdomain.com"
<br>Get-ComplianceSecurityFilter-$org за организация