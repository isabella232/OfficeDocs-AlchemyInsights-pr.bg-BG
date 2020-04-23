---
title: Отстраняване на проблеми с помощта на Отваряне с Explorer
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
ms.assetid: ed852342-e33f-4450-8400-63d30df09476
ms.openlocfilehash: cb26876d93a110b3b0addd7821206215c783f959
ms.sourcegitcommit: 631cbb5f03e5371f0995e976536d24e9d13746c3
ms.translationtype: MT
ms.contentlocale: bg-BG
ms.lasthandoff: 04/22/2020
ms.locfileid: "43759681"
---
# <a name="fix-problems-with-open-with-explorer"></a><span data-ttu-id="2f917-102">Отстраняване на проблеми с Отваряне с Explorer</span><span class="sxs-lookup"><span data-stu-id="2f917-102">Fix problems with Open with Explorer</span></span>

<span data-ttu-id="2f917-103">Отстраняване на често срещани проблеми при отваряне на библиотека с документи в SharePoint или OneDrive с помощта на командата **Отвори с Explorer:**</span><span class="sxs-lookup"><span data-stu-id="2f917-103">Fix common problems with opening a document library in SharePoint or OneDrive using the **Open with Explorer** command:</span></span> 
  
- <span data-ttu-id="2f917-104">Използване на Internet Explorer 10 или Internet Explorer 11.</span><span class="sxs-lookup"><span data-stu-id="2f917-104">Use Internet Explorer 10 or Internet Explorer 11.</span></span> <span data-ttu-id="2f917-105">**Отварянето с Explorer** не е съвместимо с Microsoft Edge, Google Chrome, Firefox и други.</span><span class="sxs-lookup"><span data-stu-id="2f917-105">**Open with Explorer** isn't compatible with Microsoft Edge, Google Chrome, Firefox and others.</span></span> <span data-ttu-id="2f917-106">**Отварянето с Explorer** е забранено във всички браузъри с изключение на Internet Explorer.</span><span class="sxs-lookup"><span data-stu-id="2f917-106">**Open with Explorer** is disabled in all browsers except Internet Explorer.</span></span> 
    
- <span data-ttu-id="2f917-107">**Отваряне с Explorer** не е налична в съвременния опит за библиотеки на SharePoint.</span><span class="sxs-lookup"><span data-stu-id="2f917-107">**Open with Explorer** is not available in the modern experience for SharePoint libraries.</span></span> <span data-ttu-id="2f917-108">Вместо това използвайте **изгледа във файловия мениджър.**</span><span class="sxs-lookup"><span data-stu-id="2f917-108">Use **View in File Explorer** instead.</span></span> <span data-ttu-id="2f917-109">Изберете **Опции за** \> **изглед в файловия мениджър**.</span><span class="sxs-lookup"><span data-stu-id="2f917-109">Select **View options** \> **View in File Explorer**.</span></span> <span data-ttu-id="2f917-110">Преглед във файловия мениджър не е съвместим с Microsoft Edge, Google Chrome, Firefox и др.</span><span class="sxs-lookup"><span data-stu-id="2f917-110">View in File Explorer is not compatible with Microsoft Edge, Google Chrome, Firefox and others.</span></span> <span data-ttu-id="2f917-111">**Преглед на файловия мениджър** в наличност само в Internet Explorer.</span><span class="sxs-lookup"><span data-stu-id="2f917-111">**View in File Explorer** in available only in Internet Explorer.</span></span> 
    
- <span data-ttu-id="2f917-112">Уверете се, че услугата WebClient се изпълнява.</span><span class="sxs-lookup"><span data-stu-id="2f917-112">Make sure the WebClient service is running.</span></span> <span data-ttu-id="2f917-113">В полето за търсене на Windows въведете изпълнение, изберете изпълнение на работния плот приложение, въведете services.mscи натиснете Enter.</span><span class="sxs-lookup"><span data-stu-id="2f917-113">In the Windows search box, type run, select the Run desktop app, type services.msc, and then press Enter.</span></span> <span data-ttu-id="2f917-114">Превъртете надолу до услугата WebClient и се уверете, че колоната **състояние** показва "Бягане".</span><span class="sxs-lookup"><span data-stu-id="2f917-114">Scroll down to the WebClient service and make sure the **Status** column displays "Running."</span></span> <span data-ttu-id="2f917-115">Ако не, щракнете двукратно върху услугата, щракнете върху **Старт**и след това щракнете върху **OK**.</span><span class="sxs-lookup"><span data-stu-id="2f917-115">If it doesn't, double-click the service, click **Start**, and then click **OK**.</span></span> <span data-ttu-id="2f917-116">(Може да се наложи първо да разрешите услугата, като изберете **ръчно** или **автоматично** в полето **Тип стартиране.)**</span><span class="sxs-lookup"><span data-stu-id="2f917-116">(You might need to first enable the service by selecting either **Manual** or **Automatic** in the **Startup type** box.)</span></span> 
    
> [!NOTE]
> <span data-ttu-id="2f917-117">Отварянето на библиотека във файловия мениджър е удобно, ако трябва да копирате или премествате няколко файла и папки веднъж, но ако искате редовно да работите в библиотеката, препоръчваме да го синхронизирате.</span><span class="sxs-lookup"><span data-stu-id="2f917-117">Opening a library in File Explorer is handy if you need to copy or move multiple files and folders once, but if you want to regularly work in the library, we recommend syncing it.</span></span> <span data-ttu-id="2f917-118">За отстраняване на проблеми при отваряне във файловия мениджър, вижте [Отвори в Explorer](https://go.microsoft.com/fwlink/?linkid=871665).</span><span class="sxs-lookup"><span data-stu-id="2f917-118">To troubleshoot issues opening in File Explorer, see [Open in Explorer](https://go.microsoft.com/fwlink/?linkid=871665).</span></span> <span data-ttu-id="2f917-119">За информация относно настройката на синхронизиране, вижте [Синхронизиране на SharePoint файлове с новия oneDrive синхронизиране клиент](https://go.microsoft.com/fwlink/?linkid=871666).</span><span class="sxs-lookup"><span data-stu-id="2f917-119">For info about setting up sync, see [Sync SharePoint files with the new OneDrive sync client](https://go.microsoft.com/fwlink/?linkid=871666).</span></span>
  
<span data-ttu-id="2f917-120">Вижте статията [Как да използвате командата "Отвори с Explorer" за отстраняване на проблеми в SharePoint Online](https://docs.microsoft.com/sharepoint/support/lists-and-libraries/troubleshoot-issues-using-open-with-explorer) за повече информация.</span><span class="sxs-lookup"><span data-stu-id="2f917-120">Please see the article [How to use the "Open with Explorer" command to troubleshoot issues in SharePoint Online](https://docs.microsoft.com/sharepoint/support/lists-and-libraries/troubleshoot-issues-using-open-with-explorer) for more information.</span></span> 
  

