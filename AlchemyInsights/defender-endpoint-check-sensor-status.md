---
title: Състояние на сензора за проверка на крайната точка на защитника
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 05/21/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "11084"
- "9003537"
ms.openlocfilehash: a53a0109c3b974806d04135dd2c102de81ec560f
ms.sourcegitcommit: ded29f44e5019b1929218b02733b390899843680
ms.translationtype: MT
ms.contentlocale: bg-BG
ms.lasthandoff: 05/24/2021
ms.locfileid: "52676040"
---
# <a name="defender-endpoint-check-sensor-status"></a><span data-ttu-id="2dc7c-102">Състояние на сензора за проверка на крайната точка на защитника</span><span class="sxs-lookup"><span data-stu-id="2dc7c-102">Defender Endpoint check sensor status</span></span>

<span data-ttu-id="2dc7c-103">Плочката **Устройства с проблеми със сензора** се намира на таблото "Операции за защита".</span><span class="sxs-lookup"><span data-stu-id="2dc7c-103">The **Devices with sensor issues** tile is located on the Security Operations dashboard.</span></span> <span data-ttu-id="2dc7c-104">Тази плочка предоставя информация за възможността на отделното устройство да предоставя данни от сензори и да комуникира с услугата Defender for Endpoint.</span><span class="sxs-lookup"><span data-stu-id="2dc7c-104">This tile provides information on the individual device’s ability to provide sensor data and communicate with the Defender for Endpoint service.</span></span> <span data-ttu-id="2dc7c-105">Той съобщава колко устройства изискват внимание и ви помага да идентифицирате проблемни устройства и да предприемете действия за коригиране на известни проблеми.</span><span class="sxs-lookup"><span data-stu-id="2dc7c-105">It reports how many devices require attention and helps you identify problematic devices and take action to correct known issues.</span></span>

<span data-ttu-id="2dc7c-106">Два индикатора за състоянието на плочката предоставят информация за броя на устройствата, които не се докладват правилно на услугата:</span><span class="sxs-lookup"><span data-stu-id="2dc7c-106">Two status indicators on the tile provide information on the number of devices not reporting properly to the service:</span></span>

- <span data-ttu-id="2dc7c-107">**Неправилно конфигурирани** Устройства, които може частично да докладват данни на сензора на услугата Defender for Endpoint и може да имат грешки в конфигурацията, които трябва да бъдат коригирани.</span><span class="sxs-lookup"><span data-stu-id="2dc7c-107">**Misconfigured** Devices that might partially be reporting sensor data to the Defender for Endpoint service and might have configuration errors that need to be corrected.</span></span>
- <span data-ttu-id="2dc7c-108">**Неактивен** Устройства, които са спрели да докладват на услугата Defender for Endpoint за повече от седем дни през последния месец.</span><span class="sxs-lookup"><span data-stu-id="2dc7c-108">**Inactive** Devices that have stopped reporting to the Defender for Endpoint service for more than seven days in the past month.</span></span>

<span data-ttu-id="2dc7c-109">Щракването върху някоя от групите ви насочва към списъка Устройства, филтрирано според вашите възможности за избор.</span><span class="sxs-lookup"><span data-stu-id="2dc7c-109">Clicking any of the groups directs you to Devices list, filtered according to your choices.</span></span> <span data-ttu-id="2dc7c-110">В списъка Устройства можете да филтрирате списъка за изздравителни състояния по следното състояние:</span><span class="sxs-lookup"><span data-stu-id="2dc7c-110">On the Devices list, you can filter the health state list by the following status:</span></span>

- <span data-ttu-id="2dc7c-111">**Активни** Устройства, които се докладват активно на услугата Defender for Endpoint.</span><span class="sxs-lookup"><span data-stu-id="2dc7c-111">**Active** Devices that are actively reporting to the Defender for Endpoint service.</span></span>
- <span data-ttu-id="2dc7c-112">**Неправилно конфигурирани** Устройства, които може частично да докладват данни от сензор на услугата Defender for Endpoint, но имат грешки в конфигурацията, които трябва да бъдат коригирани.</span><span class="sxs-lookup"><span data-stu-id="2dc7c-112">**Misconfigured** Devices that might partially be reporting sensor data to the Defender for Endpoint service but have configuration errors that need to be corrected.</span></span> <span data-ttu-id="2dc7c-113">Неправилно конфигурираните устройства могат да имат един или комбинация от следните проблеми:</span><span class="sxs-lookup"><span data-stu-id="2dc7c-113">Misconfigured devices can have either one or a combination of the following issues:</span></span>

    - <span data-ttu-id="2dc7c-114">Без данни от сензора – Устройствата спряха да изпращат данни от сензора.</span><span class="sxs-lookup"><span data-stu-id="2dc7c-114">No sensor data - Devices has stopped sending sensor data.</span></span> <span data-ttu-id="2dc7c-115">От устройството могат да се активират ограничени предупреждения.</span><span class="sxs-lookup"><span data-stu-id="2dc7c-115">Limited alerts can be triggered from the device.</span></span>
    - <span data-ttu-id="2dc7c-116">Нарушена комуникация – възможността за комуникация с устройството е нарушена.</span><span class="sxs-lookup"><span data-stu-id="2dc7c-116">Impaired communications - Ability to communicate with device is impaired.</span></span> <span data-ttu-id="2dc7c-117">Изпращането на файлове за задълбочен анализ, блокирането на файлове, изтощаване на устройство от мрежата и други действия, които изискват комуникация с устройството, може да не работи.</span><span class="sxs-lookup"><span data-stu-id="2dc7c-117">Sending files for deep analysis, blocking files, isolating device from network and other actions that require communication with the device may not work.</span></span>
- <span data-ttu-id="2dc7c-118">**Неактивен** Устройства, които са спрели отчитането на услугата Defender for Endpoint.</span><span class="sxs-lookup"><span data-stu-id="2dc7c-118">**Inactive** Devices that have stopped reporting to the Defender for Endpoint service.</span></span>

<span data-ttu-id="2dc7c-119">Можете да изтеглите целия списък в CSV формат с помощта на функцията Експортиране.</span><span class="sxs-lookup"><span data-stu-id="2dc7c-119">You can download the entire list in CSV format using the Export feature.</span></span>

<span data-ttu-id="2dc7c-120">За повече информация вижте Проверка на [състоянието на из изтезания на сензора в Microsoft Defender за крайна точка.](/microsoft-365/security/defender-endpoint/check-sensor-status)</span><span class="sxs-lookup"><span data-stu-id="2dc7c-120">For more information, see [Check sensor health state in Microsoft Defender for Endpoint](/microsoft-365/security/defender-endpoint/check-sensor-status).</span></span>

<span data-ttu-id="2dc7c-121">За повече информация какво е причинило неактивни или неправилно конфигурирани устройства, вижте Коригиране на [нездравостови](/microsoft-365/security/defender-endpoint/fix-unhealthy-sensors)сензори в Microsoft Defender за крайна точка .</span><span class="sxs-lookup"><span data-stu-id="2dc7c-121">For more information about what caused a device to be inactive or misconfigured, see [Fix unhealthy sensors in Microsoft Defender for Endpoint](/microsoft-365/security/defender-endpoint/fix-unhealthy-sensors).</span></span>
