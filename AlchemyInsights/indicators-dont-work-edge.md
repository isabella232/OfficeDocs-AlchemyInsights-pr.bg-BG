---
title: Индикаторите не работят с помощта на браузъра Edge
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 05/25/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "11230"
- "9005470"
ms.openlocfilehash: df62d965e0dc2ddb656571af99b1e4c3cb52ea35
ms.sourcegitcommit: 4b504650e11adb9894c37b6d8608b53f9d5fc13d
ms.translationtype: MT
ms.contentlocale: bg-BG
ms.lasthandoff: 05/25/2021
ms.locfileid: "52676076"
---
# <a name="indicators-dont-work-using-edge-browser"></a>Индикаторите не работят с помощта на браузъра Edge

След като сте създали индикатор, не е зачетен от Edge (Smartscreen). За повече информация вижте Създаване [на индикатори за ИД и URL адреси/домейни.](/microsoft-365/security/defender-endpoint/indicator-ip-domain)

## <a name="step-1-ensure-the-following"></a>Стъпка 1: Уверете се, че:

- Уверете се, че индикаторът е правилен (без печатни грешки в IP/URL адрес, правилно действие, правилните групи на RBAC).
- Изчакайте най-малко 2 часа след създаването на индикатора, за да се вземе предвид евентуалното закъснение.
- Уверете се, че системата(ите) са внедрани в Microsoft Defender за крайна точка.
- Уверете се, че системата(ите) могат да комуникират с облака.
- Уверете се, че Smartscreen е разрешен и до който може да се достигне, като стигнете [до тестовия сайт](https://demo.smartscreen.msft.net).

## <a name="step-2-troubleshoot-the-potential-issue"></a>Стъпка 2: Отстраняване на потенциалния проблем

- Уверете се, че клиентът отговаря на изискванията. За подробности вижте Създаване [на индикатори за ИД и URL адреси/домейни.](/microsoft-365/security/defender-endpoint/indicator-ip-domain)
- Уверете се, че използвате най-новата версия на браузъра Edge. За да разберете най-новата версия, [вижте Разберете коя версия на Microsoft Edge имате](https://support.microsoft.com/microsoft-edge/find-out-which-version-of-microsoft-edge-you-have-c726bee8-c42e-e472-e954-4cf5123497eb).
- Рестартирайте браузъра Edge.
- Навигирайте до сайта, за който имате настройка на индикатор. Ако сайтът не се показва по очаквания начин, продължете със стъпка 3. 

## <a name="step-3-collect-data"></a>Стъпка 3: Събиране на данни

- Събиране **на диагностични данни от MDEClientAnalyzer.** За инструкции вижте Проблеми [с компютрите за табло към Microsoft Defender за крайна точка.](issues-with-onboarding-machines.md)
- Ако ви е удобно да инсталирате и събирате проследяване на Fiddler, вижте [Telerik Fiddler](http://www.telerik.com/fiddler).
- Ако предпочитате указания от поддръжката на Microsoft, изберете иконата Поддръжка по-долу, за да отворите калъф за поддръжка.
