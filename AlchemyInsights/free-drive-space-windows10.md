---
title: Освобождаване на място на диск в Windows 10
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
- "9005403"
ms.openlocfilehash: 3838f3db3bc5f54bcb1a2558484056f3194b76e1
ms.sourcegitcommit: c08bed4071baa3bb5879496df3ed44fb828c8367
ms.translationtype: MT
ms.contentlocale: bg-BG
ms.lasthandoff: 03/19/2021
ms.locfileid: "51034981"
---
# <a name="free-up-drive-space-in-windows-10"></a><span data-ttu-id="aedde-102">Освобождаване на място на диск в Windows 10</span><span class="sxs-lookup"><span data-stu-id="aedde-102">Free up drive space in Windows 10</span></span>

<span data-ttu-id="aedde-103">Ето две опции, за да освободите място на диска в Windows:</span><span class="sxs-lookup"><span data-stu-id="aedde-103">Here are two options to free up drive space in Windows:</span></span>

- <span data-ttu-id="aedde-104">Освободете място за диск в Windows 10.</span><span class="sxs-lookup"><span data-stu-id="aedde-104">Free up drive space in Windows 10.</span></span>
- <span data-ttu-id="aedde-105">Освободете място за актуализации за Windows 10 с външно устройство за съхранение.</span><span class="sxs-lookup"><span data-stu-id="aedde-105">Free up space for Windows 10 updates with external storage device.</span></span>

<span data-ttu-id="aedde-106">Ако все още имате недостатъчно дисково пространство, след като сте използвали функцията за почистване на диска, е възможно вашата папка Temp бързо да се попълва с файловете за приложения (. Appx), използвани от Microsoft Store.</span><span class="sxs-lookup"><span data-stu-id="aedde-106">If you still have low disk space after using Disk Cleanup, it’s possible that your Temp folder is quickly filling up with application (.appx) files used by Microsoft Store.</span></span> <span data-ttu-id="aedde-107">За да коригирате този проблем, Нулирайте магазина, изчистете кеша на магазина и след това изпълнете програмата за отстраняване на неизправности на Windows Update.</span><span class="sxs-lookup"><span data-stu-id="aedde-107">To fix this problem, reset the Store, clear the Store cache, and then run the Windows Update troubleshooter.</span></span> <span data-ttu-id="aedde-108">Уверете се, че Microsoft Store е затворен, преди да продължите с тези стъпки.</span><span class="sxs-lookup"><span data-stu-id="aedde-108">Make sure Microsoft Store is closed before you proceed with these steps.</span></span>

<span data-ttu-id="aedde-109">**Стъпка 1: нулиране на магазина на Microsoft**</span><span class="sxs-lookup"><span data-stu-id="aedde-109">**Step 1: Reset Microsoft Store**</span></span>

<span data-ttu-id="aedde-110">**Забележка** Това окончателно изтрива данните на приложението на устройството, включително вашите предпочитания и подробни данни за влизане.</span><span class="sxs-lookup"><span data-stu-id="aedde-110">**Note** This permanently deletes the app data on the device, including your preferences and sign-in details.</span></span>

1. <span data-ttu-id="aedde-111">Изберете **Start**  >  **Settings**  >  **Apps Apps**  >  **& функции**.</span><span class="sxs-lookup"><span data-stu-id="aedde-111">Select **Start** > **Settings** > **Apps** > **Apps & features**.</span></span>

1. <span data-ttu-id="aedde-112">В списъка с приложения Намерете и изберете Microsoft Store.</span><span class="sxs-lookup"><span data-stu-id="aedde-112">In the list of apps, locate and select Microsoft Store.</span></span>

1. <span data-ttu-id="aedde-113">Изберете **Разширени опции**.</span><span class="sxs-lookup"><span data-stu-id="aedde-113">Select **Advanced options**.</span></span>

1. <span data-ttu-id="aedde-114">Превъртете надолу и изберете **нулиране** и след това **потвърдете нулиране**.</span><span class="sxs-lookup"><span data-stu-id="aedde-114">Scroll down and select **Reset**, and then **Confirm Reset**.</span></span>

<span data-ttu-id="aedde-115">**Стъпка 2: Изчистете кеша на Microsoft Store**</span><span class="sxs-lookup"><span data-stu-id="aedde-115">**Step 2: Clear the Microsoft Store cache**</span></span>

1. <span data-ttu-id="aedde-116">Натиснете клавиша с емблемата на Windows + R, за да отворите диалоговия прозорец изпълнение.</span><span class="sxs-lookup"><span data-stu-id="aedde-116">Press the Windows Logo Key + R to open the Run dialog box.</span></span>

1. <span data-ttu-id="aedde-117">Въведете wsreset.exe и изберете **OK**.</span><span class="sxs-lookup"><span data-stu-id="aedde-117">Type wsreset.exe and select **OK**.</span></span>

1. <span data-ttu-id="aedde-118">Отваря се прозорец на празна командна подкана.</span><span class="sxs-lookup"><span data-stu-id="aedde-118">A blank Command Prompt window opens.</span></span> <span data-ttu-id="aedde-119">След около 10 секунди прозорецът се затваря и Магазинът се отваря автоматично.</span><span class="sxs-lookup"><span data-stu-id="aedde-119">After about 10 seconds, the window closes and the Store opens automatically.</span></span>

<span data-ttu-id="aedde-120">**Стъпка 3: нулиране на Windows Update**</span><span class="sxs-lookup"><span data-stu-id="aedde-120">**Step 3: Reset Windows Update**</span></span>

1. <span data-ttu-id="aedde-121">Изберете **стартиране**  >  на **настройките** за  >  **актуализиране &**  >  **отстраняване на неизправности при** защитата.</span><span class="sxs-lookup"><span data-stu-id="aedde-121">Select **Start** > **Settings** > **Update & Security** > **Troubleshoot**.</span></span>

1. <span data-ttu-id="aedde-122">Превъртете надолу и изберете **Windows Update** от списъка и изберете **изпълнение на програмата за отстраняване на неизправности**.</span><span class="sxs-lookup"><span data-stu-id="aedde-122">Scroll down and select **Windows Update** from the list, and select **Run the troubleshooter**.</span></span>

1. <span data-ttu-id="aedde-123">Рестартирайте компютъра си и проверете дали все още имате проблем.</span><span class="sxs-lookup"><span data-stu-id="aedde-123">Reboot your computer and check whether you're still experiencing the issue.</span></span>

