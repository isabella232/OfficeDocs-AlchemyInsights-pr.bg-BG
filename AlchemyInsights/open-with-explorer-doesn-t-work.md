---
title: Отваряне с Explorer не работи
ms.author: toresing
author: tomresing
manager: scotv
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: b8f07022-69fe-4112-a2f6-d3a6cedb966c
ms.openlocfilehash: 5bf28982533d8ca9998605cf3592f317c0ef99b0
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: bg-BG
ms.lasthandoff: 09/14/2020
ms.locfileid: "47694445"
---
# <a name="open-with-explorer-isnt-working"></a><span data-ttu-id="8d587-102">Отваряне с Explorer не работи</span><span class="sxs-lookup"><span data-stu-id="8d587-102">Open with Explorer isn't working</span></span>

<span data-ttu-id="8d587-103">Ако **отворен с Explorer** или **изглед във File Explorer** не работи, уверете се, че услугата WebClient е настроена да се **изпълнява** , като следвате стъпките по-долу.</span><span class="sxs-lookup"><span data-stu-id="8d587-103">If **Open with Explorer** or **View in File Explorer** doesn't work make sure the WebClient service is set to **Running** by following the steps below.</span></span> <span data-ttu-id="8d587-104">Например може да отнеме много време, за да отворите библиотека на SharePoint или OneDrive, когато услугата не се изпълнява.</span><span class="sxs-lookup"><span data-stu-id="8d587-104">For example, it might take a long time to open a SharePoint or OneDrive library when the service is not running.</span></span> 
  
1. <span data-ttu-id="8d587-105">В полето за търсене на Windows въведете Run, изберете изпълнение на настолното приложение, въведете Services. msc и след това изберете **Enter**.</span><span class="sxs-lookup"><span data-stu-id="8d587-105">In the Windows search box, type run, select the Run desktop app, type services.msc, and then select **Enter**.</span></span>
    
2. <span data-ttu-id="8d587-106">Превъртете надолу до WebClient услугата и проверете колоната **състояние** .</span><span class="sxs-lookup"><span data-stu-id="8d587-106">Scroll down to the WebClient service and check the **Status** column.</span></span> <span data-ttu-id="8d587-107">Ако състоянието на услугата WebClient не се **изпълнява**, щракнете двукратно върху услугата, изберете **Старт**и след това щракнете върху **OK**.</span><span class="sxs-lookup"><span data-stu-id="8d587-107">If the WebClient service status is not **Running**, double-click the service, click **Start**, and then click **OK**.</span></span> <span data-ttu-id="8d587-108">Разрешете услугата, ако е необходимо, като изберете **ръчна** или **Автоматична** в полето **тип на стартиране** .</span><span class="sxs-lookup"><span data-stu-id="8d587-108">Enable the service, if needed, by selecting either **Manual** or **Automatic** in the **Startup type** box.</span></span> 
    
> [!NOTE]
> <span data-ttu-id="8d587-109">За отстраняване на проблеми при отваряне във File Explorer вижте [Отваряне в Explorer](https://go.microsoft.com/fwlink/?linkid=871665).</span><span class="sxs-lookup"><span data-stu-id="8d587-109">To troubleshoot issues opening in File Explorer, see [Open in Explorer](https://go.microsoft.com/fwlink/?linkid=871665).</span></span> <span data-ttu-id="8d587-110">Изследвайте синхронизирането като по-добра алтернатива: [Синхронизиране на файлове на SharePoint с новия клиент за синхронизиране на OneDrive](https://go.microsoft.com/fwlink/?linkid=871666).</span><span class="sxs-lookup"><span data-stu-id="8d587-110">Explore sync as a better alternative: [Sync SharePoint files with the new OneDrive sync client](https://go.microsoft.com/fwlink/?linkid=871666).</span></span> 
  

