---
title: Помощ за настройката за нощно осветление
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9005578"
- "9930"
ms.openlocfilehash: db551db6edab7fca1cb465cf466575a2dbcd755e
ms.sourcegitcommit: 1f43598a726cdb9904aa501eb8db87f143020d9e
ms.translationtype: MT
ms.contentlocale: bg-BG
ms.lasthandoff: 03/23/2021
ms.locfileid: "51404199"
---
# <a name="help-with-the-night-light-display-setting"></a><span data-ttu-id="e49c4-102">Помощ за настройката за нощно осветление</span><span class="sxs-lookup"><span data-stu-id="e49c4-102">Help with the night light display setting</span></span>

<span data-ttu-id="e49c4-103">За да научите повече за настройките за нощно показване, вижте [Задаване на дисплея за нощно време в Windows 10](https://support.microsoft.com/windows/set-your-display-for-night-time-in-windows-10-18fe903a-e0a1-8326-4c68-fd23d7aaf136).</span><span class="sxs-lookup"><span data-stu-id="e49c4-103">To learn more about night time display settings, see [Set your display for night time in Windows 10](https://support.microsoft.com/windows/set-your-display-for-night-time-in-windows-10-18fe903a-e0a1-8326-4c68-fd23d7aaf136).</span></span>

<span data-ttu-id="e49c4-104">Ако опциите за нощно осветление са сиви в Настройки, проверете драйвера на дисплея:</span><span class="sxs-lookup"><span data-stu-id="e49c4-104">If the night light options are grayed out in Settings, check your display driver:</span></span> 

1. <span data-ttu-id="e49c4-105">Щракнете върху полето за търсене в лентата на задачите и въведете **Диспечер на устройствата** и след това изберете Диспечер на **устройствата** в резултатите от търсенето.</span><span class="sxs-lookup"><span data-stu-id="e49c4-105">Click the search box on your taskbar and type **Device Manager**, and then select **Device Manager** in the search results.</span></span>
1. <span data-ttu-id="e49c4-106">Разгънете **Адаптери за дисплей**.</span><span class="sxs-lookup"><span data-stu-id="e49c4-106">Expand **Display adapters**.</span></span> 

<span data-ttu-id="e49c4-107">За съжаление, функцията за нощно осветление не е налична, ако вашето устройство използва драйвер на DisplayLink или драйвер за basic Display.</span><span class="sxs-lookup"><span data-stu-id="e49c4-107">Unfortunately, the night light feature is not available if your device uses a DisplayLink driver or a Basic Display driver.</span></span>

<span data-ttu-id="e49c4-108">Функцията за нощно осветление използва най-новата графична технология, така че може да се наложи да актуализирате драйвера на дисплея:</span><span class="sxs-lookup"><span data-stu-id="e49c4-108">The night light feature makes use of recent graphics technology, so you might need to update your display driver:</span></span>  

- <span data-ttu-id="e49c4-109">Проверете за актуализации, като изберете Стартиране **на**  >  **актуализирането**  >  **на настройките & проверка на**  >  **windows Update** за актуализации на  >  **Windows**.</span><span class="sxs-lookup"><span data-stu-id="e49c4-109">Check for updates by going to **Start** > **Settings** > **Update & Security** > **Windows Update** > **Check for Updates**.</span></span>  

<span data-ttu-id="e49c4-110">ИЛИ</span><span class="sxs-lookup"><span data-stu-id="e49c4-110">OR</span></span>

- <span data-ttu-id="e49c4-111">Посетете уеб сайта за поддръжка на производителя на хардуера, за да изтеглите и инсталирате ръчно най-новите драйвери за показване.</span><span class="sxs-lookup"><span data-stu-id="e49c4-111">Visit your hardware manufacturer's support website to manually download and install the latest display drivers.</span></span>

## <a name="reset-night-light-in-the-registry"></a><span data-ttu-id="e49c4-112">Нулиране на нощното осветление в системния регистър</span><span class="sxs-lookup"><span data-stu-id="e49c4-112">Reset night light in the registry</span></span>

<span data-ttu-id="e49c4-113">Ако актуализирането на драйвера на дисплея не работи, може да се наложи да нулирате нощното осветление в системния регистър.</span><span class="sxs-lookup"><span data-stu-id="e49c4-113">If updating your display driver didn't work, you might need to reset night light in the registry.</span></span>  

<span data-ttu-id="e49c4-114">**Внимание:** Тази стъпка за отстраняване на неизправности се препоръчва само за напреднали потребители.</span><span class="sxs-lookup"><span data-stu-id="e49c4-114">**Caution:** This troubleshooting step is recommended only for advanced users.</span></span> <span data-ttu-id="e49c4-115">Ако промените системния регистър неправилно, може да възникнат сериозни проблеми.</span><span class="sxs-lookup"><span data-stu-id="e49c4-115">Serious problems can occur if you modify the registry incorrectly.</span></span> <span data-ttu-id="e49c4-116">За допълнителна защита архивирайте системния регистър, преди да го промените, така че да можете да го възстановите, ако възникнат проблеми.</span><span class="sxs-lookup"><span data-stu-id="e49c4-116">For added protection, back up the registry before you modify it so  you can restore it if problems occur.</span></span>

1. <span data-ttu-id="e49c4-117">В полето за търсене въведете **regedit и** след това изберете **Редактор на системния регистър** в резултатите от търсенето.</span><span class="sxs-lookup"><span data-stu-id="e49c4-117">In the search box, type **regedit**, and then select **Registry Editor** in the search results.</span></span>

1. <span data-ttu-id="e49c4-118">Отидете на следния ключ от системния регистър:</span><span class="sxs-lookup"><span data-stu-id="e49c4-118">Go to the following registry key:</span></span> 

    <span data-ttu-id="e49c4-119">HKEY_CURRENT_USER\Software\Microsoft\Windows\CurrentVersion\CloudStore\Store\Cache\DefaultAccount</span><span class="sxs-lookup"><span data-stu-id="e49c4-119">HKEY_CURRENT_USER\Software\Microsoft\Windows\CurrentVersion\CloudStore\Store\Cache\DefaultAccount</span></span>

1. <span data-ttu-id="e49c4-120">Експортирайте и след това изтрийте следния подключ:$$windows.data.bluelightreduction.bluelightreductionstate</span><span class="sxs-lookup"><span data-stu-id="e49c4-120">Export and then delete the following subkey:$$windows.data.bluelightreduction.bluelightreductionstate</span></span>

1. <span data-ttu-id="e49c4-121">Експортирайте и след това изтрийте следния подключ:$$windows.data.bluelightreduction.settings</span><span class="sxs-lookup"><span data-stu-id="e49c4-121">Export and then delete the following subkey:$$windows.data.bluelightreduction.settings</span></span>

1. <span data-ttu-id="e49c4-122">Рестартирайте Windows и проверете дали са налични опциите за нощно осветление.</span><span class="sxs-lookup"><span data-stu-id="e49c4-122">Restart Windows and verify if the night light options are available.</span></span>


