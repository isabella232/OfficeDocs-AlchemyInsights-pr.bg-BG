---
title: Отстраняване на проблеми с помощта на "отваряне с Explorer"
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
ms.assetid: ed852342-e33f-4450-8400-63d30df09476
ms.openlocfilehash: e7fe59b94d216d89c2f2f7100a3d8bf7a0b0196e
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: bg-BG
ms.lasthandoff: 09/14/2020
ms.locfileid: "47659047"
---
# <a name="fix-problems-with-open-with-explorer"></a><span data-ttu-id="79e14-102">Отстраняване на проблеми с "отваряне с Explorer"</span><span class="sxs-lookup"><span data-stu-id="79e14-102">Fix problems with Open with Explorer</span></span>

<span data-ttu-id="79e14-103">Коригиране на често срещани проблеми при отваряне на библиотека с документи в SharePoint или OneDrive с помощта на командата " **Отваряне с Explorer** ":</span><span class="sxs-lookup"><span data-stu-id="79e14-103">Fix common problems with opening a document library in SharePoint or OneDrive using the **Open with Explorer** command:</span></span> 
  
- <span data-ttu-id="79e14-104">Използвайте Internet Explorer 10 или Internet Explorer 11.</span><span class="sxs-lookup"><span data-stu-id="79e14-104">Use Internet Explorer 10 or Internet Explorer 11.</span></span> <span data-ttu-id="79e14-105">**Отварянето с Explorer** не е съвместимо с Microsoft Edge, Google Chrome, Firefox и други.</span><span class="sxs-lookup"><span data-stu-id="79e14-105">**Open with Explorer** isn't compatible with Microsoft Edge, Google Chrome, Firefox and others.</span></span> <span data-ttu-id="79e14-106">**Отваряне с Explorer** е забранено във всички браузъри, с изключение на Internet Explorer.</span><span class="sxs-lookup"><span data-stu-id="79e14-106">**Open with Explorer** is disabled in all browsers except Internet Explorer.</span></span> 
    
- <span data-ttu-id="79e14-107">Опцията " **Отваряне с Explorer** " не е налична в съвременната среда за библиотеки на SharePoint.</span><span class="sxs-lookup"><span data-stu-id="79e14-107">**Open with Explorer** is not available in the modern experience for SharePoint libraries.</span></span> <span data-ttu-id="79e14-108">Вместо това използвайте **изгледа във File Explorer** .</span><span class="sxs-lookup"><span data-stu-id="79e14-108">Use **View in File Explorer** instead.</span></span> <span data-ttu-id="79e14-109">Изберете изглед на **Опции** \> **за преглед във файловия мениджър**.</span><span class="sxs-lookup"><span data-stu-id="79e14-109">Select **View options** \> **View in File Explorer**.</span></span> <span data-ttu-id="79e14-110">Изгледът във File Explorer не е съвместим с Microsoft Edge, Google Chrome, Firefox и други.</span><span class="sxs-lookup"><span data-stu-id="79e14-110">View in File Explorer is not compatible with Microsoft Edge, Google Chrome, Firefox and others.</span></span> <span data-ttu-id="79e14-111">Можете да **преглеждате файловия мениджър** само в Internet Explorer.</span><span class="sxs-lookup"><span data-stu-id="79e14-111">**View in File Explorer** in available only in Internet Explorer.</span></span> 
    
- <span data-ttu-id="79e14-112">Уверете се, че услугата WebClient се изпълнява.</span><span class="sxs-lookup"><span data-stu-id="79e14-112">Make sure the WebClient service is running.</span></span> <span data-ttu-id="79e14-113">В полето за търсене на Windows въведете Run, изберете изпълнение на настолното приложение, въведете Services. msc и след това натиснете клавиша ENTER.</span><span class="sxs-lookup"><span data-stu-id="79e14-113">In the Windows search box, type run, select the Run desktop app, type services.msc, and then press Enter.</span></span> <span data-ttu-id="79e14-114">Превъртете надолу до услугата WebClient и се уверете, че колоната **състояние** показва "изпълнява се."</span><span class="sxs-lookup"><span data-stu-id="79e14-114">Scroll down to the WebClient service and make sure the **Status** column displays "Running."</span></span> <span data-ttu-id="79e14-115">Ако не е, щракнете двукратно върху услугата, щракнете върху **Старт**, след което щракнете върху **OK**.</span><span class="sxs-lookup"><span data-stu-id="79e14-115">If it doesn't, double-click the service, click **Start**, and then click **OK**.</span></span> <span data-ttu-id="79e14-116">(Може да се наложи първо да разрешите услугата, като изберете **ръчна** или **Автоматична** в полето **тип стартиране** .)</span><span class="sxs-lookup"><span data-stu-id="79e14-116">(You might need to first enable the service by selecting either **Manual** or **Automatic** in the **Startup type** box.)</span></span> 
    
> [!NOTE]
> <span data-ttu-id="79e14-117">Отварянето на библиотека във файловия мениджър е удобно, ако трябва да копирате или да местите няколко файла и папки веднъж, но ако искате да работите редовно в библиотеката, ви препоръчваме да го синхронизирате.</span><span class="sxs-lookup"><span data-stu-id="79e14-117">Opening a library in File Explorer is handy if you need to copy or move multiple files and folders once, but if you want to regularly work in the library, we recommend syncing it.</span></span> <span data-ttu-id="79e14-118">За отстраняване на проблеми при отваряне във File Explorer вижте [Отваряне в Explorer](https://go.microsoft.com/fwlink/?linkid=871665).</span><span class="sxs-lookup"><span data-stu-id="79e14-118">To troubleshoot issues opening in File Explorer, see [Open in Explorer](https://go.microsoft.com/fwlink/?linkid=871665).</span></span> <span data-ttu-id="79e14-119">За информация относно настройването на синхронизирането вижте [Синхронизиране на файлове на SharePoint с новия клиент за синхронизиране на OneDrive](https://go.microsoft.com/fwlink/?linkid=871666).</span><span class="sxs-lookup"><span data-stu-id="79e14-119">For info about setting up sync, see [Sync SharePoint files with the new OneDrive sync client](https://go.microsoft.com/fwlink/?linkid=871666).</span></span>
  
<span data-ttu-id="79e14-120">Вижте статията [как да използвате командата "отваряне с Explorer", за да отстранявате проблеми в SharePoint online](https://docs.microsoft.com/sharepoint/support/lists-and-libraries/troubleshoot-issues-using-open-with-explorer) за повече информация.</span><span class="sxs-lookup"><span data-stu-id="79e14-120">Please see the article [How to use the "Open with Explorer" command to troubleshoot issues in SharePoint Online](https://docs.microsoft.com/sharepoint/support/lists-and-libraries/troubleshoot-issues-using-open-with-explorer) for more information.</span></span> 
  

