---
title: Инвентаризация на устройствата
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/27/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "1281"
- "6700008"
ms.openlocfilehash: d59ee014a64de39d01837e90909619f30ec35e89
ms.sourcegitcommit: e34bb95fb93250f1dc7aec6a13578bb3bb355935
ms.translationtype: MT
ms.contentlocale: bg-BG
ms.lasthandoff: 07/28/2020
ms.locfileid: "45438915"
---
# <a name="intune-device-inventory"></a><span data-ttu-id="12776-102">Инвентаризация на устройствата</span><span class="sxs-lookup"><span data-stu-id="12776-102">Intune Device Inventory</span></span>

<span data-ttu-id="12776-103">Blade Devices предоставя администраторски поглед върху устройствата, които се управляват в Intune на база устройство.</span><span class="sxs-lookup"><span data-stu-id="12776-103">The Devices blade provides the administrator insight into devices under management in Intune on a per device basis.</span></span> <span data-ttu-id="12776-104">Информацията, която се показва, включва: Хардуер, открити приложения, състояние на съответствие на устройството и състояние на конфигуриране на устройството.</span><span class="sxs-lookup"><span data-stu-id="12776-104">The information shown includes: Hardware, Discovered applications, Device Compliance state, and Device Configuration state.</span></span>

<span data-ttu-id="12776-105">Инвентаризационни данни за хардуер и открити приложения се събират на седемдневен цикъл.</span><span class="sxs-lookup"><span data-stu-id="12776-105">Inventory data for hardware and discovered applications is collected on a seven-day cycle.</span></span> <span data-ttu-id="12776-106">Приложенията и конкретните елементи на хардуера се различават в зависимост от операционната система на устройството и дали устройството е лично или корпоративно притежавано.</span><span class="sxs-lookup"><span data-stu-id="12776-106">The applications and specific elements of hardware reported differ depending on the device operating system and whether the device is personally or corporate owned.</span></span>

<span data-ttu-id="12776-107">За повече информация вижте [Подробности за устройството в Intune](https://docs.microsoft.com/intune/device-inventory).</span><span class="sxs-lookup"><span data-stu-id="12776-107">For more information, see [See device details in Intune](https://docs.microsoft.com/intune/device-inventory).</span></span>

<span data-ttu-id="12776-108">**ЧЗВ**</span><span class="sxs-lookup"><span data-stu-id="12776-108">**FAQ**</span></span>

<span data-ttu-id="12776-109">Q: Аз не получавам пълен списък на приложенията, налични на Intune включени Windows устройства.</span><span class="sxs-lookup"><span data-stu-id="12776-109">Q: I am not receiving a full inventory list of applications present on Intune-enrolled Windows devices.</span></span> <span data-ttu-id="12776-110">Защо не?</span><span class="sxs-lookup"><span data-stu-id="12776-110">Why not?</span></span>

<span data-ttu-id="12776-111">О: По това време само модерните приложения са изброени за компютри с Windows 10, които са идентифицирани като корпоративни устройства.</span><span class="sxs-lookup"><span data-stu-id="12776-111">A: At this time, only modern apps are listed for Windows 10 PCs that are identified as corporate devices.</span></span> <span data-ttu-id="12776-112">Intune не събира информация за Win32 приложения, инсталирани на тези устройства.</span><span class="sxs-lookup"><span data-stu-id="12776-112">Intune doesn't collect information about Win32 apps installed on these devices.</span></span>

<span data-ttu-id="12776-113">Q: Защо телефонните номера не се събират от всички устройства?</span><span class="sxs-lookup"><span data-stu-id="12776-113">Q: Why are phone numbers not collected from all devices?</span></span>

<span data-ttu-id="12776-114">A: телефони, категоризирани като корпоративни устройства в Intune не са идентифицирани с пълния си телефонен номер, когато например стартирате отчет за наличност на мобилни устройства.</span><span class="sxs-lookup"><span data-stu-id="12776-114">A: Phones categorized as corporate devices in Intune are not identified with their full phone number when, for example, you run a mobile device inventory report.</span></span> <span data-ttu-id="12776-115">Телефонните номера на собственото устройство винаги са частично маскирани със звездички (\*\*\*\*) и показват само последните четири цифри.</span><span class="sxs-lookup"><span data-stu-id="12776-115">Bring-you-own-device phone numbers are always partially masked with asterisks (\*\*\*\*), and show only the last four digits.</span></span>