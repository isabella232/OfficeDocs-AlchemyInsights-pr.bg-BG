---
title: Спулерът за печат проблем е разрешен
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/8/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "5151"
- "9002659"
ms.openlocfilehash: 53b1c9a8efa3cc978af8b602c8ed90430042186a
ms.sourcegitcommit: 4265a9e79db6c2a396aa80ec0ebd467bbaadf366
ms.translationtype: MT
ms.contentlocale: bg-BG
ms.lasthandoff: 07/08/2020
ms.locfileid: "45088279"
---
# <a name="print-spooler-issue-is-resolved"></a><span data-ttu-id="4862f-102">Спулерът за печат проблем е разрешен</span><span class="sxs-lookup"><span data-stu-id="4862f-102">Print spooler issue is resolved</span></span>

<span data-ttu-id="4862f-103">Ако устройството ви е актуализирано с Windows 10 **OS Build 19041.329**, може да сте забелязали проблем, при който някои принтери не успяват да отпечатате.</span><span class="sxs-lookup"><span data-stu-id="4862f-103">If your device was updated with Windows 10  **OS Build 19041.329**, you might have observed an issue where certain printers fail to print.</span></span> <span data-ttu-id="4862f-104">Спулерът за печат може да хвърли грешка или неочаквано затвори при опит за печат и изход от засегнатия принтер.</span><span class="sxs-lookup"><span data-stu-id="4862f-104">The print spooler might throw an error or close unexpectedly when attempting to print, and no output comes from the affected printer.</span></span> <span data-ttu-id="4862f-105">Този проблем е разрешен в компилация на ОС **19041.331** [, KB4567523](https://support.microsoft.com/help/4567523/windows-10-update-kb4567523).</span><span class="sxs-lookup"><span data-stu-id="4862f-105">This issue is resolved in OS Build  **19041.331**, [KB4567523](https://support.microsoft.com/help/4567523/windows-10-update-kb4567523).</span></span>  

<span data-ttu-id="4862f-106">**Текущо разследване**</span><span class="sxs-lookup"><span data-stu-id="4862f-106">**Ongoing investigation**</span></span>

<span data-ttu-id="4862f-107">Локална защита орган подсистема (LSASS) файл (**Isass.exe**) може да се провали на някои устройства със съобщение за грешка, "процес на критична система, C:\WINDOWS\system32\Isass.exe, неуспешна с код на състоянието c0000008.</span><span class="sxs-lookup"><span data-stu-id="4862f-107">The Local Security Authority Subsystem Service (LSASS) file (**Isass.exe**) might fail on some devices with the error message, "A critical system process, C:\WINDOWS\system32\Isass.exe, failed with status code c0000008.</span></span> <span data-ttu-id="4862f-108">Машината трябва да се рестартира".</span><span class="sxs-lookup"><span data-stu-id="4862f-108">The machine must now be restarted".</span></span>  <span data-ttu-id="4862f-109">**Microsoft работи по решение и ще предостави актуализация в предстоящо издание.**</span><span class="sxs-lookup"><span data-stu-id="4862f-109">**Microsoft is working on a resolution and will provide an update in an upcoming release.**</span></span>

<span data-ttu-id="4862f-110">За повече информация, моля, вижте [Windows 10 версия 2004 известни проблеми](https://docs.microsoft.com/windows/release-information/status-windows-10-2004#442msgdesc).</span><span class="sxs-lookup"><span data-stu-id="4862f-110">For more information, please check out  [Windows 10 Version 2004 known issues](https://docs.microsoft.com/windows/release-information/status-windows-10-2004#442msgdesc).</span></span>