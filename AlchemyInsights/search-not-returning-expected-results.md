---
title: 1491-търсене-не връщащи се очаквани-резултати
ms.author: markjjo
author: markjjo
manager: lauraw
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "1491"
- "3200003"
ms.assetid: ''
ms.openlocfilehash: 57421d459ef03049d6f931db659a5f9b253f5002
ms.sourcegitcommit: bc7d6f4f3c9f7060d073f5130e1ec856e248d020
ms.translationtype: MT
ms.contentlocale: bg-BG
ms.lasthandoff: 06/02/2020
ms.locfileid: "44510561"
---
# <a name="content-search-not-returning-expected-results"></a><span data-ttu-id="e1594-102">Търсенето на съдържание не връща очакваните резултати</span><span class="sxs-lookup"><span data-stu-id="e1594-102">Content Search not returning expected results</span></span>

<span data-ttu-id="e1594-103">Когато изпълнявате търсене на съдържание от центъра за съответствие на Microsoft 365 & за защита, можете да получите неочаквани резултати от търсенето.</span><span class="sxs-lookup"><span data-stu-id="e1594-103">When running Content Searches from the Microsoft 365 security & Compliance Center, you may receive unexpected search results.</span></span> <span data-ttu-id="e1594-104">Обмислете следните неща, които могат да повлияят на резултатите от търсенето:</span><span class="sxs-lookup"><span data-stu-id="e1594-104">Consider the following things that can affect your search results:</span></span>

- <span data-ttu-id="e1594-105">**Местоположения на съдържанието и условия за търсене:** Уверете се, че сте избрали правилните местоположения на съдържанието и условията за търсене.</span><span class="sxs-lookup"><span data-stu-id="e1594-105">**Content locations and search conditions**: Make sure you have selected the proper content locations and search conditions.</span></span> <span data-ttu-id="e1594-106">Ако сте извършили голямо търсене (с много местоположения), помислете дали да го разделите на няколко търсения.</span><span class="sxs-lookup"><span data-stu-id="e1594-106">If you ran a large search (with many locations), consider splitting it into multiple searches.</span></span>

- <span data-ttu-id="e1594-107">**Частично индексирани елементи:** [Частично индексирани елементи](https://docs.microsoft.com/microsoft-365/compliance/partially-indexed-items-in-content-search) от пощенски кутии са включени в очакваните резултати от търсенето.</span><span class="sxs-lookup"><span data-stu-id="e1594-107">**Partially indexed items**:  [Partially indexed items](https://docs.microsoft.com/microsoft-365/compliance/partially-indexed-items-in-content-search) from mailboxes are included in the estimated search results.</span></span> <span data-ttu-id="e1594-108">Обаче частично индексирани елементи от сайтове в SharePoint и OneDrive не са включени в оценката на търсенето.</span><span class="sxs-lookup"><span data-stu-id="e1594-108">However, partially indexed items from sites in SharePoint and OneDrive aren't included in the search estimate.</span></span>

- <span data-ttu-id="e1594-109">**Търсене грешки:** При търсене на голям брой пощенски кутии (над 100 000 пощенски кутии), можете да получите грешки при търсене, с кодове за грешка като CS008-009 и CS012-002).</span><span class="sxs-lookup"><span data-stu-id="e1594-109">**Search failures**: When searching a large number of mailboxes (over 100,000 mailboxes), you may get search errors, with error codes such as CS008-009 and CS012-002).</span></span> <span data-ttu-id="e1594-110">В този случай опитайте отново само за неуспешно съдържание местоположения.</span><span class="sxs-lookup"><span data-stu-id="e1594-110">In this case, retry the search only for the failed content locations.</span></span> <span data-ttu-id="e1594-111">Вижте [тази статия](https://docs.microsoft.com/microsoft-365/compliance/retry-failed-content-search) за повече информация.</span><span class="sxs-lookup"><span data-stu-id="e1594-111">See  [this article](https://docs.microsoft.com/microsoft-365/compliance/retry-failed-content-search) for more information.</span></span>
