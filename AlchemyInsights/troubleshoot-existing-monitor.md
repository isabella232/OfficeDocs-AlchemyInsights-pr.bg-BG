---
title: Отстраняване на неизправности при съществуващ монитор
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3454"
- "9001450"
ms.openlocfilehash: d90baddd01bdf8508bd6289509c8399b8241887a
ms.sourcegitcommit: 42463e8d8869f36225a27388d83d37629c6b149e
ms.translationtype: MT
ms.contentlocale: bg-BG
ms.lasthandoff: 12/18/2019
ms.locfileid: "40738558"
---
# <a name="troubleshoot-an-existing-monitor"></a><span data-ttu-id="7ee51-102">Отстраняване на неизправности при съществуващ монитор</span><span class="sxs-lookup"><span data-stu-id="7ee51-102">Troubleshoot an existing monitor</span></span>

<span data-ttu-id="7ee51-103">Изпробвайте тези решения за отстраняване на неизправности на монитора.</span><span class="sxs-lookup"><span data-stu-id="7ee51-103">Try these solutions to troubleshoot a monitor.</span></span> 

<span data-ttu-id="7ee51-104">**Обновете дисплея на монитора:**</span><span class="sxs-lookup"><span data-stu-id="7ee51-104">**Refresh your monitor's display:**</span></span>

<span data-ttu-id="7ee51-105">Натиснете следните клавиши едновременно: Windows Key + CTRL + SHIFT + B. Това ще обнови комуникацията с графичния драйвер.</span><span class="sxs-lookup"><span data-stu-id="7ee51-105">Press the following keys at the same time: Windows Key  + Ctrl + Shift + B. This will refresh communication with your graphics driver.</span></span> <span data-ttu-id="7ee51-106">Мониторите ви ще се върнат след няколко секунди.</span><span class="sxs-lookup"><span data-stu-id="7ee51-106">Your monitors will blink momentarily and come back after a few seconds.</span></span>

<span data-ttu-id="7ee51-107">**Отстраняване на неизправности в хардуера на монитора:**</span><span class="sxs-lookup"><span data-stu-id="7ee51-107">**Troubleshoot monitor hardware:**</span></span>

1. <span data-ttu-id="7ee51-108">Изключете кабела, свързващ компютъра с монитора, и го включете обратно.</span><span class="sxs-lookup"><span data-stu-id="7ee51-108">Unplug the cable connecting your PC to your monitor, and plug it back in.</span></span>
2. <span data-ttu-id="7ee51-109">Изключете всички несъществени устройства от вашия компютър (например адаптери или докове).</span><span class="sxs-lookup"><span data-stu-id="7ee51-109">Disconnect any non-essential devices from your PC (such as adapters or docks).</span></span>

<span data-ttu-id="7ee51-110">**Ако наскоро сте инсталирали актуализация на вашия компютър, можете да възстановите драйвера на дисплея:**</span><span class="sxs-lookup"><span data-stu-id="7ee51-110">**If you recently installed an update on your PC, you can roll back your display driver:**</span></span>

1. <span data-ttu-id="7ee51-111">Изберете **Старт**, въведете **Диспечер на устройствата**и изберете **Диспечер на устройствата** от резултатите.</span><span class="sxs-lookup"><span data-stu-id="7ee51-111">Select **Start**, type **device manager**, and select **Device Manager** from the results.</span></span>
2. <span data-ttu-id="7ee51-112">Разгънете секцията **дисплейни адаптери** , щракнете с десния бутон върху видеокартата, и изберете **свойства**.</span><span class="sxs-lookup"><span data-stu-id="7ee51-112">Expand the **Display adapters** section, right-click your display adapter, ands select **Properties**.</span></span>
3. <span data-ttu-id="7ee51-113">Навигирайте до раздела на **драйвера** и изберете **връщане на драйвера**.</span><span class="sxs-lookup"><span data-stu-id="7ee51-113">Navigate to the **Driver** tab and select **Roll Back Driver**.</span></span> <br>
<span data-ttu-id="7ee51-114">Забележка: Ако това не е налично или е сиво, изберете " **не** " от опциите по-долу, за да преминете към следващата стъпка.</span><span class="sxs-lookup"><span data-stu-id="7ee51-114">Note: If this isn't available or is grayed out, select **No** from the options below to move to the next step.</span></span>
4. <span data-ttu-id="7ee51-115">Може да се наложи да рестартирате КОМПЮТЪРА, преди тези промени да влязат в сила.</span><span class="sxs-lookup"><span data-stu-id="7ee51-115">You may need to restart your PC before these changes take effect.</span></span>

<span data-ttu-id="7ee51-116">**Деинсталирайте и преинсталирайте драйвера на дисплея:**</span><span class="sxs-lookup"><span data-stu-id="7ee51-116">**Uninstall and reinstall your display driver:**</span></span>

1. <span data-ttu-id="7ee51-117">Изберете **Старт**, въведете **Диспечер на устройствата**и изберете **Диспечер на устройствата** от резултатите.</span><span class="sxs-lookup"><span data-stu-id="7ee51-117">Select **Start**, type **device manager**, and select **Device Manager** from the results.</span></span>
2. <span data-ttu-id="7ee51-118">Разгънете секцията **дисплейни адаптери** , щракнете с десния бутон върху видеокартата, и изберете **Деинсталиране на устройство**.</span><span class="sxs-lookup"><span data-stu-id="7ee51-118">Expand the **Display adapters** section, right-click your display adapter, ands select **Uninstall device**.</span></span> 
3. <span data-ttu-id="7ee51-119">Поставете отметка в квадратчето до **Изтриване на софтуерния драйвер за това устройство** и изберете **Деинсталиране**.</span><span class="sxs-lookup"><span data-stu-id="7ee51-119">Select the box next to **Delete the driver software for this device** and select **Uninstall**.</span></span><br>
<span data-ttu-id="7ee51-120">Забележка: може да бъдете помолени да рестартирате компютъра на този етап.</span><span class="sxs-lookup"><span data-stu-id="7ee51-120">Note: You may be asked to restart your computer at this stage.</span></span> <span data-ttu-id="7ee51-121">Уверете се, че сте написали останалите инструкции, преди да рестартирате.</span><span class="sxs-lookup"><span data-stu-id="7ee51-121">Make sure to write down the remaining instructions before you restart.</span></span>
4. <span data-ttu-id="7ee51-122">Отворете отново диспечера на устройствата.</span><span class="sxs-lookup"><span data-stu-id="7ee51-122">Open Device Manager again.</span></span>
5. <span data-ttu-id="7ee51-123">Разгънете секцията **дисплейни адаптери** , щракнете с десния бутон върху видеокартата и изберете **актуализиране на драйвера**.</span><span class="sxs-lookup"><span data-stu-id="7ee51-123">Expand the **Display adapters** section, right-click on your display adapter, and select **Update Driver**.</span></span>
6. <span data-ttu-id="7ee51-124">Изберете **автоматично търсене за актуализиране на софтуерния драйвер** и следвайте инструкциите за инсталиране.</span><span class="sxs-lookup"><span data-stu-id="7ee51-124">Select **Search automatically for update driver software** and follow the installation instructions.</span></span>