---
title: Отстраняването на неизправности с ediscovery има грешки
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 05/20/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "11274"
- "3200003"
ms.openlocfilehash: 1df2b7153cac99419adc4f72b1c3732e7c746eac
ms.sourcegitcommit: 730efbac8eec016b2b4f83f1b0e01e077f28c444
ms.translationtype: MT
ms.contentlocale: bg-BG
ms.lasthandoff: 05/20/2021
ms.locfileid: "52676035"
---
# <a name="troubleshooting-ediscovery-holds-errors"></a>Отстраняването на неизправности с ediscovery има грешки

Имате проблеми с задържането на електронни данни? Ето някои най-добри практики, които трябва да имате предвид:

- Проверете състоянието на задържане на разпределението.  Ако състоянието е **On (Pending)** или **Off (Pending)**, изчакайте, за да завърши разпределението на задържането.
- Обединяването на откриване на електронни данни задържа актуализациите в едно групово искане, вместо да актуализира правилата неколкократно за всяка транзакция.
- Изпълнете Set-CaseHoldPolicy <policyname> -RetryDistribution в Powershell на центъра за защита и съответствие. За подробности вижте Информация [Свързване центъра за & съответствие на PowerShell.](/powershell/exchange/connect-to-scc-powershell)

За стъпки за проверка на тези настройки и допълнителни най-добри практики за ограничаване и разрешаване на откриване на електронни данни има проблеми, вижте Отстраняване на грешки при откриване [на електронни данни.](/microsoft-365/compliance/hold-distribution-errors)
За информация относно отстраняването на други често срещани проблеми с откриване на електронни данни вижте Изследване, отстраняване на неизправности и отстраняване на [често срещани проблеми с откриване на електронни данни](/microsoft-365/compliance/ediscovery-troubleshooting-common-issues).
