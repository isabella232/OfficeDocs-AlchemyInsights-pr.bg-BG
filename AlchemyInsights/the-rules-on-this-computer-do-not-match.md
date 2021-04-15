---
title: 'Грешка: Правилата на този компютър не съвпадат'
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "3518"
- "1800021"
ms.openlocfilehash: c46eb856baafbef9bc3b7fa34a0258ef16923fb8
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: bg-BG
ms.lasthandoff: 04/15/2021
ms.locfileid: "51782941"
---
# <a name="error-the-rules-on-this-computer-do-not-match"></a><span data-ttu-id="c1db7-102">Грешка: Правилата на този компютър не съвпадат</span><span class="sxs-lookup"><span data-stu-id="c1db7-102">Error: The rules on this computer do not match</span></span>

<span data-ttu-id="c1db7-103">За да видите актуализираното състояние на този известен [проблем,](https://support.office.com/article/d032e037-b224-429e-b325-633afde9b5f0) вижте Правилата на този компютър не съответстват на правилата в Microsoft Exchange</span><span class="sxs-lookup"><span data-stu-id="c1db7-103">To see updated status of this known issue, see [The rules on this computer do not match the rules on Microsoft Exchange](https://support.office.com/article/d032e037-b224-429e-b325-633afde9b5f0)</span></span>

<span data-ttu-id="c1db7-104">Екипът на Outlook е внедрил корекция в компилация 12928.10000.</span><span class="sxs-lookup"><span data-stu-id="c1db7-104">The Outlook Team has implemented a fix in Build 12928.10000.</span></span> <span data-ttu-id="c1db7-105">Корекцията вече е в Insider Fast и ще отиде на Месечен канал в края на юни 2020 г.</span><span class="sxs-lookup"><span data-stu-id="c1db7-105">The fix is already at Insider Fast and will go to Monthly Channel in late June 2020.</span></span> <span data-ttu-id="c1db7-106">След като имате фиксираната компилация, може да получите подканата "Кои правила искате да запазите" за последен път.</span><span class="sxs-lookup"><span data-stu-id="c1db7-106">Once you have the fixed build you may get the prompt "Which rules do you want to keep" one last time.</span></span> <span data-ttu-id="c1db7-107">Изберете Сървър, когато получите подкана, и след това се върнете в Outlook и разрешете отново всички забранени правила.</span><span class="sxs-lookup"><span data-stu-id="c1db7-107">Choose Server when prompted and then go back in Outlook and re-enable any rules that were disabled.</span></span>

<span data-ttu-id="c1db7-108">Докато корекцията не бъде налична, използвайте следното заобиколно решение:</span><span class="sxs-lookup"><span data-stu-id="c1db7-108">Until the fix is available please use the following workaround:</span></span>

<span data-ttu-id="c1db7-109">**Заобиколно** решение: В последните отчети възникна проблем за тези, които са създали само клиентски правила в настолната версия на Outlook.</span><span class="sxs-lookup"><span data-stu-id="c1db7-109">**Workaround**: In recent reports, the issue has occurred for those that have only created client rules in Outlook desktop.</span></span> <span data-ttu-id="c1db7-110">Ако продължите да се натучавате на проблема, помислете за изтриване на правилата и след това създайте и редактирайте правила само в OWA (Outlook Web App), докато проблемът не бъде решен.</span><span class="sxs-lookup"><span data-stu-id="c1db7-110">If you continue to run into the problem, consider deleting the rules and then create and edit rules only in OWA (Outlook Web App) until the issue is resolved.</span></span>

<span data-ttu-id="c1db7-111">Ако не можете да изтриете правилата ръчно, можете да изпълните команда на Outlook, когато стартирате Outlook, като изпълните Outlook.exe /cleanrules.</span><span class="sxs-lookup"><span data-stu-id="c1db7-111">If you cannot delete the rules manually you can run an Outlook command when you start Outlook by running Outlook.exe /cleanrules.</span></span> <span data-ttu-id="c1db7-112">Това ще изтрие както правилата за клиента, така и сървъра.</span><span class="sxs-lookup"><span data-stu-id="c1db7-112">This will delete both the client and server rules.</span></span> <span data-ttu-id="c1db7-113">Той ще изтрие всички правила за всички акаунти в профила на Outlook.</span><span class="sxs-lookup"><span data-stu-id="c1db7-113">It will delete all of the rules for all of the accounts in the Outlook Profile.</span></span> <span data-ttu-id="c1db7-114">Тази команда е документирана допълнително в статията "Превключватели на команден ред".</span><span class="sxs-lookup"><span data-stu-id="c1db7-114">This command is further documented in the Command-line switches article.</span></span>

