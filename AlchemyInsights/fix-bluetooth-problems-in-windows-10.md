---
title: Отстраняване на проблеми с Bluetooth в Windows 10
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
- "9001475"
- "3506"
ms.openlocfilehash: 7e7a397a1f6777972a81bcbb6bffa1c98d8370a4
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: bg-BG
ms.lasthandoff: 09/14/2020
ms.locfileid: "47730148"
---
# <a name="fix-bluetooth-problems-in-windows-10"></a><span data-ttu-id="9c5f6-102">Отстраняване на проблеми с Bluetooth в Windows 10</span><span class="sxs-lookup"><span data-stu-id="9c5f6-102">Fix Bluetooth problems in Windows 10</span></span>

<span data-ttu-id="9c5f6-103">Ако иконата на Bluetooth липсва или Bluetooth не може да бъде включен или изключен, може да поискате да изпълните програмата за отстраняване на неизправности с Bluetooth.</span><span class="sxs-lookup"><span data-stu-id="9c5f6-103">If the Bluetooth icon is missing or Bluetooth can't be turned on or off, you may want to run the Bluetooth troubleshooter.</span></span> <span data-ttu-id="9c5f6-104">[Отворете настройките за отстраняване на неизправности](ms-settings:troubleshoot), щракнете върху **Bluetooth** под **намиране и отстраняване на други проблеми**, щракнете върху **изпълнение на програмата за отстраняване на неизправности**.</span><span class="sxs-lookup"><span data-stu-id="9c5f6-104">[Open the Troubleshoot settings](ms-settings:troubleshoot), click **Bluetooth** under **Find and fix other problems**, click **Run the troubleshooter**.</span></span>

<span data-ttu-id="9c5f6-105">Ако не виждате иконата Bluetooth, но Bluetooth се показва в диспечера на устройствата:</span><span class="sxs-lookup"><span data-stu-id="9c5f6-105">If you don't see the Bluetooth icon, but Bluetooth does appear in Device Manager:</span></span>

1. <span data-ttu-id="9c5f6-106">В диспечера на устройствата щракнете върху **Bluetooth**.</span><span class="sxs-lookup"><span data-stu-id="9c5f6-106">In Device Manager, click **Bluetooth**.</span></span> <span data-ttu-id="9c5f6-107">Натиснете и задръжте (или щракнете с десния бутон върху) името на Bluetooth картата и щракнете върху **Деинсталиране на устройството**.</span><span class="sxs-lookup"><span data-stu-id="9c5f6-107">Press and hold (or right-click) the Bluetooth adapter name and click **Uninstall device**.</span></span>

2. <span data-ttu-id="9c5f6-108">Изключете устройството си с Windows, изчакайте няколко секунди и след това го включете отново.</span><span class="sxs-lookup"><span data-stu-id="9c5f6-108">Shut down your Windows device, wait a few seconds, and then turn it back on.</span></span> <span data-ttu-id="9c5f6-109">Windows ще опита да преинсталира драйвера.</span><span class="sxs-lookup"><span data-stu-id="9c5f6-109">Windows will try to reinstall the driver.</span></span>

<span data-ttu-id="9c5f6-110">Ако наскоро сте инсталирали актуализации за Windows 10 или сте надстроили до Windows 10, може да поискате да проверите за актуализации на драйвера:</span><span class="sxs-lookup"><span data-stu-id="9c5f6-110">If you recently installed Windows 10 updates or upgraded to Windows 10, you may want to check for driver updates:</span></span>

1. <span data-ttu-id="9c5f6-111">В диспечера на устройствата щракнете върху **Bluetooth**и след това щракнете върху името на Bluetooth адаптера (което може да включва думата "радио").</span><span class="sxs-lookup"><span data-stu-id="9c5f6-111">In Device Manager, click **Bluetooth**, and then click the Bluetooth adapter name (which may include the word "radio").</span></span>

2. <span data-ttu-id="9c5f6-112">Натиснете и задръжте (или щракнете с десния бутон върху) Bluetooth адаптера и след това щракнете върху **Актуализирай търсенето на драйвера**  >  **автоматично за актуализиран софтуер за драйвер**.</span><span class="sxs-lookup"><span data-stu-id="9c5f6-112">Press and hold (or right-click) the Bluetooth adapter, and then click **Update driver** > **Search automatically for updated driver software**.</span></span> <span data-ttu-id="9c5f6-113">Следвайте стъпките, след което щракнете върху **Затвори**.</span><span class="sxs-lookup"><span data-stu-id="9c5f6-113">Follow the steps, then click **Close**.</span></span>

      - <span data-ttu-id="9c5f6-114">Ако Windows не може да намери нов драйвер за Bluetooth, посетете уеб сайта на производителя на КОМПЮТЪРА и Изтеглете най-новия драйвер за Bluetooth оттам.</span><span class="sxs-lookup"><span data-stu-id="9c5f6-114">If Windows can't find a new Bluetooth driver, visit the PC manufacturer's website and download the latest Bluetooth driver from there.</span></span>

    - <span data-ttu-id="9c5f6-115">След като сте го изтеглили, щракнете върху **актуализиране на драйвера**  >  **за преглед на компютъра за драйвера за софтуерни продукти**  >  **Намерете** местоположението, където се съхраняват файловете на драйвера, > **OK**  >  **Next**и следвайте стъпките за инсталиране.</span><span class="sxs-lookup"><span data-stu-id="9c5f6-115">After you download it, click **Update driver** > **Browse my computer for driver software** > **Browse** for the location where the driver files are stored > **OK** > **Next**, and follow the steps to install.</span></span>

3. <span data-ttu-id="9c5f6-116">След като инсталирате актуализирания драйвер, рестартирайте компютъра и след това проверете дали това поправя проблема с връзката.</span><span class="sxs-lookup"><span data-stu-id="9c5f6-116">After installing the updated driver, restart the machine, and then check whether that fixes the connection issue.</span></span>

<span data-ttu-id="9c5f6-117">За повече информация как да отстраните проблеми с Bluetooth, вижте пълната статия, [Коригирайте проблеми с Bluetooth в Windows 10](https://support.microsoft.com/help/14169/windows-10-fix-bluetooth-problems).</span><span class="sxs-lookup"><span data-stu-id="9c5f6-117">For more details of how to troubleshoot Bluetooth problems, please see the full article, [Fix Bluetooth problems in Windows 10](https://support.microsoft.com/help/14169/windows-10-fix-bluetooth-problems).</span></span>
