---
title: Софтуерните наличности липсват или са неточни
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
- "11382"
- "9001470"
ms.openlocfilehash: e886a53f8c063b5395dd002a7d16186985584d72
ms.sourcegitcommit: 0c104e2bd34ccc09bcea389e470692e92bcf1f8f
ms.translationtype: MT
ms.contentlocale: bg-BG
ms.lasthandoff: 05/26/2021
ms.locfileid: "52676081"
---
# <a name="software-inventory-is-missing-or-inaccurate"></a>Софтуерните наличности липсват или са неточни

Софтуерните наличности в Threat and Vulnerability Management (TVM) е списък на известен софтуер във вашата организация с официални enumerations на обща платформа (CPE).

Софтуерните продукти без официална CPE нямат публикувани уязвимости. Инвентарът включва и подробности, като например името на доставчика, броя на слабите страни, заплахите и броя на експонираните устройства.

Промените в софтуера на устройства обикновено се отразяват в порталите за защита в рамките на два часа. Понякога обаче може да отнеме повече време. В момента няма начин за принудително синхронизиране; това е непрекъсната непрекъсната оценка.

Ако сте направили промяна на софтуера и промяната не е точно отразена в TVM след 5 часа, изпълнете следните стъпки:

1. Проверете секцията за софтуерни доказателства, за да разберете как е открит софтуерът.
1. Уверете се, че софтуерът се поддържа. Софтуерът може да се вижда само на ниво устройство дори ако в момента не се поддържа от Threat and Vulnerability Management. Налични са обаче само ограничени данни.
1. За стъпки, за да съобщите за неточност от портала, вижте [Докладване на неточност](/microsoft-365/security/defender-endpoint/tvm-software-inventory?view=o365-worldwide#report-inaccuracy).
   
    **Забележка:** Съобщаването за неточност от портала на MDE е еднопосочен канал за инженерни дейности. Ако проблемът е спешен, отворете билет за поддръжка.

За повече информация вижте [Софтуерни наличности – Threat and Vulnerability Management](/microsoft-365/security/defender-endpoint/tvm-software-inventory).