---
title: Правила за защита на приложенията
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/22/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "1073"
- "6700006"
ms.openlocfilehash: ab6ad9c4bf95ee013c66384ec8449ceb1b56e8f3ea9e95c695dbbab0e9fa3fc3
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: bg-BG
ms.lasthandoff: 08/05/2021
ms.locfileid: "53969960"
---
# <a name="application-protection-policy"></a>Правила за защита на приложенията

Ако сте начинаещ в правилата за защита на приложенията (APP), прегледайте общ преглед на правилата [за защита на приложенията](https://docs.microsoft.com/intune/apps/app-protection-policy).

За да започнете да използвате APP, вижте [Как да създавате и присвоявате правила за защита на приложения](https://docs.microsoft.com/intune/app-protection-policies).

Изисквания към правилата за защита на приложенията:

- Потребителят има лиценз за Intune или EMS.
- Потребителят принадлежи към група, към която са насочени правилата за защита на приложенията.
- Само един корпоративен потребител е влезли в защитени приложения на устройство.
- Приложението е внедрило [SDK на Intune](https://docs.microsoft.com/intune/app-sdk-get-started). За списък с приложения, които поддържат SDK, вж. [Microsoft Intune приложения.](https://docs.microsoft.com/intune/apps-supported-intune-apps)

Правилата се прилагат, след като потребител, който отговаря на горните изисквания, влезе в приложение с активиран SDK на Intune. Най-лесният начин да определите дали е приложено правило, е да се изисква потребителят да зададете пин в правилата. 

За повече информация вижте:

[ЧЗВ за отстраняване на неизправности в APP/MAM](https://docs.microsoft.com/intune/apps/troubleshoot-mam)  

[Как да проверите настройката на правилата за защита на приложенията](https://docs.microsoft.com/intune/app-protection-policies-validate)

[Разбиране на времето за доставяне на правилата за защита на приложенията](https://docs.microsoft.com/intune/app-protection-policy-delivery)  

[Как да следите правилата за защита на приложения](https://docs.microsoft.com/intune/app-protection-policies-monitor)