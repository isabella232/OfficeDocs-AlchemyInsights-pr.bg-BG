---
title: Политика за защита на молбите
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/22/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "1073"
- "6700006"
ms.openlocfilehash: 7fed65e6749f72e6264070b360a52e72968fc8da
ms.sourcegitcommit: 6f7cbf1dc28c0693009ddf03d9768c1c65018964
ms.translationtype: MT
ms.contentlocale: bg-BG
ms.lasthandoff: 07/22/2020
ms.locfileid: "45423295"
---
# <a name="application-protection-policy"></a>Политика за защита на молбите

Ако сте нови за правилата за защита на приложението (APP), разгледайте преглед на [правилата за защита](https://docs.microsoft.com/intune/apps/app-protection-policy)на приложения .

За да започнете да използвате ПРИЛОЖЕНИЕТО, вижте [Как да създадете и присвоите правила за защита на приложенията](https://docs.microsoft.com/intune/app-protection-policies).

Изисквания на политиката за защита на приложението:

- Потребителят има лиценз Intune или EMS.
- Потребителят принадлежи към група, насочена към правилата за защита на приложението.
- Само един корпоративен потребител е влязъл в защитени приложения на дадено устройство.
- Приложението е внедрило [sdK На Intune](https://docs.microsoft.com/intune/app-sdk-get-started). За списък с приложения, които поддържат SDK, вижте [защитените с Microsoft Intune приложения.](https://docs.microsoft.com/intune/apps-supported-intune-apps)

Правилата важат, след като потребител, който отговаря на горните изисквания, се регистрира в приложение с активирано Внтуе SDK. Най-лесният начин да определите дали се прилага дадена политика е като се изисква потребителят да зададе ПИН в правилата. 

За повече информация вижте:

[ЧЗВ за отстраняване на НЕИЗПРАВНОСТИ APP/MAM](https://docs.microsoft.com/intune/apps/troubleshoot-mam)  

[Как да проверите настройката на правилата за защита на приложението](https://docs.microsoft.com/intune/app-protection-policies-validate)

[Разберете времето за доставка на правилата за защита на приложението](https://docs.microsoft.com/intune/app-protection-policy-delivery)  

[Как да следите правилата за защита на приложения](https://docs.microsoft.com/intune/app-protection-policies-monitor)