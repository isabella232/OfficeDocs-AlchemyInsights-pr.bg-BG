---
title: Отстраняване на проблеми с отворен с изследовател
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
ms.openlocfilehash: 03bb3ad01a716390ec50845b29ddf6cc81a83116
ms.sourcegitcommit: 03a156a9c9740521155a30775492c7dff0982588
ms.translationtype: MT
ms.contentlocale: bg-BG
ms.lasthandoff: 03/22/2019
ms.locfileid: "30759283"
---
# <a name="fix-problems-with-open-with-explorer"></a><span data-ttu-id="2a9c5-102">Отстраняване на проблеми при отваряне с Explorer</span><span class="sxs-lookup"><span data-stu-id="2a9c5-102">Fix problems with Open with Explorer</span></span>

<span data-ttu-id="2a9c5-103">Отстраните често срещани проблеми с отварянето на библиотека с документи в SharePoint или OneDrive, с помощта на командата **Отваряне с Explorer** :</span><span class="sxs-lookup"><span data-stu-id="2a9c5-103">Fix common problems with opening a document library in SharePoint or OneDrive using the **Open with Explorer** command:</span></span> 
  
- <span data-ttu-id="2a9c5-104">Използвайте Internet Explorer 10 или 11 на Internet Explorer.</span><span class="sxs-lookup"><span data-stu-id="2a9c5-104">Use Internet Explorer 10 or Internet Explorer 11.</span></span> <span data-ttu-id="2a9c5-105">**Отваряне с Explorer** не е съвместима с Microsoft ръб, Google Chrome, Firefox и др.</span><span class="sxs-lookup"><span data-stu-id="2a9c5-105">**Open with Explorer** isn't compatible with Microsoft Edge, Google Chrome, Firefox and others.</span></span> <span data-ttu-id="2a9c5-106">**Отваряне с Explorer** е забранено във всички браузъри освен Internet Explorer.</span><span class="sxs-lookup"><span data-stu-id="2a9c5-106">**Open with Explorer** is disabled in all browsers except Internet Explorer.</span></span> 
    
- <span data-ttu-id="2a9c5-107">**Отваряне с Explorer** не е налична в съвременният опит за библиотеки на SharePoint.</span><span class="sxs-lookup"><span data-stu-id="2a9c5-107">**Open with Explorer** is not available in the modern experience for SharePoint libraries.</span></span> <span data-ttu-id="2a9c5-108">Вместо това използвайте **изгледа в File Explorer** .</span><span class="sxs-lookup"><span data-stu-id="2a9c5-108">Use **View in File Explorer** instead.</span></span> <span data-ttu-id="2a9c5-109">Изберете **опциите за изглед** \> **мнение в File Explorer**.</span><span class="sxs-lookup"><span data-stu-id="2a9c5-109">Select **View options** \> **View in File Explorer**.</span></span> <span data-ttu-id="2a9c5-110">Мнение в File Explorer не е съвместим с Microsoft ръб, Google Chrome, Firefox и др.</span><span class="sxs-lookup"><span data-stu-id="2a9c5-110">View in File Explorer is not compatible with Microsoft Edge, Google Chrome, Firefox and others.</span></span> <span data-ttu-id="2a9c5-111">**Мнение в File Explorer** в достъпна само в Internet Explorer.</span><span class="sxs-lookup"><span data-stu-id="2a9c5-111">**View in File Explorer** in available only in Internet Explorer.</span></span> 
    
- <span data-ttu-id="2a9c5-112">Уверете се, че се изпълнява услугата на WebClient.</span><span class="sxs-lookup"><span data-stu-id="2a9c5-112">Make sure the WebClient service is running.</span></span> <span data-ttu-id="2a9c5-113">В полето за търсене на Windows въведете изпълни, изберете Run работния плот ап, вид services.msc и натиснете клавиша Enter.</span><span class="sxs-lookup"><span data-stu-id="2a9c5-113">In the Windows search box, type run, select the Run desktop app, type services.msc, and then press Enter.</span></span> <span data-ttu-id="2a9c5-114">Превъртете надолу до услугата на WebClient и се уверете, че колоната **състояние** показва "Движение."</span><span class="sxs-lookup"><span data-stu-id="2a9c5-114">Scroll down to the WebClient service and make sure the **Status** column displays "Running."</span></span> <span data-ttu-id="2a9c5-115">Ако това не стане, щракнете двукратно върху услугата, щракнете върху **Старт**и след това щракнете върху **OK**.</span><span class="sxs-lookup"><span data-stu-id="2a9c5-115">If it doesn't, double-click the service, click **Start**, and then click **OK**.</span></span> <span data-ttu-id="2a9c5-116">(Трябва да първо да разрешите услугата като изберете или **ръчно** или **автоматично** в полето **тип стартиране** .)</span><span class="sxs-lookup"><span data-stu-id="2a9c5-116">(You might need to first enable the service by selecting either **Manual** or **Automatic** in the **Startup type** box.)</span></span> 
    
> [!NOTE]
> <span data-ttu-id="2a9c5-117">Отваряне на библиотека в File Explorer е удобен, ако искате да копирате или преместите множество файлове и папки, веднъж, но ако искате да редовно работи в библиотеката, ние препоръчваме да го синхронизирате.</span><span class="sxs-lookup"><span data-stu-id="2a9c5-117">Opening a library in File Explorer is handy if you need to copy or move multiple files and folders once, but if you want to regularly work in the library, we recommend syncing it.</span></span> <span data-ttu-id="2a9c5-118">За да отстраните проблеми с отварянето в File Explorer, вижте [отворен in Изследовател](https://go.microsoft.com/fwlink/?linkid=871665).</span><span class="sxs-lookup"><span data-stu-id="2a9c5-118">To troubleshoot issues opening in File Explorer, see [Open in Explorer](https://go.microsoft.com/fwlink/?linkid=871665).</span></span> <span data-ttu-id="2a9c5-119">За информация за настройка на синхронизация вижте [файлове за синхронизиране на SharePoint с новия клиент, OneDrive синхронизиране](https://go.microsoft.com/fwlink/?linkid=871666).</span><span class="sxs-lookup"><span data-stu-id="2a9c5-119">For info about setting up sync, see [Sync SharePoint files with the new OneDrive sync client](https://go.microsoft.com/fwlink/?linkid=871666).</span></span>
  
<span data-ttu-id="2a9c5-120">Моля, вижте статията [как да използвате командата "отваряне с Explorer" за отстраняване на проблеми в SharePoint Online](https://support.office.com/article/How-to-use-the-Open-with-Explorer-command-to-troubleshoot-issues-in-SharePoint-Online-87155331-0c92-4224-a4c1-da5c21c4ade4) за повече информация.</span><span class="sxs-lookup"><span data-stu-id="2a9c5-120">Please see the article [How to use the "Open with Explorer" command to troubleshoot issues in SharePoint Online](https://support.office.com/article/How-to-use-the-Open-with-Explorer-command-to-troubleshoot-issues-in-SharePoint-Online-87155331-0c92-4224-a4c1-da5c21c4ade4) for more information.</span></span> 
  

