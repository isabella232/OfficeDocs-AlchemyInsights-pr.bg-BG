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
ms.openlocfilehash: 2367a7a55d1837fa7c7095fd0ac10ff1cf7ae72d
ms.sourcegitcommit: db908b3da2c7a6508a77bf4f2c80afb294fadbd1
ms.translationtype: MT
ms.contentlocale: bg-BG
ms.lasthandoff: 03/29/2021
ms.locfileid: "51404254"
---
# <a name="configure-privacy-settings-in-microsoft-edge"></a><span data-ttu-id="565b4-102">Конфигуриране на настройките за поверителност в Microsoft Edge</span><span class="sxs-lookup"><span data-stu-id="565b4-102">Configure privacy settings in Microsoft Edge</span></span>

<span data-ttu-id="565b4-103">По подразбиране, ако Microsoft Edge е разположен на платформи, които не са на Windows, диагностичните данни и информацията за сайта не се изпращат на Microsoft.</span><span class="sxs-lookup"><span data-stu-id="565b4-103">By default, if Microsoft Edge is deployed on non-Windows platforms, diagnostic data and site information aren't sent to Microsoft.</span></span> <span data-ttu-id="565b4-104">Ако обаче Microsoft Edge е разположен в Windows 10, диагностичните данни и информацията за сайта се изпращат според настройките на диагностичните данни [на Windows на потребителите.](https://go.microsoft.com/fwlink/?linkid=2132472)</span><span class="sxs-lookup"><span data-stu-id="565b4-104">However, if Microsoft Edge is deployed on Windows 10, diagnostic data and site information are sent according to users' [Windows Diagnostic data settings](https://go.microsoft.com/fwlink/?linkid=2132472).</span></span>

<span data-ttu-id="565b4-105">За да конфигурирате как Microsoft Edge обработва събирането на данни за вашата организация, използвайте следните групови правила:</span><span class="sxs-lookup"><span data-stu-id="565b4-105">To configure how Microsoft Edge handles data collection for your organization, use the following group policies:</span></span>
- <span data-ttu-id="565b4-106">[МетрикиReportingEnabled](https://go.microsoft.com/fwlink/?linkid=2132470) включва отчитането на данни, свързани с използването и сривовете.</span><span class="sxs-lookup"><span data-stu-id="565b4-106">[MetricsReportingEnabled](https://go.microsoft.com/fwlink/?linkid=2132470) turns on reporting of usage and crash-related data.</span></span>
- <span data-ttu-id="565b4-107">[SendSiteInfoToImproveServices изпраща информация](https://go.microsoft.com/fwlink/?linkid=2132470) за сайта, използвана за подобряване на услугите на Microsoft.</span><span class="sxs-lookup"><span data-stu-id="565b4-107">[SendSiteInfoToImproveServices](https://go.microsoft.com/fwlink/?linkid=2132470) sends site information used to improve Microsoft services.</span></span>

<span data-ttu-id="565b4-108">За да научите повече, вижте [Конфигуриране на настройките на правилата](https://go.microsoft.com/fwlink/?linkid=2132577).</span><span class="sxs-lookup"><span data-stu-id="565b4-108">To learn more, see [Configure policy settings](https://go.microsoft.com/fwlink/?linkid=2132577).</span></span>
