---
title: Отстраняване на проблеми с помощта на Open с Explorer
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
ms.assetid: ed852342-e33f-4450-8400-63d30df09476
ms.openlocfilehash: a9ab7dd27e4dc1bd76c93cc81260616063e638ed
ms.sourcegitcommit: a256e8680379c006287ae30996763051c4d9ff85
ms.translationtype: MT
ms.contentlocale: bg-BG
ms.lasthandoff: 09/04/2019
ms.locfileid: "36742722"
---
# <a name="fix-problems-with-open-with-explorer"></a><span data-ttu-id="140eb-102">Отстраняване на проблеми с Open с Explorer</span><span class="sxs-lookup"><span data-stu-id="140eb-102">Fix problems with Open with Explorer</span></span>

<span data-ttu-id="140eb-103">Отстраняване на често срещани проблеми с отварянето на библиотека с документи в SharePoint или OneDrive с помощта на командата **Open с Explorer** :</span><span class="sxs-lookup"><span data-stu-id="140eb-103">Fix common problems with opening a document library in SharePoint or OneDrive using the **Open with Explorer** command:</span></span> 
  
- <span data-ttu-id="140eb-104">Използвайте Internet Explorer 10 или Internet Explorer 11.</span><span class="sxs-lookup"><span data-stu-id="140eb-104">Use Internet Explorer 10 or Internet Explorer 11.</span></span> <span data-ttu-id="140eb-105">**Open с Explorer** не е съвместим с Microsoft Edge, Google Chrome, Firefox и други.</span><span class="sxs-lookup"><span data-stu-id="140eb-105">**Open with Explorer** isn't compatible with Microsoft Edge, Google Chrome, Firefox and others.</span></span> <span data-ttu-id="140eb-106">**Open с Explorer** е забранена във всички браузъри с изключение на Internet Explorer.</span><span class="sxs-lookup"><span data-stu-id="140eb-106">**Open with Explorer** is disabled in all browsers except Internet Explorer.</span></span> 
    
- <span data-ttu-id="140eb-107">**Open с Explorer** не е наличен в съвременното преживяване за библиотеките на SharePoint.</span><span class="sxs-lookup"><span data-stu-id="140eb-107">**Open with Explorer** is not available in the modern experience for SharePoint libraries.</span></span> <span data-ttu-id="140eb-108">Вместо това използвайте **изглед във файловия мениджър** .</span><span class="sxs-lookup"><span data-stu-id="140eb-108">Use **View in File Explorer** instead.</span></span> <span data-ttu-id="140eb-109">Изберете изглед на **Опции** \> **за изглед във файловия мениджър**.</span><span class="sxs-lookup"><span data-stu-id="140eb-109">Select **View options** \> **View in File Explorer**.</span></span> <span data-ttu-id="140eb-110">Изгледът във файловия мениджър не е съвместим с Microsoft Edge, Google Chrome, Firefox и други.</span><span class="sxs-lookup"><span data-stu-id="140eb-110">View in File Explorer is not compatible with Microsoft Edge, Google Chrome, Firefox and others.</span></span> <span data-ttu-id="140eb-111">**Преглед във файловия мениджър** в наличен само в Internet Explorer.</span><span class="sxs-lookup"><span data-stu-id="140eb-111">**View in File Explorer** in available only in Internet Explorer.</span></span> 
    
- <span data-ttu-id="140eb-112">Уверете се, че услугата WebClient се изпълнява.</span><span class="sxs-lookup"><span data-stu-id="140eb-112">Make sure the WebClient service is running.</span></span> <span data-ttu-id="140eb-113">В полето за търсене на Windows въведете Run, изберете изпълнение на настолното приложение, въведете Services. msc и след това натиснете ENTER.</span><span class="sxs-lookup"><span data-stu-id="140eb-113">In the Windows search box, type run, select the Run desktop app, type services.msc, and then press Enter.</span></span> <span data-ttu-id="140eb-114">Превъртете надолу до услугата WebClient и се уверете, че колоната **състояние** показва "изпълнение".</span><span class="sxs-lookup"><span data-stu-id="140eb-114">Scroll down to the WebClient service and make sure the **Status** column displays "Running."</span></span> <span data-ttu-id="140eb-115">Ако не, щракнете двукратно върху услугата, щракнете върху **старти**след това щракнете върху **OK**.</span><span class="sxs-lookup"><span data-stu-id="140eb-115">If it doesn't, double-click the service, click **Start**, and then click **OK**.</span></span> <span data-ttu-id="140eb-116">(Може да се наложи първо да разрешите услугата, като изберете **ръчно** или **автоматично** в полето **тип стартиране** .)</span><span class="sxs-lookup"><span data-stu-id="140eb-116">(You might need to first enable the service by selecting either **Manual** or **Automatic** in the **Startup type** box.)</span></span> 
    
> [!NOTE]
> <span data-ttu-id="140eb-117">Отварянето на библиотека във файловия мениджър е удобно, ако трябва да копирате или премествате няколко файла и папки веднъж, но ако искате да работите редовно в библиотеката, ви препоръчваме да го синхронизирате.</span><span class="sxs-lookup"><span data-stu-id="140eb-117">Opening a library in File Explorer is handy if you need to copy or move multiple files and folders once, but if you want to regularly work in the library, we recommend syncing it.</span></span> <span data-ttu-id="140eb-118">За отстраняване на проблеми при отваряне на файловия мениджър вижте [Отваряне в Explorer](https://go.microsoft.com/fwlink/?linkid=871665).</span><span class="sxs-lookup"><span data-stu-id="140eb-118">To troubleshoot issues opening in File Explorer, see [Open in Explorer](https://go.microsoft.com/fwlink/?linkid=871665).</span></span> <span data-ttu-id="140eb-119">За информация относно настройването на синхронизацията вижте [Синхронизиране на SharePoint файлове с новия OneDrive синхронизиране на клиента](https://go.microsoft.com/fwlink/?linkid=871666).</span><span class="sxs-lookup"><span data-stu-id="140eb-119">For info about setting up sync, see [Sync SharePoint files with the new OneDrive sync client](https://go.microsoft.com/fwlink/?linkid=871666).</span></span>
  
<span data-ttu-id="140eb-120">Моля, вижте статията [как да използвате командата "отвори с Explorer" за отстраняване на проблеми в SharePoint online](https://docs.microsoft.com/sharepoint/support/lists-and-libraries/troubleshoot-issues-using-open-with-explorer) за повече информация.</span><span class="sxs-lookup"><span data-stu-id="140eb-120">Please see the article [How to use the "Open with Explorer" command to troubleshoot issues in SharePoint Online](https://docs.microsoft.com/sharepoint/support/lists-and-libraries/troubleshoot-issues-using-open-with-explorer) for more information.</span></span> 
  

