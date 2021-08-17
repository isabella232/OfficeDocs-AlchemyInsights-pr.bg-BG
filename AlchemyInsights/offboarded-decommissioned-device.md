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
ms.openlocfilehash: 6eb59d16a1dab2de0e7a44faf9b34be6432342f9e20c94b6932e69e937751add
ms.sourcegitcommit: 920051182781bd97ce4d4d6fbd268cb37b84d239
ms.translationtype: MT
ms.contentlocale: bg-BG
ms.lasthandoff: 08/11/2021
ms.locfileid: "57891992"
---
# <a name="issues-with-removing-an-offboarded-or-decommissioned-device-from-the-device-inventory"></a>Проблеми с премахването на изключено или изведено от експлоатация устройство от наличностите на устройствата

Microsoft Defender за крайна точка в момента не позволява ръчно премахване на записа на устройството на изключено или изведено от експлоатация устройство от инвентара на устройството.

За целите на защитата устройството остава в портала като исторически запис за до 180 дни. Данните на устройството обаче се изчистват според конфигурирания период на съхранение.

**Забележка:** Дезактивиран или дезактивиран уред се превключва автоматично в **неактивно** състояние след седем дни. Освен това устройствата, които не са активни през последните 30 дни, не се вземат предвид в данните, които отразяват вашата организация Threat and Vulnerability Management оценка на експозицията или Защитен резултат на Microsoft за устройства.
 
Ако все още не искате да виждате определени устройства в изгледа "Наличности на устройства", опитайте да поставите етикет на устройство, за да филтрирате изведеното от експлоатация устройство от изгледа Наличности на устройства.

За повече информация вижте:

[Устройства offboard от услугата Microsoft Defender за крайна точка](https://docs.microsoft.com/microsoft-365/security/defender-endpoint/offboard-machines.md)

[Оценка на експозицията в Threat and Vulnerability Management](https://docs.microsoft.com/microsoft-365/security/defender-endpoint/tvm-exposure-score.md)

[Коригиране на нездравостови сензори в Microsoft Defender за крайна точка](https://docs.microsoft.com/microsoft-365/security/defender-endpoint/fix-unhealthy-sensors#inactive-devices.md)

[Как да използвате ефективно маркирането (част 1)](https://techcommunity.microsoft.com/t5/microsoft-defender-for-endpoint/how-to-use-tagging-effectively-part-1/ba-p/1964058)

[Как да използвате ефективно маркирането (част 2)](https://techcommunity.microsoft.com/t5/microsoft-defender-for-endpoint/how-to-use-tagging-effectively-part-2/ba-p/1962008)

[Как да използвате ефективно маркирането (част 3)](https://techcommunity.microsoft.com/t5/microsoft-defender-for-endpoint/how-to-use-tagging-effectively-part-3/ba-p/1964073)




