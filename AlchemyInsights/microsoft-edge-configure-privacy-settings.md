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
# <a name="microsoft-edge-configure-privacy-settings"></a><span data-ttu-id="fcd73-102">Настройки за поверителност на Microsoft Edge конфигурирайте</span><span class="sxs-lookup"><span data-stu-id="fcd73-102">Microsoft Edge configure privacy settings</span></span>

<span data-ttu-id="fcd73-103">По подразбиране, ако Microsoft Edge е разположен на платформи, които не са на Windows, не се изпращат диагностични данни и информация за сайта на Microsoft.</span><span class="sxs-lookup"><span data-stu-id="fcd73-103">By default, if Microsoft Edge is deployed on non-Windows platforms, diagnostic data and site information are not sent to Microsoft.</span></span> <span data-ttu-id="fcd73-104">Ако обаче Microsoft Edge е разположен в Windows 10, се изпращат диагностични данни и информация за сайта според [настройките за диагностични данни в Windows](https://docs.microsoft.com/windows/privacy/configure-windows-diagnostic-data-in-your-organization).</span><span class="sxs-lookup"><span data-stu-id="fcd73-104">However, if Microsoft Edge is deployed on Windows 10, diagnostic data and site information are sent according to users' [Windows Diagnostic data settings](https://docs.microsoft.com/windows/privacy/configure-windows-diagnostic-data-in-your-organization).</span></span>

<span data-ttu-id="fcd73-105">За да конфигурирате как Microsoft Edge управлява събирането на данни за вашата организация, използвайте следните групови правила:</span><span class="sxs-lookup"><span data-stu-id="fcd73-105">To configure how Microsoft Edge handles data collection for your organization, use the following group policies:</span></span>
- <span data-ttu-id="fcd73-106">[MetricsReportingEnabled](https://docs.microsoft.com/DeployEdge/microsoft-edge-policies#metricsreportingenabled): тези правила разрешават отчитането на данни за използване и сривове.</span><span class="sxs-lookup"><span data-stu-id="fcd73-106">[MetricsReportingEnabled](https://docs.microsoft.com/DeployEdge/microsoft-edge-policies#metricsreportingenabled): This policy enables reporting of usage and crash-related data.</span></span>
- <span data-ttu-id="fcd73-107">[SendSiteInfoToImproveServices](https://docs.microsoft.com/DeployEdge/microsoft-edge-policies#sendsiteinfotoimproveservices): тези правила изпращат информация за сайта, която се използва за подобряване на услугите на Microsoft.</span><span class="sxs-lookup"><span data-stu-id="fcd73-107">[SendSiteInfoToImproveServices](https://docs.microsoft.com/DeployEdge/microsoft-edge-policies#sendsiteinfotoimproveservices): This policy sends site information that is used to improve Microsoft services.</span></span>

<span data-ttu-id="fcd73-108">За да научите повече, вижте [Конфигуриране на настройките за правилата](https://docs.microsoft.com/deployedge/microsoft-edge-enterprise-privacy-settings#configure-policy-settings).</span><span class="sxs-lookup"><span data-stu-id="fcd73-108">To learn more, see [Configure policy settings](https://docs.microsoft.com/deployedge/microsoft-edge-enterprise-privacy-settings#configure-policy-settings).</span></span>