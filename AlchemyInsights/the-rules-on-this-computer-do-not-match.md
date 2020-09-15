---
title: 'Грешка: правилата на този компютър не съвпадат'
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "3518"
- "1800021"
ms.openlocfilehash: c2feb6da651d8b3eb7af6a057335b28d26f9e7f6
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: bg-BG
ms.lasthandoff: 09/14/2020
ms.locfileid: "47690952"
---
# <a name="error-the-rules-on-this-computer-do-not-match"></a><span data-ttu-id="a959a-102">Грешка: правилата на този компютър не съвпадат</span><span class="sxs-lookup"><span data-stu-id="a959a-102">Error: The rules on this computer do not match</span></span>

<span data-ttu-id="a959a-103">За да видите актуализираното състояние на този известен проблем, вижте [правилата на този компютър не отговарят на правилата за Microsoft Exchange](https://support.office.com/article/d032e037-b224-429e-b325-633afde9b5f0)</span><span class="sxs-lookup"><span data-stu-id="a959a-103">To see updated status of this known issue, see [The rules on this computer do not match the rules on Microsoft Exchange](https://support.office.com/article/d032e037-b224-429e-b325-633afde9b5f0)</span></span>

<span data-ttu-id="a959a-104">Екипът на Outlook е реализирал корекция в компилация 12928,10000.</span><span class="sxs-lookup"><span data-stu-id="a959a-104">The Outlook Team has implemented a fix in Build 12928.10000.</span></span> <span data-ttu-id="a959a-105">Корекцията вече е в Insider Fast и ще премине към месечен канал в края на юни 2020.</span><span class="sxs-lookup"><span data-stu-id="a959a-105">The fix is already at Insider Fast and will go to Monthly Channel in late June 2020.</span></span> <span data-ttu-id="a959a-106">След като приключите с фиксираната компилация, може да получите подканата "кои правила искате да запазите" за последен път.</span><span class="sxs-lookup"><span data-stu-id="a959a-106">Once you have the fixed build you may get the prompt "Which rules do you want to keep" one last time.</span></span> <span data-ttu-id="a959a-107">Изберете сървър, когато получите подкана, и след това се върнете в Outlook и разрешете отново правилата, които са забранени.</span><span class="sxs-lookup"><span data-stu-id="a959a-107">Choose Server when prompted and then go back in Outlook and re-enable any rules that were disabled.</span></span>

<span data-ttu-id="a959a-108">Докато корекцията е налична, моля, използвайте следното заобиколно решение:</span><span class="sxs-lookup"><span data-stu-id="a959a-108">Until the fix is available please use the following workaround:</span></span>

<span data-ttu-id="a959a-109">**Заобиколно решение**: в последните отчети проблемът е възникнал за тези, които имат само създадени клиентски правила в настолната версия на Outlook.</span><span class="sxs-lookup"><span data-stu-id="a959a-109">**Workaround**: In recent reports, the issue has occurred for those that have only created client rules in Outlook desktop.</span></span> <span data-ttu-id="a959a-110">Ако продължавате да се сблъскате с проблема, можете да изтриете правилата и след това да създадете и редактирате правила само в OWA (Outlook Web App), докато проблемът не бъде разрешен.</span><span class="sxs-lookup"><span data-stu-id="a959a-110">If you continue to run into the problem, consider deleting the rules and then create and edit rules only in OWA (Outlook Web App) until the issue is resolved.</span></span>

<span data-ttu-id="a959a-111">Ако не можете да изтриете ръчно правилата, можете да изпълните команда на Outlook, когато стартирате Outlook, като изпълните Outlook.exe/cleanrules.</span><span class="sxs-lookup"><span data-stu-id="a959a-111">If you cannot delete the rules manually you can run an Outlook command when you start Outlook by running Outlook.exe /cleanrules.</span></span> <span data-ttu-id="a959a-112">Това ще изтрие и правилата за клиента и сървъра.</span><span class="sxs-lookup"><span data-stu-id="a959a-112">This will delete both the client and server rules.</span></span> <span data-ttu-id="a959a-113">Ще изтрие всички правила за всички акаунти в профила на Outlook.</span><span class="sxs-lookup"><span data-stu-id="a959a-113">It will delete all of the rules for all of the accounts in the Outlook Profile.</span></span> <span data-ttu-id="a959a-114">Тази команда е допълнително документирана в статията ключове за командния ред.</span><span class="sxs-lookup"><span data-stu-id="a959a-114">This command is further documented in the Command-line switches article.</span></span>

