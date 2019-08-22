---
title: Отваряне с Explorer не работи
ms.author: toresing
author: tomresing
manager: scotv
ms.date: 12/10/2018
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: b8f07022-69fe-4112-a2f6-d3a6cedb966c
ms.openlocfilehash: 7680766b53bd5e85789375d3f9e9ab635780ec6c
ms.sourcegitcommit: 1d98db8acb9959aba3b5e308a567ade6b62da56c
ms.translationtype: MT
ms.contentlocale: bg-BG
ms.lasthandoff: 08/22/2019
ms.locfileid: "36538450"
---
# <a name="open-with-explorer-isnt-working"></a><span data-ttu-id="75d50-102">Отваряне с Explorer не работи</span><span class="sxs-lookup"><span data-stu-id="75d50-102">Open with Explorer isn't working</span></span>

<span data-ttu-id="75d50-103">Ако **Отваряне с Explorer** или **мнение в File Explorer** не работи се уверете, че услугата на WebClient е настроен да **работи** като следвате стъпките по-долу.</span><span class="sxs-lookup"><span data-stu-id="75d50-103">If **Open with Explorer** or **View in File Explorer** doesn't work make sure the WebClient service is set to **Running** by following the steps below.</span></span> <span data-ttu-id="75d50-104">Например това може да отнеме дълго време за отваряне на SharePoint или OneDrive Библиотека, когато услугата не се изпълнява.</span><span class="sxs-lookup"><span data-stu-id="75d50-104">For example, it might take a long time to open a SharePoint or OneDrive library when the service is not running.</span></span> 
  
1. <span data-ttu-id="75d50-105">В Windows полето за търсене въведете тичам, изберете Run работния плот ап, вид services.msc и след това изберете **Enter**.</span><span class="sxs-lookup"><span data-stu-id="75d50-105">In the Windows search box, type run, select the Run desktop app, type services.msc, and then select **Enter**.</span></span>
    
2. <span data-ttu-id="75d50-106">Превъртете надолу до услугата на WebClient и проверете колоната **състояние** .</span><span class="sxs-lookup"><span data-stu-id="75d50-106">Scroll down to the WebClient service and check the **Status** column.</span></span> <span data-ttu-id="75d50-107">Ако състоянието на WebClient услуга не се **изпълнява**, щракнете двукратно върху услугата, щракнете върху **Старт**и след това щракнете върху **OK**.</span><span class="sxs-lookup"><span data-stu-id="75d50-107">If the WebClient service status is not **Running**, double-click the service, click **Start**, and then click **OK**.</span></span> <span data-ttu-id="75d50-108">Разреши услугата, ако е необходимо, избирайки или **ръчно** или **автоматично** в полето **тип на стартиране** .</span><span class="sxs-lookup"><span data-stu-id="75d50-108">Enable the service, if needed, by selecting either **Manual** or **Automatic** in the **Startup type** box.</span></span> 
    
> [!NOTE]
> <span data-ttu-id="75d50-109">За да отстраните проблеми с отварянето в File Explorer, вижте [отворен in Изследовател](https://go.microsoft.com/fwlink/?linkid=871665).</span><span class="sxs-lookup"><span data-stu-id="75d50-109">To troubleshoot issues opening in File Explorer, see [Open in Explorer](https://go.microsoft.com/fwlink/?linkid=871665).</span></span> <span data-ttu-id="75d50-110">Разгледайте синхронизация като по-добра алтернатива: [файлове за синхронизиране на SharePoint с новия клиент, OneDrive синхронизиране](https://go.microsoft.com/fwlink/?linkid=871666).</span><span class="sxs-lookup"><span data-stu-id="75d50-110">Explore sync as a better alternative: [Sync SharePoint files with the new OneDrive sync client](https://go.microsoft.com/fwlink/?linkid=871666).</span></span> 
  

