---
title: 'Грешка: Правилата на този компютър не съвпадат'
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "3518"
- "1800021"
ms.openlocfilehash: c0982da82826d1644f437b19e0d343a59d7ac473
ms.sourcegitcommit: e09af4285c6b81ca0a5320fdb811713ac25748c3
ms.translationtype: MT
ms.contentlocale: bg-BG
ms.lasthandoff: 06/09/2020
ms.locfileid: "44664235"
---
# <a name="error-the-rules-on-this-computer-do-not-match"></a><span data-ttu-id="78123-102">Грешка: Правилата на този компютър не съвпадат</span><span class="sxs-lookup"><span data-stu-id="78123-102">Error: The rules on this computer do not match</span></span>

<span data-ttu-id="78123-103">За да видите състоянието на този известен проблем, вижте [правилата на този компютър не съвпадат с правилата на Microsoft Exchange](https://support.office.com/article/d032e037-b224-429e-b325-633afde9b5f0)</span><span class="sxs-lookup"><span data-stu-id="78123-103">To see updated status of this known issue, see [The rules on this computer do not match the rules on Microsoft Exchange](https://support.office.com/article/d032e037-b224-429e-b325-633afde9b5f0)</span></span>

<span data-ttu-id="78123-104">Екипът на Outlook е внедрила корекция в компилация 12928.10000.</span><span class="sxs-lookup"><span data-stu-id="78123-104">The Outlook Team has implemented a fix in Build 12928.10000.</span></span> <span data-ttu-id="78123-105">Корекцията вече е в Insider бързо и ще отиде в месечен канал в края на юни 2020.</span><span class="sxs-lookup"><span data-stu-id="78123-105">The fix is already at Insider Fast and will go to Monthly Channel in late June 2020.</span></span> <span data-ttu-id="78123-106">След като имате фиксиран изграждане може да получите подкана "Кои правила искате да запазите" за последен път.</span><span class="sxs-lookup"><span data-stu-id="78123-106">Once you have the fixed build you may get the prompt "Which rules do you want to keep" one last time.</span></span> <span data-ttu-id="78123-107">Изберете сървър при подкана и след това се върнете в Outlook и отново разрешите всички правила, които са забранени.</span><span class="sxs-lookup"><span data-stu-id="78123-107">Choose Server when prompted and then go back in Outlook and re-enable any rules that were disabled.</span></span>

<span data-ttu-id="78123-108">Докато корекцията е налична, използвайте следния заобиколно решение:</span><span class="sxs-lookup"><span data-stu-id="78123-108">Until the fix is available please use the following workaround:</span></span>

<span data-ttu-id="78123-109">**Решение:** в последните отчети проблемът е възникнал за тези, които са създали само правила за клиент в outlook десктоп.</span><span class="sxs-lookup"><span data-stu-id="78123-109">**Workaround**: In recent reports, the issue has occurred for those that have only created client rules in Outlook desktop.</span></span> <span data-ttu-id="78123-110">Ако продължавате да се сблъскате с проблема, помислете за изтриване на правилата и след това създайте и редактирате правила само в OWA (Outlook Web App) докато проблемът е разрешен.</span><span class="sxs-lookup"><span data-stu-id="78123-110">If you continue to run into the problem, consider deleting the rules and then create and edit rules only in OWA (Outlook Web App) until the issue is resolved.</span></span>

<span data-ttu-id="78123-111">Ако не можете да изтриете ръчно правилата, можете да стартирате команда от Outlook, когато стартирате Outlook, като изпълните Outlook.exe /cleanrules.</span><span class="sxs-lookup"><span data-stu-id="78123-111">If you cannot delete the rules manually you can run an Outlook command when you start Outlook by running Outlook.exe /cleanrules.</span></span> <span data-ttu-id="78123-112">Това ще изтрие правилата на клиента и сървъра.</span><span class="sxs-lookup"><span data-stu-id="78123-112">This will delete both the client and server rules.</span></span> <span data-ttu-id="78123-113">Тя ще изтрие всички правила за всички акаунти в профила на Outlook.</span><span class="sxs-lookup"><span data-stu-id="78123-113">It will delete all of the rules for all of the accounts in the Outlook Profile.</span></span> <span data-ttu-id="78123-114">Тази команда е допълнително документирана в статията с превключватели на командния ред.</span><span class="sxs-lookup"><span data-stu-id="78123-114">This command is further documented in the Command-line switches article.</span></span>

