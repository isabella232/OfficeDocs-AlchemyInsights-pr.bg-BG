---
title: Отваряне с Explorer не работи
ms.author: toresing
author: tomresing
manager: scotv
ms.date: 12/10/2018
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom: Adm_O365
ms.assetid: b8f07022-69fe-4112-a2f6-d3a6cedb966c
ms.openlocfilehash: b55fc7bd5670e655334ef7be368b245c8899633a
ms.sourcegitcommit: e2864efcfb493b6e46b662b746661a61232bdba7
ms.translationtype: MT
ms.contentlocale: bg-BG
ms.lasthandoff: 01/24/2019
ms.locfileid: "29457771"
---
# <a name="open-with-explorer-isnt-working"></a><span data-ttu-id="e70cc-102">Отваряне с Explorer не работи</span><span class="sxs-lookup"><span data-stu-id="e70cc-102">Open with Explorer isn't working</span></span>

<span data-ttu-id="e70cc-p101">Ако **Отваряне с Explorer** или **мнение в File Explorer** не работи се уверете, че услугата на WebClient е настроен да **работи** като следвате стъпките по-долу. Например това може да отнеме дълго време за отваряне на SharePoint или OneDrive Библиотека, когато услугата не се изпълнява.</span><span class="sxs-lookup"><span data-stu-id="e70cc-p101">If **Open with Explorer** or **View in File Explorer** doesn't work make sure the WebClient service is set to **Running** by following the steps below. For example, it might take a long time to open a SharePoint or OneDrive library when the service is not running.</span></span> 
  
1. <span data-ttu-id="e70cc-105">В Windows полето за търсене въведете тичам, изберете Run работния плот ап, вид services.msc и след това изберете **Enter**.</span><span class="sxs-lookup"><span data-stu-id="e70cc-105">In the Windows search box, type run, select the Run desktop app, type services.msc, and then select **Enter**.</span></span>
    
2. <span data-ttu-id="e70cc-p102">Превъртете надолу до услугата на WebClient и проверете колоната **състояние** . Ако състоянието на WebClient услуга не се **изпълнява**, щракнете двукратно върху услугата, щракнете върху **Старт**и след това щракнете върху **OK**. Разреши услугата, ако е необходимо, избирайки или **ръчно** или **автоматично** в полето **тип на стартиране** .</span><span class="sxs-lookup"><span data-stu-id="e70cc-p102">Scroll down to the WebClient service and check the **Status** column. If the WebClient service status is not **Running**, double-click the service, click **Start**, and then click **OK**. Enable the service, if needed, by selecting either **Manual** or **Automatic** in the **Startup type** box.</span></span> 
    
> [!NOTE]
> <span data-ttu-id="e70cc-p103">За да отстраните проблеми с отварянето в File Explorer, вижте [отворен in Изследовател](https://go.microsoft.com/fwlink/?linkid=871665). Разгледайте синхронизация като по-добра алтернатива: [файлове за синхронизиране на SharePoint с новия клиент, OneDrive синхронизиране](https://go.microsoft.com/fwlink/?linkid=871666).</span><span class="sxs-lookup"><span data-stu-id="e70cc-p103">To troubleshoot issues opening in File Explorer, see [Open in Explorer](https://go.microsoft.com/fwlink/?linkid=871665). Explore sync as a better alternative: [Sync SharePoint files with the new OneDrive sync client](https://go.microsoft.com/fwlink/?linkid=871666).</span></span> 
  

