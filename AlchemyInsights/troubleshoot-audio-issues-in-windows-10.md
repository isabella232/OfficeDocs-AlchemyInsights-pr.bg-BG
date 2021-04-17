---
title: Отстраняване на проблеми с аудиото в Windows 10
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
- "3476"
- "9001463"
ms.openlocfilehash: 1bafc97b2ab1394087d2451d73168a29267d64ab
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: bg-BG
ms.lasthandoff: 04/15/2021
ms.locfileid: "51833280"
---
# <a name="troubleshooting-audio-issues-in-windows-10"></a><span data-ttu-id="b7362-102">Отстраняване на проблеми с аудиото в Windows 10</span><span class="sxs-lookup"><span data-stu-id="b7362-102">Troubleshooting audio issues in Windows 10</span></span>

<span data-ttu-id="b7362-103">**Изпълнение на програмата за отстраняване на неизправности с аудиото**</span><span class="sxs-lookup"><span data-stu-id="b7362-103">**Run the audio troubleshooter**</span></span>

1.  <span data-ttu-id="b7362-104">Отворете настройките [за отстраняване на неизправности](ms-settings:troubleshoot).</span><span class="sxs-lookup"><span data-stu-id="b7362-104">Open the [Troubleshoot settings](ms-settings:troubleshoot).</span></span>

2.  <span data-ttu-id="b7362-105">Изберете **Изпълнение на аудио Изпълнение** на програмата за отстраняване на  >  **неизправности**.</span><span class="sxs-lookup"><span data-stu-id="b7362-105">Select **Playing Audio** > **Run the troubleshooter**.</span></span>

<span data-ttu-id="b7362-106">**Задаване на устройството по подразбиране**</span><span class="sxs-lookup"><span data-stu-id="b7362-106">**Set the default device**</span></span>

<span data-ttu-id="b7362-107">Ако се свързвате към аудиоустройство чрез USB или HDMI, може да се наложи да зададете това устройство по подразбиране:</span><span class="sxs-lookup"><span data-stu-id="b7362-107">If you're connecting to an audio device using USB or HDMI, you might need to set that device as the default:</span></span>

1. <span data-ttu-id="b7362-108">Отворете **Стартиране**  >  **на звука** и след това **изберете** Звук или Промяна **на звуците на** системата от списъка с резултати.</span><span class="sxs-lookup"><span data-stu-id="b7362-108">Open **Start** > **Sound**, and then select **Sound** or **Change system sounds** from the list of results.</span></span>

2.  <span data-ttu-id="b7362-109">В **раздела Възпроизвеждане** изберете устройство, изберете Задайте **по подразбиране** и след това **изберете OK**.</span><span class="sxs-lookup"><span data-stu-id="b7362-109">On the **Playback** tab, select a device, select **Set Default**, and then select **OK**.</span></span>

<span data-ttu-id="b7362-110">**Проверка на кабели, сила на звука, високоговорители и слушалки**</span><span class="sxs-lookup"><span data-stu-id="b7362-110">**Check cables, volume, speakers, and headphones**</span></span>

1. <span data-ttu-id="b7362-111">Проверете връзките на високоговорителя и слушалките за хлабави кабели и се уверете, че са свързани към правилния жак.</span><span class="sxs-lookup"><span data-stu-id="b7362-111">Check your speaker and headphone connections for loose cables, and make sure they're connected to the correct jack.</span></span>

2. <span data-ttu-id="b7362-112">Проверете нивата на силата и силата на звука и опитайте да включите всички контроли за силата на звука.</span><span class="sxs-lookup"><span data-stu-id="b7362-112">Check your power and volume levels and try turning all the volume controls up.</span></span>

3. <span data-ttu-id="b7362-113">Някои високоговорители и приложения имат собствени контроли за силата на звука; може да се наложи да проверите всички, за да се уверите, че са на правилното ниво.</span><span class="sxs-lookup"><span data-stu-id="b7362-113">Some speakers and apps have their own volume controls; you might have to check them all to make sure they're at the right levels.</span></span>

4. <span data-ttu-id="b7362-114">Опитайте да се свържете с друг USB порт.</span><span class="sxs-lookup"><span data-stu-id="b7362-114">Try connecting using a different USB port.</span></span>

