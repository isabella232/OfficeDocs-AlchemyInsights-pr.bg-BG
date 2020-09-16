---
title: Изпълнение на Windows за диагностика на паметта в Windows 10
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9002959"
- "5661"
ms.openlocfilehash: f2b8306d0cd604b144b82275243c5a84580bc609
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: bg-BG
ms.lasthandoff: 09/14/2020
ms.locfileid: "47720779"
---
# <a name="run-windows-memory-diagnostics-in-windows-10"></a><span data-ttu-id="6efb0-102">Изпълнение на Windows за диагностика на паметта в Windows 10</span><span class="sxs-lookup"><span data-stu-id="6efb0-102">Run Windows Memory Diagnostics in Windows 10</span></span>

<span data-ttu-id="6efb0-103">Ако Windows и приложенията на КОМПЮТЪРА ви се сриват, замразяват или действат по нестабилен начин, е възможно да имате проблем с паметта на КОМПЮТЪРА (RAM).</span><span class="sxs-lookup"><span data-stu-id="6efb0-103">If Windows and apps on your PC are crashing, freezing, or acting in an unstable manner, you may have a problem with the PC’s memory (RAM).</span></span> <span data-ttu-id="6efb0-104">Можете да изпълните диагностичната памет на Windows, за да проверите за проблеми с RAM на КОМПЮТЪРА.</span><span class="sxs-lookup"><span data-stu-id="6efb0-104">You can run the Windows Memory Diagnostic to check for problems with the PC’s RAM.</span></span>

<span data-ttu-id="6efb0-105">В полето за търсене на лентата на задачите въведете **диагностична памет**и след това изберете **Windows за диагностика на паметта**.</span><span class="sxs-lookup"><span data-stu-id="6efb0-105">In the search box on your taskbar, type **memory diagnostic**, and then select **Windows Memory Diagnostic**.</span></span> 

<span data-ttu-id="6efb0-106">За да изпълните диагностичния тест, КОМПЮТЪРЪТ трябва да се рестартира.</span><span class="sxs-lookup"><span data-stu-id="6efb0-106">To run the diagnostic, the PC needs to restart.</span></span> <span data-ttu-id="6efb0-107">Разполагате с опцията за незабавно рестартиране (Моля, запазете работата си и затворете отворените документи и имейлите си първо) или планирайте диагностичната проверка да се изпълнява автоматично при следващото рестартиране на КОМПЮТЪРА:</span><span class="sxs-lookup"><span data-stu-id="6efb0-107">You have the option to restart immediately (please save your work and close open documents and e-mails first), or schedule the diagnostic to run automatically the next time the PC restarts:</span></span>

![Диагностика на паметта в Windows](media/windows-memory-diagnostic.png)

<span data-ttu-id="6efb0-109">Когато КОМПЮТЪРЪТ се рестартира, **Инструментът за диагностика на паметта на Windows** ще се стартира автоматично.</span><span class="sxs-lookup"><span data-stu-id="6efb0-109">When the PC restarts, the **Windows Memory Diagnostics Tool** will run automatically.</span></span> <span data-ttu-id="6efb0-110">Състоянието и ходът ще бъдат показвани като план за диагностика и имате възможност да анулирате диагностиката, като натиснете клавиша **ESC** на клавиатурата.</span><span class="sxs-lookup"><span data-stu-id="6efb0-110">Status and progress will be displayed as the diagnostics run, and you have the option of cancelling the diagnostics by hitting the **ESC** key on your keyboard.</span></span>

<span data-ttu-id="6efb0-111">Когато диагностиката завърши, прозорците ще започнат нормално.</span><span class="sxs-lookup"><span data-stu-id="6efb0-111">When the diagnostics are complete, Windows will start normally.</span></span>
<span data-ttu-id="6efb0-112">Веднага след рестартиране, когато се покаже работният плот, ще се появи известие (до иконата на **работния център** в лентата на задачите), за да укажете дали са открити грешки в паметта.</span><span class="sxs-lookup"><span data-stu-id="6efb0-112">Immediately after restart, when the Desktop appears, a notification will appear (next to the **Action Center** icon on the taskbar), to indicate whether any memory errors were found.</span></span> <span data-ttu-id="6efb0-113">Например:</span><span class="sxs-lookup"><span data-stu-id="6efb0-113">For example:</span></span>

<span data-ttu-id="6efb0-114">Ето иконата на работния център:</span><span class="sxs-lookup"><span data-stu-id="6efb0-114">Here's the Action Center icon:</span></span> ![Икона на работния център](media/action-center-icon.png) 

<span data-ttu-id="6efb0-116">И примерно уведомление:</span><span class="sxs-lookup"><span data-stu-id="6efb0-116">And a sample notification:</span></span> ![Без грешки в паметта](media/no-memory-errors.png)

<span data-ttu-id="6efb0-118">Ако сте пропуснали известието, можете да изберете иконата на **работния център** в лентата на задачите, за да покажете работния **център** и да видите превъртащ се списък с уведомления.</span><span class="sxs-lookup"><span data-stu-id="6efb0-118">If you missed the notification, you can select the **Action Center** icon  on the taskbar to display the **Action Center** and see a scrollable list of notifications.</span></span>

<span data-ttu-id="6efb0-119">За да прегледате подробна информация, въведете **Event** в полето за търсене на лентата на задачите и след това изберете **визуализатор на събития**.</span><span class="sxs-lookup"><span data-stu-id="6efb0-119">To review detailed information, type **event** into the search box on your taskbar, and then select **Event Viewer**.</span></span> <span data-ttu-id="6efb0-120">В левия екран на **визуализатора на събития**се придвижете до **регистрите на Windows > System**.</span><span class="sxs-lookup"><span data-stu-id="6efb0-120">In the **Event Viewer**’s left-hand pane, navigate to **Windows Logs > System**.</span></span> <span data-ttu-id="6efb0-121">В дясната част на екрана, прегледайте списъка, докато гледате колоната **източник** , докато не видите събития с изходна стойност на **MemoryDiagnostics – резултати**.</span><span class="sxs-lookup"><span data-stu-id="6efb0-121">In the right-hand pane, scan down the list while looking at the **Source** column, until you see events with Source value **MemoryDiagnostics-Results**.</span></span> <span data-ttu-id="6efb0-122">Осветяване на всяко такова събитие и показване на информацията за резултат в полето под раздела **Общи** под списъка.</span><span class="sxs-lookup"><span data-stu-id="6efb0-122">Highlight each such event and see the result information in the box under the **General** tab below the list.</span></span>
