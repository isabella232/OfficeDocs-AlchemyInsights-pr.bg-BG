---
title: Намиране на изгубени устройства с iOS чрез "Настройки"
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
- "1283"
- "6700008"
ms.openlocfilehash: 70f12328813a312631c67cd72cc75559ed2eca1b
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: bg-BG
ms.lasthandoff: 09/14/2020
ms.locfileid: "47675144"
---
# <a name="locating-lost-ios-devices-with-intune"></a><span data-ttu-id="f61f9-102">Намиране на изгубени устройства с iOS чрез "Настройки"</span><span class="sxs-lookup"><span data-stu-id="f61f9-102">Locating lost iOS devices with Intune</span></span>

<span data-ttu-id="f61f9-103">Разрешаването на изгубения режим на устройство с iOS позволява на администратора да получи съобщение и номер за контакт, показан на екрана при заключване.</span><span class="sxs-lookup"><span data-stu-id="f61f9-103">Enabling lost mode on an iOS device allows an administrator to have a message and contact phone number displayed on the lock screen.</span></span>

<span data-ttu-id="f61f9-104">След като опцията Lost е разрешена, администраторът може да използва действието за намиране на устройство, за да идентифицира физическото местоположение на устройството.</span><span class="sxs-lookup"><span data-stu-id="f61f9-104">After lost mode is enabled the admin can use the Locate device action to identify the physical location of the device.</span></span>

<span data-ttu-id="f61f9-105">Действието за намиране на устройството в "търси" работи с устройства с iOS, за да покаже местоположението на конкретно устройство на карта.</span><span class="sxs-lookup"><span data-stu-id="f61f9-105">The Locate device action in Intune works with iOS devices to show the location of a specific device on a map.</span></span>

<span data-ttu-id="f61f9-106">Използването на това действие изисква устройството с iOS да е в:</span><span class="sxs-lookup"><span data-stu-id="f61f9-106">Using this action requires the iOS device to be in:</span></span>

- <span data-ttu-id="f61f9-107">Наблюдаван режим</span><span class="sxs-lookup"><span data-stu-id="f61f9-107">Supervised mode</span></span>
- <span data-ttu-id="f61f9-108">Изгубен режим</span><span class="sxs-lookup"><span data-stu-id="f61f9-108">Lost mode</span></span>

<span data-ttu-id="f61f9-109">За повече информация вижте [Разрешаване на загубване на режим на устройства с IOS/iPadOS с настройки](https://docs.microsoft.com/intune/device-lost-mode) и [намиране на изгубени или откраднати устройства с IOS/iPadOS с пренастройване](https://docs.microsoft.com/intune/device-locate).</span><span class="sxs-lookup"><span data-stu-id="f61f9-109">For more info, see [Enable lost mode on iOS/iPadOS devices with Intune](https://docs.microsoft.com/intune/device-lost-mode) and [Locate lost or stolen iOS/iPadOS devices with Intune](https://docs.microsoft.com/intune/device-locate).</span></span>

<span data-ttu-id="f61f9-110">**ЧЗВ**</span><span class="sxs-lookup"><span data-stu-id="f61f9-110">**FAQ**</span></span>

<span data-ttu-id="f61f9-111">В: Издадох отдалечено действие, за да премахнете фирмените данни от устройство и сега то е блокирано в Чакащо състояние.</span><span class="sxs-lookup"><span data-stu-id="f61f9-111">Q: I issued a remote action to remove company data from a device, and now it’s stuck in a pending state.</span></span>

<span data-ttu-id="f61f9-112">А: за да завърши успешно отдалечено действие, целевото устройство трябва да бъде онлайн и здравословно.</span><span class="sxs-lookup"><span data-stu-id="f61f9-112">A: For a remote action to successfully complete, the targeted device must be online and healthy.</span></span> <span data-ttu-id="f61f9-113">В следните ситуации отдалеченото действие остава в Чакащ щат за 30 дни или докато устройството признае командата:</span><span class="sxs-lookup"><span data-stu-id="f61f9-113">In the following situations, the remote action stays in a pending state for 30 days, or until the device acknowledges the command:</span></span>

- <span data-ttu-id="f61f9-114">Когато устройството не разполага с връзка</span><span class="sxs-lookup"><span data-stu-id="f61f9-114">When the device does not have connectivity</span></span>
- <span data-ttu-id="f61f9-115">Когато устройството изгуби състоянието си на управление с "Настройки"</span><span class="sxs-lookup"><span data-stu-id="f61f9-115">When the device loses its management status with Intune</span></span>

<span data-ttu-id="f61f9-116">Ако смятате, че устройството вече не се вкарва и че няма да може да премахне фирмените данни, изберете Изтрий.</span><span class="sxs-lookup"><span data-stu-id="f61f9-116">If you think a device is no longer checking in, and that it won’t be able to remove company data, select Delete.</span></span> <span data-ttu-id="f61f9-117">Изтриването премахва записа на устройството, така че да не се показва повече в списъка на ненастроините устройства.</span><span class="sxs-lookup"><span data-stu-id="f61f9-117">Deleting removes the device record so that it no longer appears in the Intune list of devices.</span></span> <span data-ttu-id="f61f9-118">Ако устройството отново се активира, потребителят му ще трябва да го запише повторно.</span><span class="sxs-lookup"><span data-stu-id="f61f9-118">If the device becomes active again, its user will have to re-enroll it.</span></span>

<span data-ttu-id="f61f9-119">В: защо някои отдалечени действия не са налични за мен?</span><span class="sxs-lookup"><span data-stu-id="f61f9-119">Q: Why are certain remote actions not available for me to use?</span></span>

<span data-ttu-id="f61f9-120">А: не всички платформи поддържат всички действия за отдалечени устройства.</span><span class="sxs-lookup"><span data-stu-id="f61f9-120">A: Not all platforms support all remote device actions.</span></span> <span data-ttu-id="f61f9-121">Следните отдалечени действия са специфични за платформата, така че те са достъпни само за посочените платформи.</span><span class="sxs-lookup"><span data-stu-id="f61f9-121">The following remote actions are platform-specific, so they are available only for the platforms noted.</span></span>

- <span data-ttu-id="f61f9-122">Забрана за заключване при активиране (само за iOS)</span><span class="sxs-lookup"><span data-stu-id="f61f9-122">Bypass Activation Lock (iOS only)</span></span>
- <span data-ttu-id="f61f9-123">Ново начало (само за Windows)</span><span class="sxs-lookup"><span data-stu-id="f61f9-123">Fresh Start (Windows only)</span></span>
- <span data-ttu-id="f61f9-124">Загубване на режим (само за iOS)</span><span class="sxs-lookup"><span data-stu-id="f61f9-124">Lost mode (iOS only)</span></span>
- <span data-ttu-id="f61f9-125">Намиране на устройство (само за iOS)</span><span class="sxs-lookup"><span data-stu-id="f61f9-125">Locate device (iOS only)</span></span>
- <span data-ttu-id="f61f9-126">Рестартирайте (само за Windows)</span><span class="sxs-lookup"><span data-stu-id="f61f9-126">Restart (Windows only)</span></span>

<span data-ttu-id="f61f9-127">За повече информация относно всяко действие вижте [наличните действия за устройството](https://docs.microsoft.com/intune/device-management#available-device-actions).</span><span class="sxs-lookup"><span data-stu-id="f61f9-127">For more details about each action, see [Available device actions](https://docs.microsoft.com/intune/device-management#available-device-actions).</span></span>