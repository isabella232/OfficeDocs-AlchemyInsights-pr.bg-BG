---
title: Настройки за поверителност на Microsoft Edge конфигурирайте
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
ms.openlocfilehash: dcd1d91dcde1f585caf0e1e3af30946513a0f26c
ms.sourcegitcommit: 94036315916fbc79dca2a692c2e9bc1139dd28f6
ms.translationtype: MT
ms.contentlocale: bg-BG
ms.lasthandoff: 12/08/2020
ms.locfileid: "49676835"
---
# <a name="microsoft-edge-configure-privacy-settings"></a>Настройки за поверителност на Microsoft Edge конфигурирайте

По подразбиране, ако Microsoft Edge е разположен на платформи, които не са на Windows, не се изпращат диагностични данни и информация за сайта на Microsoft. Ако обаче Microsoft Edge е разположен в Windows 10, се изпращат диагностични данни и информация за сайта според [настройките за диагностични данни в Windows](https://docs.microsoft.com/windows/privacy/configure-windows-diagnostic-data-in-your-organization).

За да конфигурирате как Microsoft Edge управлява събирането на данни за вашата организация, използвайте следните групови правила:
- [MetricsReportingEnabled](https://docs.microsoft.com/DeployEdge/microsoft-edge-policies#metricsreportingenabled): тези правила разрешават отчитането на данни за използване и сривове.
- [SendSiteInfoToImproveServices](https://docs.microsoft.com/DeployEdge/microsoft-edge-policies#sendsiteinfotoimproveservices): тези правила изпращат информация за сайта, която се използва за подобряване на услугите на Microsoft.

За да научите повече, вижте [Конфигуриране на настройките за правилата](https://docs.microsoft.com/deployedge/microsoft-edge-enterprise-privacy-settings#configure-policy-settings).