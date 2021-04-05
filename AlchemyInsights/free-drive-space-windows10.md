---
title: Освобождаване на място на Windows 10
ms.author: pebaum
author: pebaum
manager: dansimp
ms.date: 03/16/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9771"
- "9774"
- "9005390"
- "9005403"
ms.openlocfilehash: 2313636307bfddce2810c2d4c4ce9e3b407a7bdf
ms.sourcegitcommit: 7b2e5078dd65f11af6650e692a7ea48e91f544e0
ms.translationtype: HT
ms.contentlocale: bg-BG
ms.lasthandoff: 04/02/2021
ms.locfileid: "51505345"
---
# <a name="free-up-drive-space-in-windows-10"></a><span data-ttu-id="6232a-102">Освобождаване на място на Windows 10</span><span class="sxs-lookup"><span data-stu-id="6232a-102">Free up drive space in Windows 10</span></span>

<span data-ttu-id="6232a-103">Ето две опции, за да освободите дисково пространство в Windows:</span><span class="sxs-lookup"><span data-stu-id="6232a-103">Here are two options to free up drive space in Windows:</span></span>

- <span data-ttu-id="6232a-104">Освобождаване на място на Windows 10.</span><span class="sxs-lookup"><span data-stu-id="6232a-104">Free up drive space in Windows 10.</span></span>
- <span data-ttu-id="6232a-105">Освобождаване на място за актуализации на Windows 10 чрез външно устройство за съхранение.</span><span class="sxs-lookup"><span data-stu-id="6232a-105">Free up space for Windows 10 updates with external storage device.</span></span>

<span data-ttu-id="6232a-106">Ако все още имате малко дисково пространство след почистването на диска, е възможно папката „Temp“ бързо да се запълни с файловете на приложения (.appx), използвани от Microsoft Store.</span><span class="sxs-lookup"><span data-stu-id="6232a-106">If you still have low disk space after using Disk Cleanup, it’s possible that your Temp folder is quickly filling up with application (.appx) files used by Microsoft Store.</span></span> <span data-ttu-id="6232a-107">За да коригирате този проблем, нулирайте магазина, изчистете кеша от магазина и след това изпълнете програмата за отстраняване на неизправности на Windows Update.</span><span class="sxs-lookup"><span data-stu-id="6232a-107">To fix this problem, reset the Store, clear the Store cache, and then run the Windows Update troubleshooter.</span></span> <span data-ttu-id="6232a-108">Уверете се, че Microsoft Store е затворен, преди да продължите с тези стъпки.</span><span class="sxs-lookup"><span data-stu-id="6232a-108">Make sure Microsoft Store is closed before you proceed with these steps.</span></span>

<span data-ttu-id="6232a-109">**Стъпка 1: Нулиране на Microsoft Store**</span><span class="sxs-lookup"><span data-stu-id="6232a-109">**Step 1: Reset Microsoft Store**</span></span>

<span data-ttu-id="6232a-110">**Забележка** Това изтрива окончателно данните на приложението на устройството, включително вашите предпочитания и подробни данни за влизане.</span><span class="sxs-lookup"><span data-stu-id="6232a-110">**Note** This permanently deletes the app data on the device, including your preferences and sign-in details.</span></span>

1. <span data-ttu-id="6232a-111">Изберете **Стартиране** > **Настройки** > **Приложения** > **Приложения и функции**.</span><span class="sxs-lookup"><span data-stu-id="6232a-111">Select **Start** > **Settings** > **Apps** > **Apps & features**.</span></span>

1. <span data-ttu-id="6232a-112">В списъка с приложения намерете и изберете Microsoft Store.</span><span class="sxs-lookup"><span data-stu-id="6232a-112">In the list of apps, locate and select Microsoft Store.</span></span>

1. <span data-ttu-id="6232a-113">Изберете **Разширени опции**.</span><span class="sxs-lookup"><span data-stu-id="6232a-113">Select **Advanced options**.</span></span>

1. <span data-ttu-id="6232a-114">Превъртете надолу и изберете **Нулиране** и след това **Потвърждаване на нулирането**.</span><span class="sxs-lookup"><span data-stu-id="6232a-114">Scroll down and select **Reset**, and then **Confirm Reset**.</span></span>

<span data-ttu-id="6232a-115">**Стъпка 2: Изчистване на кеша от Microsoft Store**</span><span class="sxs-lookup"><span data-stu-id="6232a-115">**Step 2: Clear the Microsoft Store cache**</span></span>

1. <span data-ttu-id="6232a-116">Натиснете клавиша с емблемата на Windows + R, за да отворите диалоговия прозорец „Изпълнение“.</span><span class="sxs-lookup"><span data-stu-id="6232a-116">Press the Windows Logo Key + R to open the Run dialog box.</span></span>

1. <span data-ttu-id="6232a-117">Въведете wsreset.exe и изберете **OK**.</span><span class="sxs-lookup"><span data-stu-id="6232a-117">Type wsreset.exe and select **OK**.</span></span>

1. <span data-ttu-id="6232a-118">Отваря се празен прозорец на командната среда.</span><span class="sxs-lookup"><span data-stu-id="6232a-118">A blank Command Prompt window opens.</span></span> <span data-ttu-id="6232a-119">След около 10 секунди прозорецът се затваря и магазинът се отваря автоматично.</span><span class="sxs-lookup"><span data-stu-id="6232a-119">After about 10 seconds, the window closes and the Store opens automatically.</span></span>

<span data-ttu-id="6232a-120">**Стъпка 3: Нулиране на Windows Update**</span><span class="sxs-lookup"><span data-stu-id="6232a-120">**Step 3: Reset Windows Update**</span></span>

1. <span data-ttu-id="6232a-121">Изберете **Стартиране** > **Настройки** > **Актуализация и сигурност** > **Отстраняване на неизправности**.</span><span class="sxs-lookup"><span data-stu-id="6232a-121">Select **Start** > **Settings** > **Update & Security** > **Troubleshoot**.</span></span>

1. <span data-ttu-id="6232a-122">Превъртете надолу и изберете **Windows Update** от списъка, и изберете **Изпълняване на програмата за отстраняване на неизправности**.</span><span class="sxs-lookup"><span data-stu-id="6232a-122">Scroll down and select **Windows Update** from the list, and select **Run the troubleshooter**.</span></span>

1. <span data-ttu-id="6232a-123">Рестартирайте компютъра си и проверете дали все още имате този проблем.</span><span class="sxs-lookup"><span data-stu-id="6232a-123">Reboot your computer and check whether you're still experiencing the issue.</span></span>

