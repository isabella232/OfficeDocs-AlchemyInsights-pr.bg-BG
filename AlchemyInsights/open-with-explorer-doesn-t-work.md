---
title: Отваряне с Explorer не работи
ms.author: toresing
author: tomresing
manager: scotv
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: b8f07022-69fe-4112-a2f6-d3a6cedb966c
ms.openlocfilehash: dc939a3451ff4fe95e4aa5a999839a2c532b398c
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: bg-BG
ms.lasthandoff: 04/22/2020
ms.locfileid: "43713023"
---
# <a name="open-with-explorer-isnt-working"></a><span data-ttu-id="60466-102">Отваряне с Explorer не работи</span><span class="sxs-lookup"><span data-stu-id="60466-102">Open with Explorer isn't working</span></span>

<span data-ttu-id="60466-103">Ако **отворете с Explorer** или изглед във **файловия мениджър** не работи уверете се, че уебклиент услугата е настроена на **изпълнява,** като следвате стъпките по-долу.</span><span class="sxs-lookup"><span data-stu-id="60466-103">If **Open with Explorer** or **View in File Explorer** doesn't work make sure the WebClient service is set to **Running** by following the steps below.</span></span> <span data-ttu-id="60466-104">Например може да отнеме много време, за да отворите библиотека на SharePoint или OneDrive, когато услугата не се изпълнява.</span><span class="sxs-lookup"><span data-stu-id="60466-104">For example, it might take a long time to open a SharePoint or OneDrive library when the service is not running.</span></span> 
  
1. <span data-ttu-id="60466-105">В полето за търсене на Windows въведете изпълнение, изберете изпълнение на десктоп приложение, въведете services.mscи след това изберете **Enter**.</span><span class="sxs-lookup"><span data-stu-id="60466-105">In the Windows search box, type run, select the Run desktop app, type services.msc, and then select **Enter**.</span></span>
    
2. <span data-ttu-id="60466-106">Превъртете надолу до услугата WebClient и проверете **колоната състояние.**</span><span class="sxs-lookup"><span data-stu-id="60466-106">Scroll down to the WebClient service and check the **Status** column.</span></span> <span data-ttu-id="60466-107">Ако състоянието на услугата WebClient не се **изпълнява**, щракнете двукратно върху услугата, щракнете върху **Старт**и след това щракнете върху **OK**.</span><span class="sxs-lookup"><span data-stu-id="60466-107">If the WebClient service status is not **Running**, double-click the service, click **Start**, and then click **OK**.</span></span> <span data-ttu-id="60466-108">Активирайте услугата, ако е необходимо, като изберете **ръчно** или **автоматично** в полето **Тип стартиране** .</span><span class="sxs-lookup"><span data-stu-id="60466-108">Enable the service, if needed, by selecting either **Manual** or **Automatic** in the **Startup type** box.</span></span> 
    
> [!NOTE]
> <span data-ttu-id="60466-109">За отстраняване на проблеми при отваряне във файловия мениджър, вижте [Отвори в Explorer](https://go.microsoft.com/fwlink/?linkid=871665).</span><span class="sxs-lookup"><span data-stu-id="60466-109">To troubleshoot issues opening in File Explorer, see [Open in Explorer](https://go.microsoft.com/fwlink/?linkid=871665).</span></span> <span data-ttu-id="60466-110">Разгледайте синхронизирането като по-добра алтернатива: [Синхронизиране на SharePoint файлове с новия oneDrive синхронизиране клиент](https://go.microsoft.com/fwlink/?linkid=871666).</span><span class="sxs-lookup"><span data-stu-id="60466-110">Explore sync as a better alternative: [Sync SharePoint files with the new OneDrive sync client](https://go.microsoft.com/fwlink/?linkid=871666).</span></span> 
  

