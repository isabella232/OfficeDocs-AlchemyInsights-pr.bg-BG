---
title: Изпълнение на диагностика на паметта на Windows в Windows 10
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9002959"
- "5661"
ms.openlocfilehash: 3fedc52d02f1f70743429d0313eda0361306c3f3
ms.sourcegitcommit: 18b080c2a5d741af01ec589158effc35ea7cf449
ms.translationtype: MT
ms.contentlocale: bg-BG
ms.lasthandoff: 05/19/2020
ms.locfileid: "44357279"
---
# <a name="run-windows-memory-diagnostics-in-windows-10"></a><span data-ttu-id="01e6b-102">Изпълнение на диагностика на паметта на Windows в Windows 10</span><span class="sxs-lookup"><span data-stu-id="01e6b-102">Run Windows Memory Diagnostics in Windows 10</span></span>

<span data-ttu-id="01e6b-103">Ако Windows и приложенията на компютъра ви се сриват, замръзват или действат нестабилно, може да имате проблем с паметта на компютъра (RAM).</span><span class="sxs-lookup"><span data-stu-id="01e6b-103">If Windows and apps on your PC are crashing, freezing, or acting in an unstable manner, you may have a problem with the PC’s memory (RAM).</span></span> <span data-ttu-id="01e6b-104">Можете да стартирате диагностиката на паметта на Windows, за да проверите за проблеми с RAM паметта на компютъра.</span><span class="sxs-lookup"><span data-stu-id="01e6b-104">You can run the Windows Memory Diagnostic to check for problems with the PC’s RAM.</span></span>

<span data-ttu-id="01e6b-105">В полето за търсене на лентата на задачите въведете **диагностика на паметта**, след което изберете Диагностика на паметта на **Windows**.</span><span class="sxs-lookup"><span data-stu-id="01e6b-105">In the search box on your taskbar, type **memory diagnostic**, and then select **Windows Memory Diagnostic**.</span></span> 

<span data-ttu-id="01e6b-106">За да стартирате диагностиката, компютърът трябва да се рестартира.</span><span class="sxs-lookup"><span data-stu-id="01e6b-106">To run the diagnostic, the PC needs to restart.</span></span> <span data-ttu-id="01e6b-107">Имате възможност да рестартирате незабавно (моля, запишете работата си и затворете първо отворените документи и имейли) или насрочвайте диагностиката да се стартира автоматично при следващото рестартиране на компютъра:</span><span class="sxs-lookup"><span data-stu-id="01e6b-107">You have the option to restart immediately (please save your work and close open documents and e-mails first), or schedule the diagnostic to run automatically the next time the PC restarts:</span></span>

![Диагностика на паметта в Windows](media/windows-memory-diagnostic.png)

<span data-ttu-id="01e6b-109">Когато компютърът се рестартира, **инструментът за диагностика на паметта** на Windows ще се стартира автоматично.</span><span class="sxs-lookup"><span data-stu-id="01e6b-109">When the PC restarts, the **Windows Memory Diagnostics Tool** will run automatically.</span></span> <span data-ttu-id="01e6b-110">Състоянието и напредъкът ще се показват при изпълнение на диагностиката и имате възможност да отмените диагностиката чрез натискане на **клавиша ESC** на клавиатурата.</span><span class="sxs-lookup"><span data-stu-id="01e6b-110">Status and progress will be displayed as the diagnostics run, and you have the option of cancelling the diagnostics by hitting the **ESC** key on your keyboard.</span></span>

<span data-ttu-id="01e6b-111">Когато диагностиката завърши, Windows ще започне нормално.</span><span class="sxs-lookup"><span data-stu-id="01e6b-111">When the diagnostics are complete, Windows will start normally.</span></span>
<span data-ttu-id="01e6b-112">Веднага след рестарт, когато се появи работния плот, ще се появи известие (до иконата на **работния център** в лентата на задачите), за да се покаже дали са открити грешки в паметта.</span><span class="sxs-lookup"><span data-stu-id="01e6b-112">Immediately after restart, when the Desktop appears, a notification will appear (next to the **Action Center** icon on the taskbar), to indicate whether any memory errors were found.</span></span> <span data-ttu-id="01e6b-113">Например:</span><span class="sxs-lookup"><span data-stu-id="01e6b-113">For example:</span></span>

<span data-ttu-id="01e6b-114">Ето и иконата на работния център:</span><span class="sxs-lookup"><span data-stu-id="01e6b-114">Here's the Action Center icon:</span></span> ![Икона на работния център](media/action-center-icon.png) 

<span data-ttu-id="01e6b-116">И примерно известие:</span><span class="sxs-lookup"><span data-stu-id="01e6b-116">And a sample notification:</span></span> ![Няма грешки в паметта](media/no-memory-errors.png)

<span data-ttu-id="01e6b-118">Ако сте пропуснали известието, можете да изберете иконата на **работния център** в лентата на задачите, за да се покаже **работния център** и да видите списък с известия, който може да се превърта.</span><span class="sxs-lookup"><span data-stu-id="01e6b-118">If you missed the notification, you can select the **Action Center** icon  on the taskbar to display the **Action Center** and see a scrollable list of notifications.</span></span>

<span data-ttu-id="01e6b-119">За да прегледате подробна информация, въведете **събитие** в полето за търсене на лентата на задачите, след което изберете **Програма за преглед на събития**.</span><span class="sxs-lookup"><span data-stu-id="01e6b-119">To review detailed information, type **event** into the search box on your taskbar, and then select **Event Viewer**.</span></span> <span data-ttu-id="01e6b-120">В панела **на прозореца за преглед**на събития надясно отидете до **Регистрационните > system на Windows**.</span><span class="sxs-lookup"><span data-stu-id="01e6b-120">In the **Event Viewer**’s left-hand pane, navigate to **Windows Logs > System**.</span></span> <span data-ttu-id="01e6b-121">В десния екран сканирайте списъка, докато преглеждате колоната **Източник,** докато видите събития с Източник стойност **MemoryDiagnostics-Results**.</span><span class="sxs-lookup"><span data-stu-id="01e6b-121">In the right-hand pane, scan down the list while looking at the **Source** column, until you see events with Source value **MemoryDiagnostics-Results**.</span></span> <span data-ttu-id="01e6b-122">Маркирайте всяко такова събитие и вижте информацията за резултата в полето под раздела **Общи** под списъка.</span><span class="sxs-lookup"><span data-stu-id="01e6b-122">Highlight each such event and see the result information in the box under the **General** tab below the list.</span></span>
