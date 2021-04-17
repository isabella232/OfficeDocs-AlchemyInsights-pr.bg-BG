---
title: Настройки за стартиране в Windows 10
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
- "9001691"
- "3768"
ms.openlocfilehash: 6dfae58a398db088ba00d9c2ea9788bab929ccc1
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: bg-BG
ms.lasthandoff: 04/15/2021
ms.locfileid: "51828141"
---
# <a name="startup-settings-in-windows-10"></a><span data-ttu-id="72c2b-102">Настройки за стартиране в Windows 10</span><span class="sxs-lookup"><span data-stu-id="72c2b-102">Startup settings in Windows 10</span></span>

<span data-ttu-id="72c2b-103">**Промяна на това кои приложения да се изпълняват автоматично при стартиране**</span><span class="sxs-lookup"><span data-stu-id="72c2b-103">**Change which apps run automatically at startup**</span></span>

1. <span data-ttu-id="72c2b-104">Отидете на [Настройки > приложения > стартиране](ms-settings:startupapps?activationSource=GetHelp).</span><span class="sxs-lookup"><span data-stu-id="72c2b-104">Go to [Settings > Apps > Startup](ms-settings:startupapps?activationSource=GetHelp).</span></span>

2. <span data-ttu-id="72c2b-105">Уверете се, че всяко приложение, което искате да изпълните при стартиране, е **включено**.</span><span class="sxs-lookup"><span data-stu-id="72c2b-105">Make sure any app you want to run at startup is turned **On**.</span></span>

<span data-ttu-id="72c2b-106">**Добавяне на приложение за автоматично изпълнение при стартиране**</span><span class="sxs-lookup"><span data-stu-id="72c2b-106">**Add an app to run automatically at startup**</span></span>

1. <span data-ttu-id="72c2b-107">Щракнете върху или **докоснете Старт** и намерете приложението, което искате да изпълните при стартиране.</span><span class="sxs-lookup"><span data-stu-id="72c2b-107">Click or tap **Start** and find the app you want to run at startup.</span></span>

2. <span data-ttu-id="72c2b-108">Щракнете с десния бутон върху приложението, щракнете върху **Още** и след това щракнете върху **Отвори местоположението на файла**.</span><span class="sxs-lookup"><span data-stu-id="72c2b-108">Right-click the app, click **More**, and then click **Open file location**.</span></span> <span data-ttu-id="72c2b-109">Това отваря местоположението, където се записва прекият път до приложението.</span><span class="sxs-lookup"><span data-stu-id="72c2b-109">This opens the location where the shortcut to the app is saved.</span></span> <span data-ttu-id="72c2b-110">Ако няма опция за отваряне на местоположението на файла, това означава, че приложението не може да се изпълнява при стартиране.</span><span class="sxs-lookup"><span data-stu-id="72c2b-110">If there is no option for Open file location, it means the app can't run at startup.</span></span>

3. <span data-ttu-id="72c2b-111">Когато местоположението на файла е отворено, натиснете клавиша **с емблемата на Windows + R**, въведете **shell:startup**, след което щракнете върху **OK**.</span><span class="sxs-lookup"><span data-stu-id="72c2b-111">With the file location open, press the **Windows logo key  + R**, type **shell:startup**, then click **OK**.</span></span> <span data-ttu-id="72c2b-112">Това отваря папката "Стартиране".</span><span class="sxs-lookup"><span data-stu-id="72c2b-112">This opens the Startup folder.</span></span>

4. <span data-ttu-id="72c2b-113">Копирайте и поставете прекия път в приложението от местоположението на файла в папката "Стартиране".</span><span class="sxs-lookup"><span data-stu-id="72c2b-113">Copy and paste the shortcut to the app from the file location to the Startup folder.</span></span>

<span data-ttu-id="72c2b-114">**Разширени опции за стартиране (включително безопасен режим, настройки на UEFI и зареждане от друго устройство)**</span><span class="sxs-lookup"><span data-stu-id="72c2b-114">**Advanced startup options (including Safe Mode, UEFI settings, and booting from another device)**</span></span>

1. <span data-ttu-id="72c2b-115">Запишете работата си и затворете всички отворени документи, тъй като тези стъпки ще рестартират компютъра ви.</span><span class="sxs-lookup"><span data-stu-id="72c2b-115">Save your work and close any open documents, since these steps will restart your PC.</span></span>

2. <span data-ttu-id="72c2b-116">Отидете на [Настройки > актуализирай & на > възстановяване](ms-settings:recovery?activationSource=GetHelp).</span><span class="sxs-lookup"><span data-stu-id="72c2b-116">Go to [Settings > Update & Security > Recovery](ms-settings:recovery?activationSource=GetHelp).</span></span>

3. <span data-ttu-id="72c2b-117">Под **Разширено стартиране щракнете** върху Рестартиране **сега.**</span><span class="sxs-lookup"><span data-stu-id="72c2b-117">Under **Advanced startup**, click **Restart now**.</span></span> 

4. <span data-ttu-id="72c2b-118">След като компютърът се рестартира на екрана Избор на опция:</span><span class="sxs-lookup"><span data-stu-id="72c2b-118">After your PC restarts to the Choose an option screen:</span></span>

    - <span data-ttu-id="72c2b-119">За да стартирате от устройство, като например USB устройство, щракнете **върху Използване на устройство**.</span><span class="sxs-lookup"><span data-stu-id="72c2b-119">To boot from a device like a USB drive, click **Use a device**.</span></span>

    - <span data-ttu-id="72c2b-120">За да въведете настройките на UEFI (понякога наричани настройка на BIOS), щракнете върху Отстраняване на неизправности > Разширени опции > настройките на **фърмуера на UEFI**.</span><span class="sxs-lookup"><span data-stu-id="72c2b-120">To enter the UEFI settings (sometimes called BIOS setup), click **Troubleshoot > Advanced options > UEFI Firmware Settings**.</span></span> 

    - <span data-ttu-id="72c2b-121">За да въведете безопасен режим или да промените разширените настройки за стартиране, щракнете върху Отстраняване на > разширени опции > настройки при **стартиране,** след което щракнете върху **Рестартиране**.</span><span class="sxs-lookup"><span data-stu-id="72c2b-121">To enter Safe Mode or change advanced startup settings, click **Troubleshoot > Advanced options > Startup Settings**, then click **Restart**.</span></span> <span data-ttu-id="72c2b-122">Може да бъдете помолени да въведете своя [ключ за възстановяване на BitLocker](https://support.microsoft.com/help/4026181/windows-10-find-my-bitlocker-recovery-key).</span><span class="sxs-lookup"><span data-stu-id="72c2b-122">You may be asked to enter your [BitLocker recovery key](https://support.microsoft.com/help/4026181/windows-10-find-my-bitlocker-recovery-key).</span></span> <span data-ttu-id="72c2b-123">След като компютърът се рестартира отново, щракнете върху настройката за стартиране, която искате да използвате.</span><span class="sxs-lookup"><span data-stu-id="72c2b-123">After your PC restarts again, click the startup setting you want to use.</span></span>