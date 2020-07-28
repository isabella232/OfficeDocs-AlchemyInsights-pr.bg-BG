---
title: Намиране на загубени IOS устройства с Intune
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
- "1283"
- "6700008"
ms.openlocfilehash: faaea65c7edc345bb676d2fb266e20f85ba2cbe5
ms.sourcegitcommit: e34bb95fb93250f1dc7aec6a13578bb3bb355935
ms.translationtype: MT
ms.contentlocale: bg-BG
ms.lasthandoff: 07/28/2020
ms.locfileid: "45438907"
---
# <a name="locating-lost-ios-devices-with-intune"></a><span data-ttu-id="20d99-102">Намиране на загубени IOS устройства с Intune</span><span class="sxs-lookup"><span data-stu-id="20d99-102">Locating lost iOS devices with Intune</span></span>

<span data-ttu-id="20d99-103">Разрешаването на режима на загубено устройство на iOS позволява на администратора да има съобщение и контакт телефонен номер се показва на заключения екран.</span><span class="sxs-lookup"><span data-stu-id="20d99-103">Enabling lost mode on an iOS device allows an administrator to have a message and contact phone number displayed on the lock screen.</span></span>

<span data-ttu-id="20d99-104">След загубен режим е активиран администраторът може да използва действието на устройството за идентифициране на физическото местоположение на устройството.</span><span class="sxs-lookup"><span data-stu-id="20d99-104">After lost mode is enabled the admin can use the Locate device action to identify the physical location of the device.</span></span>

<span data-ttu-id="20d99-105">Намерете действие в Intune работи с iOS устройства да покаже местоположението на конкретно устройство на карта.</span><span class="sxs-lookup"><span data-stu-id="20d99-105">The Locate device action in Intune works with iOS devices to show the location of a specific device on a map.</span></span>

<span data-ttu-id="20d99-106">Използването на това действие изисква iOS устройството да бъде в:</span><span class="sxs-lookup"><span data-stu-id="20d99-106">Using this action requires the iOS device to be in:</span></span>

- <span data-ttu-id="20d99-107">Режим на наблюдение</span><span class="sxs-lookup"><span data-stu-id="20d99-107">Supervised mode</span></span>
- <span data-ttu-id="20d99-108">Изгубен режим</span><span class="sxs-lookup"><span data-stu-id="20d99-108">Lost mode</span></span>

<span data-ttu-id="20d99-109">За повече информация вижте [Разрешаване на загубения режим на iOS / iPadOS устройства с Intune](https://docs.microsoft.com/intune/device-lost-mode) и [Намерете изгубени или откраднати iOS /iPadOS устройства с Intune](https://docs.microsoft.com/intune/device-locate).</span><span class="sxs-lookup"><span data-stu-id="20d99-109">For more info, see [Enable lost mode on iOS/iPadOS devices with Intune](https://docs.microsoft.com/intune/device-lost-mode) and [Locate lost or stolen iOS/iPadOS devices with Intune](https://docs.microsoft.com/intune/device-locate).</span></span>

<span data-ttu-id="20d99-110">**ЧЗВ**</span><span class="sxs-lookup"><span data-stu-id="20d99-110">**FAQ**</span></span>

<span data-ttu-id="20d99-111">Q: Аз издавам дистанционно действие за премахване на фирмени данни от устройство, а сега е блокирано в чакащо състояние.</span><span class="sxs-lookup"><span data-stu-id="20d99-111">Q: I issued a remote action to remove company data from a device, and now it’s stuck in a pending state.</span></span>

<span data-ttu-id="20d99-112">О: За да завършите отдалеченото действие, целевото устройство трябва да е онлайн и здравословно.</span><span class="sxs-lookup"><span data-stu-id="20d99-112">A: For a remote action to successfully complete, the targeted device must be online and healthy.</span></span> <span data-ttu-id="20d99-113">В следните ситуации отдалечено действие остава в чакащо състояние в продължение на 30 дни или докато устройството потвърди командата:</span><span class="sxs-lookup"><span data-stu-id="20d99-113">In the following situations, the remote action stays in a pending state for 30 days, or until the device acknowledges the command:</span></span>

- <span data-ttu-id="20d99-114">Когато устройството няма връзка</span><span class="sxs-lookup"><span data-stu-id="20d99-114">When the device does not have connectivity</span></span>
- <span data-ttu-id="20d99-115">Когато устройството загуби своето състояние на управление с Intune</span><span class="sxs-lookup"><span data-stu-id="20d99-115">When the device loses its management status with Intune</span></span>

<span data-ttu-id="20d99-116">Ако смятате, че дадено устройство вече не се регистрира и че няма да може да премахне фирмени данни, изберете Изтриване.</span><span class="sxs-lookup"><span data-stu-id="20d99-116">If you think a device is no longer checking in, and that it won’t be able to remove company data, select Delete.</span></span> <span data-ttu-id="20d99-117">Изтриването премахва записа на устройството, така че той вече да не се появява в списъка с устройства Intune.</span><span class="sxs-lookup"><span data-stu-id="20d99-117">Deleting removes the device record so that it no longer appears in the Intune list of devices.</span></span> <span data-ttu-id="20d99-118">Ако устройството стане отново активен, неговият потребител ще трябва да го запишат отново.</span><span class="sxs-lookup"><span data-stu-id="20d99-118">If the device becomes active again, its user will have to re-enroll it.</span></span>

<span data-ttu-id="20d99-119">Въпрос: Защо някои дистанционни действия не са достъпни за мен да използвам?</span><span class="sxs-lookup"><span data-stu-id="20d99-119">Q: Why are certain remote actions not available for me to use?</span></span>

<span data-ttu-id="20d99-120">О: Не всички платформи поддържат всички действия за отдалечени устройства.</span><span class="sxs-lookup"><span data-stu-id="20d99-120">A: Not all platforms support all remote device actions.</span></span> <span data-ttu-id="20d99-121">Следните отдалечени действия са специфични за платформата, така че те са достъпни само за посочените платформи.</span><span class="sxs-lookup"><span data-stu-id="20d99-121">The following remote actions are platform-specific, so they are available only for the platforms noted.</span></span>

- <span data-ttu-id="20d99-122">Байпас заключване за активиране (само за iOS)</span><span class="sxs-lookup"><span data-stu-id="20d99-122">Bypass Activation Lock (iOS only)</span></span>
- <span data-ttu-id="20d99-123">"Старт на старт" (само за Windows)</span><span class="sxs-lookup"><span data-stu-id="20d99-123">Fresh Start (Windows only)</span></span>
- <span data-ttu-id="20d99-124">Загубен режим (само за iOS)</span><span class="sxs-lookup"><span data-stu-id="20d99-124">Lost mode (iOS only)</span></span>
- <span data-ttu-id="20d99-125">Намиране на устройство (само за iOS)</span><span class="sxs-lookup"><span data-stu-id="20d99-125">Locate device (iOS only)</span></span>
- <span data-ttu-id="20d99-126">Рестартиране (само за Windows)</span><span class="sxs-lookup"><span data-stu-id="20d99-126">Restart (Windows only)</span></span>

<span data-ttu-id="20d99-127">За повече подробности за всяко действие вижте [Налични действия на устройството](https://docs.microsoft.com/intune/device-management#available-device-actions).</span><span class="sxs-lookup"><span data-stu-id="20d99-127">For more details about each action, see [Available device actions](https://docs.microsoft.com/intune/device-management#available-device-actions).</span></span>