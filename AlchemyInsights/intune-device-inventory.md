---
title: Настройване на списъка с устройства
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/27/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "1281"
- "6700008"
ms.openlocfilehash: 5d2be7485be8578f7fdee3216dc6f3970be67fd1
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: bg-BG
ms.lasthandoff: 09/14/2020
ms.locfileid: "47667867"
---
# <a name="intune-device-inventory"></a><span data-ttu-id="afa60-102">Настройване на списъка с устройства</span><span class="sxs-lookup"><span data-stu-id="afa60-102">Intune Device Inventory</span></span>

<span data-ttu-id="afa60-103">Blade на устройства предоставя на администратора вникване в устройства под управление в съзвучие на база на устройство.</span><span class="sxs-lookup"><span data-stu-id="afa60-103">The Devices blade provides the administrator insight into devices under management in Intune on a per device basis.</span></span> <span data-ttu-id="afa60-104">Показаната информация включва: хардуер, открити приложения, състояние на съответствие на устройството и състояние на конфигурацията на устройството.</span><span class="sxs-lookup"><span data-stu-id="afa60-104">The information shown includes: Hardware, Discovered applications, Device Compliance state, and Device Configuration state.</span></span>

<span data-ttu-id="afa60-105">Данни за инвентаризация за хардуер и открити приложения се събират в седемдневен цикъл.</span><span class="sxs-lookup"><span data-stu-id="afa60-105">Inventory data for hardware and discovered applications is collected on a seven-day cycle.</span></span> <span data-ttu-id="afa60-106">Приложенията и определени елементи на хардуера се различават в зависимост от операционната система на устройството и дали устройството е лично или корпоративна собственост.</span><span class="sxs-lookup"><span data-stu-id="afa60-106">The applications and specific elements of hardware reported differ depending on the device operating system and whether the device is personally or corporate owned.</span></span>

<span data-ttu-id="afa60-107">За повече информация вижте [Вижте подробности за устройството в настройки](https://docs.microsoft.com/intune/device-inventory).</span><span class="sxs-lookup"><span data-stu-id="afa60-107">For more information, see [See device details in Intune](https://docs.microsoft.com/intune/device-inventory).</span></span>

<span data-ttu-id="afa60-108">**ЧЗВ**</span><span class="sxs-lookup"><span data-stu-id="afa60-108">**FAQ**</span></span>

<span data-ttu-id="afa60-109">В: не получавам пълен списък с налични приложения за приложенията, които са записани на устройства с Windows.</span><span class="sxs-lookup"><span data-stu-id="afa60-109">Q: I am not receiving a full inventory list of applications present on Intune-enrolled Windows devices.</span></span> <span data-ttu-id="afa60-110">Защо не?</span><span class="sxs-lookup"><span data-stu-id="afa60-110">Why not?</span></span>

<span data-ttu-id="afa60-111">А: към този момент само съвременните приложения са изброени за компютри с Windows 10, които се идентифицират като корпоративни устройства.</span><span class="sxs-lookup"><span data-stu-id="afa60-111">A: At this time, only modern apps are listed for Windows 10 PCs that are identified as corporate devices.</span></span> <span data-ttu-id="afa60-112">В "Настройки" не се събира информация за Win32 приложенията, инсталирани на тези устройства.</span><span class="sxs-lookup"><span data-stu-id="afa60-112">Intune doesn't collect information about Win32 apps installed on these devices.</span></span>

<span data-ttu-id="afa60-113">В: защо телефонните номера не се събират от всички устройства?</span><span class="sxs-lookup"><span data-stu-id="afa60-113">Q: Why are phone numbers not collected from all devices?</span></span>

<span data-ttu-id="afa60-114">А: телефони, категоризирани като корпоративни устройства в "ненастрои", не се идентифицират с пълния си телефонен номер, когато например стартирате отчет за инвентаризация на мобилно устройство.</span><span class="sxs-lookup"><span data-stu-id="afa60-114">A: Phones categorized as corporate devices in Intune are not identified with their full phone number when, for example, you run a mobile device inventory report.</span></span> <span data-ttu-id="afa60-115">Телефонните номера за собствено устройство винаги се маскират частично със звездички (\* \* \* \*) и показват само последните четири цифри.</span><span class="sxs-lookup"><span data-stu-id="afa60-115">Bring-you-own-device phone numbers are always partially masked with asterisks (\*\*\*\*), and show only the last four digits.</span></span>