---
title: Отстраняване на проблеми с спулера за печат
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/8/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "5151"
- "9002659"
ms.openlocfilehash: 66b39434ef6f9ad2b8392f811704e67c1bcffd2b
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: HT
ms.contentlocale: bg-BG
ms.lasthandoff: 09/15/2020
ms.locfileid: "47801830"
---
# <a name="print-spooler-issue-is-resolved"></a><span data-ttu-id="7023e-102">Отстраняване на проблеми с спулера за печат</span><span class="sxs-lookup"><span data-stu-id="7023e-102">Print spooler issue is resolved</span></span>

<span data-ttu-id="7023e-103">Ако вашето устройство е било актуализирано с Windows 10  **OS компилация 19041,329**, е възможно да сте забелязали проблем, при който някои принтери не могат да се отпечатат.</span><span class="sxs-lookup"><span data-stu-id="7023e-103">If your device was updated with Windows 10  **OS Build 19041.329**, you might have observed an issue where certain printers fail to print.</span></span> <span data-ttu-id="7023e-104">Спулерът за печат може да хвърли съобщение за грешка или да затвори неочаквано при опит за печат, а изходните резултати да не се предоставят от повредения принтер.</span><span class="sxs-lookup"><span data-stu-id="7023e-104">The print spooler might throw an error or close unexpectedly when attempting to print, and no output comes from the affected printer.</span></span> <span data-ttu-id="7023e-105">Този проблем е решен в ос компилация  **19041,331**, [KB4567523](https://support.microsoft.com/help/4567523/windows-10-update-kb4567523).</span><span class="sxs-lookup"><span data-stu-id="7023e-105">This issue is resolved in OS Build  **19041.331**, [KB4567523](https://support.microsoft.com/help/4567523/windows-10-update-kb4567523).</span></span>  

<span data-ttu-id="7023e-106">**Текущо проучване**</span><span class="sxs-lookup"><span data-stu-id="7023e-106">**Ongoing investigation**</span></span>

<span data-ttu-id="7023e-107">Файлът за услуга на подсистемата за системен доставчик на LSASS (**Isass.exe**) може да е неуспешно на някои устройства със съобщение за грешка "критична системен процес, C:\WINDOWS\system32\Isass.exe, неуспешно с код на състояние c0000008.</span><span class="sxs-lookup"><span data-stu-id="7023e-107">The Local Security Authority Subsystem Service (LSASS) file (**Isass.exe**) might fail on some devices with the error message, "A critical system process, C:\WINDOWS\system32\Isass.exe, failed with status code c0000008.</span></span> <span data-ttu-id="7023e-108">Сега машината трябва да бъде рестартирана.</span><span class="sxs-lookup"><span data-stu-id="7023e-108">The machine must now be restarted".</span></span>  <span data-ttu-id="7023e-109">**Microsoft работи по резолюция и ще предостави актуализация в предстоящо издание.**</span><span class="sxs-lookup"><span data-stu-id="7023e-109">**Microsoft is working on a resolution and will provide an update in an upcoming release.**</span></span>

<span data-ttu-id="7023e-110">За повече информация вижте  [Windows 10 версия 2004 известни проблеми](https://docs.microsoft.com/windows/release-information/status-windows-10-2004#442msgdesc).</span><span class="sxs-lookup"><span data-stu-id="7023e-110">For more information, please check out  [Windows 10 Version 2004 known issues](https://docs.microsoft.com/windows/release-information/status-windows-10-2004#442msgdesc).</span></span>