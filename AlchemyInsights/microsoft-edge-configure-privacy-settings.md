---
title: Microsoft Edge конфигурирате настройките за поверителност
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 12/03/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9003843"
- "6892"
ms.openlocfilehash: 24721325aefd4a8c0dbeb7864ce6da637c4df932694d4b6fff80cab5bb5b4319
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: bg-BG
ms.lasthandoff: 08/05/2021
ms.locfileid: "54114161"
---
# <a name="microsoft-edge-configure-privacy-settings"></a>Microsoft Edge конфигурирате настройките за поверителност

По подразбиране, ако Microsoft Edge е разположена на платформи, които не са Windows, диагностичните данни и информацията за сайта не се изпращат на Microsoft. Ако обаче Microsoft Edge в Windows 10, диагностичните данни и информацията за сайта се изпращат според настройките [на Windows диагностични данни](https://docs.microsoft.com/windows/privacy/configure-windows-diagnostic-data-in-your-organization)на потребителите.

За да конфигурирате как Microsoft Edge обработва събирането на данни за вашата организация, използвайте следните групови правила:
- [МетрикиReportingEnabled:](https://docs.microsoft.com/DeployEdge/microsoft-edge-policies#metricsreportingenabled)Тези правила позволяват отчитане на данните, свързани с използването и сривовете.
- [SendSiteInfoToImproveServices](https://docs.microsoft.com/DeployEdge/microsoft-edge-policies#sendsiteinfotoimproveservices): Това правило изпраща информация за сайта, която се използва за подобряване на Услуги на Microsoft.

За да научите повече, вижте [Конфигуриране на настройките на правилата](https://docs.microsoft.com/deployedge/microsoft-edge-enterprise-privacy-settings#configure-policy-settings).