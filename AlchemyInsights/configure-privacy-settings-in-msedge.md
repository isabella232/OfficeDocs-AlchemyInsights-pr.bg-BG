---
title: Конфигуриране на настройките за поверителност в Microsoft Edge
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 03/24/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004632"
- "8367"
ms.openlocfilehash: 991f323249e15abd137c3e69b400e40503ed30dec6507cc5071a0b1af7f72bb3
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: bg-BG
ms.lasthandoff: 08/05/2021
ms.locfileid: "54090287"
---
# <a name="configure-privacy-settings-in-microsoft-edge"></a>Конфигуриране на настройките за поверителност в Microsoft Edge

По подразбиране, ако Microsoft Edge е разположена на платформи, които не са Windows, диагностичните данни и информацията за сайта не се изпращат на Microsoft. Ако обаче Microsoft Edge в Windows 10, диагностичните данни и информацията за сайта се изпращат според настройките [на Windows диагностични данни](https://go.microsoft.com/fwlink/?linkid=2132472)на потребителите.

За да конфигурирате как Microsoft Edge обработва събирането на данни за вашата организация, използвайте следните групови правила:
- [МетрикиReportingEnabled](https://go.microsoft.com/fwlink/?linkid=2132470) включва отчитането на данни, свързани с използването и сривовете.
- [SendSiteInfoToImproveServices](https://go.microsoft.com/fwlink/?linkid=2132470) изпраща информация за сайта, използвана за подобряване Услуги на Microsoft.

За да научите повече, вижте [Конфигуриране на настройките на правилата](https://go.microsoft.com/fwlink/?linkid=2132577).
