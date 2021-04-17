---
title: Отстраняване на неизправности със съществуващ монитор
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3454"
- "9001450"
ms.openlocfilehash: c4d2bb64b6b5ea79d4cd585e2be85c3c17e0f76f
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: bg-BG
ms.lasthandoff: 04/15/2021
ms.locfileid: "51824568"
---
# <a name="troubleshoot-an-existing-monitor"></a><span data-ttu-id="01d41-102">Отстраняване на неизправности със съществуващ монитор</span><span class="sxs-lookup"><span data-stu-id="01d41-102">Troubleshoot an existing monitor</span></span>

<span data-ttu-id="01d41-103">Изпробвайте тези решения, за да отстраните неизправности с монитор.</span><span class="sxs-lookup"><span data-stu-id="01d41-103">Try these solutions to troubleshoot a monitor.</span></span> 

<span data-ttu-id="01d41-104">**Обновяване на дисплея на монитора:**</span><span class="sxs-lookup"><span data-stu-id="01d41-104">**Refresh your monitor's display:**</span></span>

<span data-ttu-id="01d41-105">Едновременно с това натиснете следните клавиши: Клавиш windows + Ctrl + Shift + B. Това ще обнови комуникацията с вашия графичен драйвер.</span><span class="sxs-lookup"><span data-stu-id="01d41-105">Press the following keys at the same time: Windows Key  + Ctrl + Shift + B. This will refresh communication with your graphics driver.</span></span> <span data-ttu-id="01d41-106">Мониторите ви ще мигат мигове и ще се върнат след няколко секунди.</span><span class="sxs-lookup"><span data-stu-id="01d41-106">Your monitors will blink momentarily and come back after a few seconds.</span></span>

<span data-ttu-id="01d41-107">**Отстраняване на неизправности с хардуера на монитора:**</span><span class="sxs-lookup"><span data-stu-id="01d41-107">**Troubleshoot monitor hardware:**</span></span>

1. <span data-ttu-id="01d41-108">Изключете кабела, който свързва компютъра към монитора, и го включете отново.</span><span class="sxs-lookup"><span data-stu-id="01d41-108">Unplug the cable connecting your PC to your monitor, and plug it back in.</span></span>
2. <span data-ttu-id="01d41-109">Изключете всички несъществени устройства от вашия компютър (например адаптери или докинг станция).</span><span class="sxs-lookup"><span data-stu-id="01d41-109">Disconnect any non-essential devices from your PC (such as adapters or docks).</span></span>

<span data-ttu-id="01d41-110">**Ако наскоро сте инсталирали актуализация на вашия компютър, можете да върнете драйвера на дисплея:**</span><span class="sxs-lookup"><span data-stu-id="01d41-110">**If you recently installed an update on your PC, you can roll back your display driver:**</span></span>

1. <span data-ttu-id="01d41-111">Изберете **Старт**, въведете **диспечера на устройствата** и изберете Диспечер на **устройствата** от резултатите.</span><span class="sxs-lookup"><span data-stu-id="01d41-111">Select **Start**, type **device manager**, and select **Device Manager** from the results.</span></span>
2. <span data-ttu-id="01d41-112">Разгънете **секцията Адаптери за** дисплей, щракнете с десния бутон върху видеокартата и изберете **Свойства**.</span><span class="sxs-lookup"><span data-stu-id="01d41-112">Expand the **Display adapters** section, right-click your display adapter, ands select **Properties**.</span></span>
3. <span data-ttu-id="01d41-113">Навигирайте **до раздела** Драйвер и изберете **Връщане на драйвера .**</span><span class="sxs-lookup"><span data-stu-id="01d41-113">Navigate to the **Driver** tab and select **Roll Back Driver**.</span></span> <br>
<span data-ttu-id="01d41-114">Забележка: Ако това не е налично или е в сиво, изберете **Не** от опциите по-долу, за да преминете към следващата стъпка.</span><span class="sxs-lookup"><span data-stu-id="01d41-114">Note: If this isn't available or is grayed out, select **No** from the options below to move to the next step.</span></span>
4. <span data-ttu-id="01d41-115">Може да се наложи да рестартирате компютъра, преди тези промени да влязат в сила.</span><span class="sxs-lookup"><span data-stu-id="01d41-115">You may need to restart your PC before these changes take effect.</span></span>

<span data-ttu-id="01d41-116">**Деинсталирайте и преинсталирайте драйвера на дисплея:**</span><span class="sxs-lookup"><span data-stu-id="01d41-116">**Uninstall and reinstall your display driver:**</span></span>

1. <span data-ttu-id="01d41-117">Изберете **Старт**, въведете **диспечера на устройствата** и изберете Диспечер на **устройствата** от резултатите.</span><span class="sxs-lookup"><span data-stu-id="01d41-117">Select **Start**, type **device manager**, and select **Device Manager** from the results.</span></span>
2. <span data-ttu-id="01d41-118">Разгънете **секцията Адаптери за** дисплей, щракнете с десния бутон върху видеокартата и изберете **Деинсталиране на устройство**.</span><span class="sxs-lookup"><span data-stu-id="01d41-118">Expand the **Display adapters** section, right-click your display adapter, ands select **Uninstall device**.</span></span> 
3. <span data-ttu-id="01d41-119">Изберете полето до Изтриване на **софтуера на драйвера за това устройство и** изберете **Деинсталиране**.</span><span class="sxs-lookup"><span data-stu-id="01d41-119">Select the box next to **Delete the driver software for this device** and select **Uninstall**.</span></span><br>
<span data-ttu-id="01d41-120">Забележка: Може да бъдете помолени да рестартирате компютъра си на този етап.</span><span class="sxs-lookup"><span data-stu-id="01d41-120">Note: You may be asked to restart your computer at this stage.</span></span> <span data-ttu-id="01d41-121">Не забравяйте да запишете останалите инструкции, преди да рестартирате.</span><span class="sxs-lookup"><span data-stu-id="01d41-121">Make sure to write down the remaining instructions before you restart.</span></span>
4. <span data-ttu-id="01d41-122">Отворете диспечера на устройствата отново.</span><span class="sxs-lookup"><span data-stu-id="01d41-122">Open Device Manager again.</span></span>
5. <span data-ttu-id="01d41-123">Разгънете **секцията Адаптери за** дисплей, щракнете с десния бутон върху видеокартата и изберете Актуализиране **на драйвера**.</span><span class="sxs-lookup"><span data-stu-id="01d41-123">Expand the **Display adapters** section, right-click on your display adapter, and select **Update Driver**.</span></span>
6. <span data-ttu-id="01d41-124">Изберете **Автоматично търсене на софтуер за актуализиране на драйвера** и следвайте инструкциите за инсталиране.</span><span class="sxs-lookup"><span data-stu-id="01d41-124">Select **Search automatically for update driver software** and follow the installation instructions.</span></span>