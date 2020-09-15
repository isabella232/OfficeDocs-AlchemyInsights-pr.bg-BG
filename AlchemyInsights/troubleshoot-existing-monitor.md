---
title: Отстраняване на неизправности при съществуващ монитор
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3454"
- "9001450"
ms.openlocfilehash: 2dc9a24c1d0d808e26733738cedbc32d513926a0
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: bg-BG
ms.lasthandoff: 09/14/2020
ms.locfileid: "47690700"
---
# <a name="troubleshoot-an-existing-monitor"></a><span data-ttu-id="cc40e-102">Отстраняване на неизправности при съществуващ монитор</span><span class="sxs-lookup"><span data-stu-id="cc40e-102">Troubleshoot an existing monitor</span></span>

<span data-ttu-id="cc40e-103">Изпробвайте тези решения, за да отстраните монитора.</span><span class="sxs-lookup"><span data-stu-id="cc40e-103">Try these solutions to troubleshoot a monitor.</span></span> 

<span data-ttu-id="cc40e-104">**Обновяване на дисплея на монитора:**</span><span class="sxs-lookup"><span data-stu-id="cc40e-104">**Refresh your monitor's display:**</span></span>

<span data-ttu-id="cc40e-105">Натиснете едновременно следните клавиши: клавиш Windows + CTRL + SHIFT + B. Това ще обнови комуникацията с вашия графичен драйвер.</span><span class="sxs-lookup"><span data-stu-id="cc40e-105">Press the following keys at the same time: Windows Key  + Ctrl + Shift + B. This will refresh communication with your graphics driver.</span></span> <span data-ttu-id="cc40e-106">Мониторите ви ще мигат мигновено и се връщат след няколко секунди.</span><span class="sxs-lookup"><span data-stu-id="cc40e-106">Your monitors will blink momentarily and come back after a few seconds.</span></span>

<span data-ttu-id="cc40e-107">**Отстраняване на неизправности при хардуер за монитор:**</span><span class="sxs-lookup"><span data-stu-id="cc40e-107">**Troubleshoot monitor hardware:**</span></span>

1. <span data-ttu-id="cc40e-108">Изключете кабела, свързващ компютъра ви с монитора, и го включете отново.</span><span class="sxs-lookup"><span data-stu-id="cc40e-108">Unplug the cable connecting your PC to your monitor, and plug it back in.</span></span>
2. <span data-ttu-id="cc40e-109">Прекъснете връзката на всички неосновни устройства от вашия компютър (като например адаптери или докинг станция).</span><span class="sxs-lookup"><span data-stu-id="cc40e-109">Disconnect any non-essential devices from your PC (such as adapters or docks).</span></span>

<span data-ttu-id="cc40e-110">**Ако наскоро сте инсталирали актуализация на вашия компютър, можете да се върнете към драйвера на вашия дисплей:**</span><span class="sxs-lookup"><span data-stu-id="cc40e-110">**If you recently installed an update on your PC, you can roll back your display driver:**</span></span>

1. <span data-ttu-id="cc40e-111">Изберете **Старт**, въведете **Диспечер на устройствата**и изберете **Диспечер на устройствата** от резултатите.</span><span class="sxs-lookup"><span data-stu-id="cc40e-111">Select **Start**, type **device manager**, and select **Device Manager** from the results.</span></span>
2. <span data-ttu-id="cc40e-112">Разгънете **секцията "видеокарти"** , щракнете с десния бутон върху видеокартата за показване и изберете **свойства**.</span><span class="sxs-lookup"><span data-stu-id="cc40e-112">Expand the **Display adapters** section, right-click your display adapter, ands select **Properties**.</span></span>
3. <span data-ttu-id="cc40e-113">Придвижете се до раздела **драйвер** и изберете **връщане на драйвер**.</span><span class="sxs-lookup"><span data-stu-id="cc40e-113">Navigate to the **Driver** tab and select **Roll Back Driver**.</span></span> <br>
<span data-ttu-id="cc40e-114">Забележка: Ако това не е налично или е в сиво, изберете **не** от опциите по-долу, за да преминете към следващата стъпка.</span><span class="sxs-lookup"><span data-stu-id="cc40e-114">Note: If this isn't available or is grayed out, select **No** from the options below to move to the next step.</span></span>
4. <span data-ttu-id="cc40e-115">Може да се наложи да рестартирате КОМПЮТЪРА си, преди да влязат в сила тези промени.</span><span class="sxs-lookup"><span data-stu-id="cc40e-115">You may need to restart your PC before these changes take effect.</span></span>

<span data-ttu-id="cc40e-116">**Деинсталирайте и преинсталирайте драйвера на дисплея:**</span><span class="sxs-lookup"><span data-stu-id="cc40e-116">**Uninstall and reinstall your display driver:**</span></span>

1. <span data-ttu-id="cc40e-117">Изберете **Старт**, въведете **Диспечер на устройствата**и изберете **Диспечер на устройствата** от резултатите.</span><span class="sxs-lookup"><span data-stu-id="cc40e-117">Select **Start**, type **device manager**, and select **Device Manager** from the results.</span></span>
2. <span data-ttu-id="cc40e-118">Разгънете **секцията "видеокарти"** , щракнете с десния бутон върху видеокартата за показване и изберете **Деинсталиране на устройството**.</span><span class="sxs-lookup"><span data-stu-id="cc40e-118">Expand the **Display adapters** section, right-click your display adapter, ands select **Uninstall device**.</span></span> 
3. <span data-ttu-id="cc40e-119">Изберете квадратчето за отметка до **Изтриване на драйвера за това устройство** и изберете **Деинсталиране**.</span><span class="sxs-lookup"><span data-stu-id="cc40e-119">Select the box next to **Delete the driver software for this device** and select **Uninstall**.</span></span><br>
<span data-ttu-id="cc40e-120">Забележка: възможно е да бъдете подканени да рестартирате компютъра си на този етап.</span><span class="sxs-lookup"><span data-stu-id="cc40e-120">Note: You may be asked to restart your computer at this stage.</span></span> <span data-ttu-id="cc40e-121">Уверете се, че сте записали останалите инструкции, преди да рестартирате.</span><span class="sxs-lookup"><span data-stu-id="cc40e-121">Make sure to write down the remaining instructions before you restart.</span></span>
4. <span data-ttu-id="cc40e-122">Отворете диспечера на устройствата отново.</span><span class="sxs-lookup"><span data-stu-id="cc40e-122">Open Device Manager again.</span></span>
5. <span data-ttu-id="cc40e-123">Разгънете **секцията видеокарти** , щракнете с десния бутон върху видеокартата и изберете **актуализиране на драйвера**.</span><span class="sxs-lookup"><span data-stu-id="cc40e-123">Expand the **Display adapters** section, right-click on your display adapter, and select **Update Driver**.</span></span>
6. <span data-ttu-id="cc40e-124">Изберете **Търсене автоматично за актуализиране на софтуерни драйвери** и следвайте инструкциите за инсталиране.</span><span class="sxs-lookup"><span data-stu-id="cc40e-124">Select **Search automatically for update driver software** and follow the installation instructions.</span></span>