<span data-ttu-id="b7362-115">**Забележка:** Не забравяйте, че високоговорителите може да не работят, когато слушалките са включени.</span><span class="sxs-lookup"><span data-stu-id="b7362-115">**Note**: Remember that your speakers may not work when headphones are plugged in.</span></span>

<span data-ttu-id="b7362-116">**Проверка на диспечера на устройствата**</span><span class="sxs-lookup"><span data-stu-id="b7362-116">**Check Device Manager**</span></span>

<span data-ttu-id="b7362-117">За да сте сигурни, че драйверите са актуални:</span><span class="sxs-lookup"><span data-stu-id="b7362-117">To make sure the drivers are up to date:</span></span>

1. <span data-ttu-id="b7362-118">Изберете **Старт**, въведете **Диспечер на устройствата** и след това изберете Диспечер **на** устройствата от списъка с резултати.</span><span class="sxs-lookup"><span data-stu-id="b7362-118">Select **Start**, type **Device Manager**, and then select **Device Manager** from the list of results.</span></span>

2. <span data-ttu-id="b7362-119">Под **Контролери за звук, видео и игри** изберете звуковата карта, отворете я, изберете раздела **Драйвер** и изберете Актуализиране на **драйвера**.</span><span class="sxs-lookup"><span data-stu-id="b7362-119">Under **Sound, video, and game controllers**, select your sound card, open it, select the **Driver** tab, and select **Update Driver**.</span></span>

<span data-ttu-id="b7362-120">**Забележка:** Ако Windows не намери нов драйвер, потърсете такъв в уеб сайта на производителя на устройството и следвайте инструкциите му.</span><span class="sxs-lookup"><span data-stu-id="b7362-120">**Note**: If Windows doesn't find a new driver, look for one on the device manufacturer's website and follow their instructions.</span></span>

<span data-ttu-id="b7362-121">**Преинсталиране на драйвера**</span><span class="sxs-lookup"><span data-stu-id="b7362-121">**Reinstall the driver**</span></span>

<span data-ttu-id="b7362-122">Ако не можете да актуализирате чрез диспечера на устройствата или да намерите нов драйвер в уеб сайта на производителя, изпробвайте тези стъпки:</span><span class="sxs-lookup"><span data-stu-id="b7362-122">If you can't update via Device Manager or find a new driver on the manufacturer's website, try these steps:</span></span>

1. <span data-ttu-id="b7362-123">В Диспечер на устройствата щракнете с десния бутон върху (или натиснете и задръжте) аудио драйвера и изберете **Деинсталиране**.</span><span class="sxs-lookup"><span data-stu-id="b7362-123">In Device Manager, right-click (or press and hold) the audio driver, and select **Uninstall**.</span></span> <span data-ttu-id="b7362-124">Рестартирайте устройството си и Windows ще се опита да преинсталира драйвера.</span><span class="sxs-lookup"><span data-stu-id="b7362-124">Restart your device and Windows will attempt to reinstall the driver.</span></span>

2. <span data-ttu-id="b7362-125">Ако преинсталирането на драйвера не работи, опитайте да използвате общ аудио драйвер, който се предоставя с Windows.</span><span class="sxs-lookup"><span data-stu-id="b7362-125">If reinstalling the driver doesn't work, try using the generic audio driver that comes with Windows.</span></span> <span data-ttu-id="b7362-126">В Диспечер на устройствата щракнете с десния бутон (или натиснете и задръжте) аудио драйвера > **Актуализирай** софтуера на драйвера Преглед на моя компютър за софтуерен драйвер Позволете ми да избера от списък с драйвери на устройства на моя компютър , изберете Аудиоустройство с висока разделителна способност  >    >  , изберете **Напред** и следвайте инструкциите, за да го инсталирате. </span><span class="sxs-lookup"><span data-stu-id="b7362-126">In Device Manager, right-click (or press and hold) your audio driver > **Update driver software** > **Browse my computer for driver software** > **Let me pick from a list of device drivers on my computer**, select **High Definition Audio Device**, select **Next**, and follow the instructions to install it.</span></span>
