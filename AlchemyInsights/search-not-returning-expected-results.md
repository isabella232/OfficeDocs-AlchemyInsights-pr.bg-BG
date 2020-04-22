---
title: 1491-Търсене-не-връщащи се очаквани-резултати
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
ms.openlocfilehash: d0707af19b0299f7257a10a20ab38f47860308fb
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: bg-BG
ms.lasthandoff: 04/22/2020
ms.locfileid: "43709216"
---
# <a name="content-search-not-returning-expected-results"></a><span data-ttu-id="b2ad7-102">Търсене на съдържание, което не връща очакванирезултати</span><span class="sxs-lookup"><span data-stu-id="b2ad7-102">Content Search not returning expected results</span></span>

<span data-ttu-id="b2ad7-103">Когато изпълнявате търсения за съдържание от центъра за сигурност на Microsoft 365 & Съответствието, може да получите неочаквани резултати от търсенето.</span><span class="sxs-lookup"><span data-stu-id="b2ad7-103">When running Content Searches from the Microsoft 365 security & Compliance Center, you may receive unexpected search results.</span></span> <span data-ttu-id="b2ad7-104">Обмислете следните неща, които могат да повлияят на резултатите от търсенето Ви:</span><span class="sxs-lookup"><span data-stu-id="b2ad7-104">Consider the following things that can affect your search results:</span></span>

- <span data-ttu-id="b2ad7-105">**Местоположения на съдържание и условия за търсене:** Уверете се, че сте избрали правилните местоположения на съдържание и условия за търсене.</span><span class="sxs-lookup"><span data-stu-id="b2ad7-105">**Content locations and search conditions**: Make sure you have selected the proper content locations and search conditions.</span></span> <span data-ttu-id="b2ad7-106">Ако сте направили голямо търсене (с много местоположения), помислете дали да го разделите на няколко търсения.</span><span class="sxs-lookup"><span data-stu-id="b2ad7-106">If you ran a large search (with many locations), consider splitting it into multiple searches.</span></span>

- <span data-ttu-id="b2ad7-107">**Частично индексирани елементи:** [Частично индексираните елементи](https://docs.microsoft.com/office365/securitycompliance/partially-indexed-items-in-content-search) от пощенски кутии са включени в оценката на резултатите от търсенето.</span><span class="sxs-lookup"><span data-stu-id="b2ad7-107">**Partially indexed items**:  [Partially indexed items](https://docs.microsoft.com/office365/securitycompliance/partially-indexed-items-in-content-search) from mailboxes are included in the estimated search results.</span></span> <span data-ttu-id="b2ad7-108">Обаче частично индексираелементи от сайтове в SharePoint и OneDrive не са включени в оценката за търсене.</span><span class="sxs-lookup"><span data-stu-id="b2ad7-108">However, partially indexed items from sites in SharePoint and OneDrive aren't included in the search estimate.</span></span>

- <span data-ttu-id="b2ad7-109">**Грешки при търсене:** Когато търсите голям брой пощенски кутии (над 100 000 пощенски кутии), можете да получите търсене грешки, с кодове за грешка като CS008-009 и CS012-002).</span><span class="sxs-lookup"><span data-stu-id="b2ad7-109">**Search failures**: When searching a large number of mailboxes (over 100,000 mailboxes), you may get search errors, with error codes such as CS008-009 and CS012-002).</span></span> <span data-ttu-id="b2ad7-110">В този случай опитайте отново търсенето само за неуспешните местоположения на съдържание.</span><span class="sxs-lookup"><span data-stu-id="b2ad7-110">In this case, retry the search only for the failed content locations.</span></span> <span data-ttu-id="b2ad7-111">Вижте [тази статия](https://docs.microsoft.com/office365/securitycompliance/retry-failed-content-search) за повече информация.</span><span class="sxs-lookup"><span data-stu-id="b2ad7-111">See  [this article](https://docs.microsoft.com/office365/securitycompliance/retry-failed-content-search) for more information.</span></span>
