---
title: Проблеми с премахването на изключено или изведено от експлоатация устройство от наличностите на устройствата
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 05/11/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9002913"
- "11187"
ms.openlocfilehash: 13865acb75b60a824c1dde9427c11471e980ea9e
ms.sourcegitcommit: ab75f66355116e995b3cb5505465b31989339e28
ms.translationtype: MT
ms.contentlocale: bg-BG
ms.lasthandoff: 08/13/2021
ms.locfileid: "58324433"
---
# <a name="issues-with-removing-an-offboarded-or-decommissioned-device-from-the-device-inventory"></a>Проблеми с премахването на изключено или изведено от експлоатация устройство от наличностите на устройствата

Microsoft Defender за крайна точка в момента не позволява ръчно премахване на записа на устройството на изключено или изведено от експлоатация устройство от инвентара на устройството.

За целите на защитата устройството остава в портала като исторически запис за до 180 дни. Данните на устройството обаче се изчистват според конфигурирания период на съхранение.

**Забележка:** Дезактивиран или дезактивиран уред се превключва автоматично на **Неактивно** състояние след седем дни. Освен това устройствата, които не са активни през последните 30 дни, не се вземат предвид в данните, които отразяват вашата организация Threat and Vulnerability Management на експозицията или защитения резултат на Microsoft за устройства.
 
Ако все още не искате да виждате определени устройства в изгледа "Наличности на устройства", опитайте да поставите етикет на устройство, за да филтрирате изведеното от експлоатация устройство от изгледа Наличности на устройства.

За повече информация вижте:

[Устройства offboard от услугата Microsoft Defender за крайна точка](https://docs.microsoft.com/microsoft-365/security/defender-endpoint/offboard-machines.md)

[Оценка на експозицията в Threat and Vulnerability Management](https://docs.microsoft.com/microsoft-365/security/defender-endpoint/tvm-exposure-score.md)

[Коригиране на нездравостови сензори в Microsoft Defender за крайна точка](https://docs.microsoft.com/microsoft-365/security/defender-endpoint/fix-unhealthy-sensors#inactive-devices.md)

[Как да използвате ефективно маркирането (част 1)](https://techcommunity.microsoft.com/t5/microsoft-defender-for-endpoint/how-to-use-tagging-effectively-part-1/ba-p/1964058)

[Как да използвате ефективно маркирането (част 2)](https://techcommunity.microsoft.com/t5/microsoft-defender-for-endpoint/how-to-use-tagging-effectively-part-2/ba-p/1962008)

[Как да използвате ефективно маркирането (част 3)](https://techcommunity.microsoft.com/t5/microsoft-defender-for-endpoint/how-to-use-tagging-effectively-part-3/ba-p/1964073)




