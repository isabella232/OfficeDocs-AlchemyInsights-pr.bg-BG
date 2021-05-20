---
title: Проблеми с премахването на изключено или изведено от експлоатация устройство от инвентара на устройството
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
ms.openlocfilehash: 46ac46c583cd0ac956797737d8150277f0d79ba5
ms.sourcegitcommit: c685f197dbf83a9dfd85e9acfdf14a4daf0e9a5a
ms.translationtype: MT
ms.contentlocale: bg-BG
ms.lasthandoff: 05/11/2021
ms.locfileid: "52564032"
---
# <a name="issues-with-removing-an-offboarded-or-decommissioned-device-from-the-device-inventory"></a><span data-ttu-id="b9cfc-102">Проблеми с премахването на изключено или изведено от експлоатация устройство от инвентара на устройството</span><span class="sxs-lookup"><span data-stu-id="b9cfc-102">Issues with removing an offboarded or decommissioned device from the Device Inventory</span></span>

<span data-ttu-id="b9cfc-103">Microsoft Defender за крайна точка в момента не позволява ръчно премахване на записа на устройството на изключено или изведено от експлоатация устройство от инвентара на устройството.</span><span class="sxs-lookup"><span data-stu-id="b9cfc-103">Microsoft Defender for Endpoint does not currently allow manually removing the device record of an offboarded or decommissioned device from the Device Inventory.</span></span>

<span data-ttu-id="b9cfc-104">За целите на защитата устройството остава в портала като исторически запис за до 180 дни.</span><span class="sxs-lookup"><span data-stu-id="b9cfc-104">For security purposes, the device remains in the portal as an historical record for up to 180 days.</span></span> <span data-ttu-id="b9cfc-105">Данните на устройството обаче се изчистват според конфигурирания период на съхранение.</span><span class="sxs-lookup"><span data-stu-id="b9cfc-105">However, the device data is purged according to your configured retention period.</span></span>

<span data-ttu-id="b9cfc-106">**Забележка:** Дезактивиран или дезактивиран уред се превключва автоматично на **Неактивно** състояние след седем дни.</span><span class="sxs-lookup"><span data-stu-id="b9cfc-106">**Note:** An offboarded or decommissioned device switches automatically to **Inactive** state after seven days.</span></span> <span data-ttu-id="b9cfc-107">Освен това устройствата, които не са активни през последните 30 дни, не се вземат предвид в данните, които отразяват вашата организация Threat and Vulnerability Management оценка на експозицията или Microsoft Secure Score за устройства.</span><span class="sxs-lookup"><span data-stu-id="b9cfc-107">In addition, devices not active in the last 30 days are not factored into the data that reflects your organization threat and vulnerability management exposure score or Microsoft Secure Score for Devices.</span></span>
 
<span data-ttu-id="b9cfc-108">Ако все още не искате да виждате определени устройства в изгледа "Наличности на устройства", опитайте да поставите етикет на устройство, за да филтрирате изведеното от експлоатация устройство от изгледа Наличности на устройства.</span><span class="sxs-lookup"><span data-stu-id="b9cfc-108">If you still don't want to see certain devices in Device Inventory view, try placing a device tag to filter out the decommissioned device from the Device Inventory view.</span></span>

<span data-ttu-id="b9cfc-109">За повече информация вижте:</span><span class="sxs-lookup"><span data-stu-id="b9cfc-109">For more information, see:</span></span>

[<span data-ttu-id="b9cfc-110">Offboard devices from the Microsoft Defender for Endpoint service</span><span class="sxs-lookup"><span data-stu-id="b9cfc-110">Offboard devices from the Microsoft Defender for Endpoint service</span></span>](/microsoft-365/security/defender-endpoint/offboard-machines.md)

[<span data-ttu-id="b9cfc-111">Оценка на експозицията в Threat and Vulnerability Management</span><span class="sxs-lookup"><span data-stu-id="b9cfc-111">Exposure score in threat and vulnerability management</span></span>](/microsoft-365/security/defender-endpoint/tvm-exposure-score.md)

[<span data-ttu-id="b9cfc-112">Коригиране на нездравостови сензори в Microsoft Defender за крайна точка</span><span class="sxs-lookup"><span data-stu-id="b9cfc-112">Fix unhealthy sensors in Microsoft Defender for Endpoint</span></span>](/microsoft-365/security/defender-endpoint/fix-unhealthy-sensors#inactive-devices.md)

[<span data-ttu-id="b9cfc-113">Как да използвате ефективно маркирането (част 1)</span><span class="sxs-lookup"><span data-stu-id="b9cfc-113">How to use tagging effectively (Part 1)</span></span>](https://techcommunity.microsoft.com/t5/microsoft-defender-for-endpoint/how-to-use-tagging-effectively-part-1/ba-p/1964058)

[<span data-ttu-id="b9cfc-114">Как да използвате ефективно маркирането (част 2)</span><span class="sxs-lookup"><span data-stu-id="b9cfc-114">How to use tagging effectively (Part 2)</span></span>](https://techcommunity.microsoft.com/t5/microsoft-defender-for-endpoint/how-to-use-tagging-effectively-part-2/ba-p/1962008)

[<span data-ttu-id="b9cfc-115">Как да използвате ефективно маркирането (част 3)</span><span class="sxs-lookup"><span data-stu-id="b9cfc-115">How to use tagging effectively (Part 3)</span></span>](https://techcommunity.microsoft.com/t5/microsoft-defender-for-endpoint/how-to-use-tagging-effectively-part-3/ba-p/1964073)




