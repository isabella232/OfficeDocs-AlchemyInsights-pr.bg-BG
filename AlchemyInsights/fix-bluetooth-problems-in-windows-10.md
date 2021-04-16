---
title: Коригиране на проблеми с Bluetooth в Windows 10
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
- "9001475"
- "3506"
ms.openlocfilehash: f20bf4a642e019c7901e988a027e0220f0f1b07b
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: bg-BG
ms.lasthandoff: 04/15/2021
ms.locfileid: "51812921"
---
# <a name="fix-bluetooth-problems-in-windows-10"></a><span data-ttu-id="f0b1a-102">Коригиране на проблеми с Bluetooth в Windows 10</span><span class="sxs-lookup"><span data-stu-id="f0b1a-102">Fix Bluetooth problems in Windows 10</span></span>

<span data-ttu-id="f0b1a-103">Ако иконата за Bluetooth липсва или Bluetooth не може да бъде включена или изключена, може да искате да изпълните програмата за отстраняване на неизправности с Bluetooth.</span><span class="sxs-lookup"><span data-stu-id="f0b1a-103">If the Bluetooth icon is missing or Bluetooth can't be turned on or off, you may want to run the Bluetooth troubleshooter.</span></span> <span data-ttu-id="f0b1a-104">[Отворете настройките за отстраняване на неизправности](ms-settings:troubleshoot), щракнете върху **Bluetooth** под Търсене и отстраняване на **други проблеми** щракнете върху Изпълнение на програмата за отстраняване **на неизправности.**</span><span class="sxs-lookup"><span data-stu-id="f0b1a-104">[Open the Troubleshoot settings](ms-settings:troubleshoot), click **Bluetooth** under **Find and fix other problems**, click **Run the troubleshooter**.</span></span>

<span data-ttu-id="f0b1a-105">Ако не виждате иконата на Bluetooth, но Bluetooth се показва в диспечера на устройствата:</span><span class="sxs-lookup"><span data-stu-id="f0b1a-105">If you don't see the Bluetooth icon, but Bluetooth does appear in Device Manager:</span></span>

1. <span data-ttu-id="f0b1a-106">В Диспечер на устройствата щракнете върху **Bluetooth**.</span><span class="sxs-lookup"><span data-stu-id="f0b1a-106">In Device Manager, click **Bluetooth**.</span></span> <span data-ttu-id="f0b1a-107">Натиснете и задръжте (или щракнете с десния бутон върху) името на Bluetooth адаптера и щракнете **върху Деинсталиране на устройство**.</span><span class="sxs-lookup"><span data-stu-id="f0b1a-107">Press and hold (or right-click) the Bluetooth adapter name and click **Uninstall device**.</span></span>

2. <span data-ttu-id="f0b1a-108">Изключете устройството си с Windows, изчакайте няколко секунди и след това го включете отново.</span><span class="sxs-lookup"><span data-stu-id="f0b1a-108">Shut down your Windows device, wait a few seconds, and then turn it back on.</span></span> <span data-ttu-id="f0b1a-109">Windows ще се опита да преинсталира драйвера.</span><span class="sxs-lookup"><span data-stu-id="f0b1a-109">Windows will try to reinstall the driver.</span></span>

<span data-ttu-id="f0b1a-110">Ако наскоро сте инсталирали актуализации на Windows 10 или сте надстроени до Windows 10, може да искате да проверите за актуализации на драйвери:</span><span class="sxs-lookup"><span data-stu-id="f0b1a-110">If you recently installed Windows 10 updates or upgraded to Windows 10, you may want to check for driver updates:</span></span>

1. <span data-ttu-id="f0b1a-111">В Диспечер на устройствата щракнете върху **Bluetooth** и след това щракнете върху името на Bluetooth адаптера (което може да включва думата "радио").</span><span class="sxs-lookup"><span data-stu-id="f0b1a-111">In Device Manager, click **Bluetooth**, and then click the Bluetooth adapter name (which may include the word "radio").</span></span>

2. <span data-ttu-id="f0b1a-112">Натиснете и задръжте (или щракнете с десния бутон върху) Bluetooth адаптера и след това щракнете върху Автоматично актуализиране на  >  **драйвера Търсене на актуализиран софтуерен драйвер**.</span><span class="sxs-lookup"><span data-stu-id="f0b1a-112">Press and hold (or right-click) the Bluetooth adapter, and then click **Update driver** > **Search automatically for updated driver software**.</span></span> <span data-ttu-id="f0b1a-113">Следвайте стъпките, след което щракнете върху **Затвори**.</span><span class="sxs-lookup"><span data-stu-id="f0b1a-113">Follow the steps, then click **Close**.</span></span>

      - <span data-ttu-id="f0b1a-114">Ако Windows не може да намери нов Bluetooth драйвер, посетете уеб сайта на производителя на компютъра и изтеглете най-новия Bluetooth драйвер оттам.</span><span class="sxs-lookup"><span data-stu-id="f0b1a-114">If Windows can't find a new Bluetooth driver, visit the PC manufacturer's website and download the latest Bluetooth driver from there.</span></span>

    - <span data-ttu-id="f0b1a-115">След като го изтеглите, щракнете върху Актуализирай драйвера Преглед на моя компютър за софтуерен драйвер Потърсете местоположението, където се съхраняват файловете на  >    >   драйвера, > **OK**  >  **Напред** и следвайте стъпките, за да инсталирате.</span><span class="sxs-lookup"><span data-stu-id="f0b1a-115">After you download it, click **Update driver** > **Browse my computer for driver software** > **Browse** for the location where the driver files are stored > **OK** > **Next**, and follow the steps to install.</span></span>

3. <span data-ttu-id="f0b1a-116">След като инсталирате актуализирания драйвер, рестартирайте компютъра и след това проверете дали това коригира проблема с връзката.</span><span class="sxs-lookup"><span data-stu-id="f0b1a-116">After installing the updated driver, restart the machine, and then check whether that fixes the connection issue.</span></span>

<span data-ttu-id="f0b1a-117">За повече подробности как да отстранявате проблеми с Bluetooth, вижте пълната статия Отстраняване [на проблеми с Bluetooth в Windows 10](https://support.microsoft.com/help/14169/windows-10-fix-bluetooth-problems).</span><span class="sxs-lookup"><span data-stu-id="f0b1a-117">For more details of how to troubleshoot Bluetooth problems, please see the full article, [Fix Bluetooth problems in Windows 10](https://support.microsoft.com/help/14169/windows-10-fix-bluetooth-problems).</span></span>
