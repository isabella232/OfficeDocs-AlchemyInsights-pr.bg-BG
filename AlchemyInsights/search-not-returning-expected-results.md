---
title: 1491-Search-not-Re-Re---Up-очаквани резултати
ms.author: markjjo
author: markjjo
manager: lauraw
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "1491"
- "3200003"
ms.assetid: ''
ms.openlocfilehash: 5c4452726c1dbe2232ee63e8a9ee4d089f5c76db
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: bg-BG
ms.lasthandoff: 09/14/2020
ms.locfileid: "47740463"
---
# <a name="content-search-not-returning-expected-results"></a><span data-ttu-id="3c48c-102">Търсенето на съдържание не връща очакваните резултати</span><span class="sxs-lookup"><span data-stu-id="3c48c-102">Content Search not returning expected results</span></span>

<span data-ttu-id="3c48c-103">При изпълнение на търсения на съдържание от центъра за съответствие на Microsoft 365 Security &, е възможно да получите неочаквани резултати от търсенето.</span><span class="sxs-lookup"><span data-stu-id="3c48c-103">When running Content Searches from the Microsoft 365 security & Compliance Center, you may receive unexpected search results.</span></span> <span data-ttu-id="3c48c-104">Обмислете следните неща, които могат да повлияят на резултатите от търсенето:</span><span class="sxs-lookup"><span data-stu-id="3c48c-104">Consider the following things that can affect your search results:</span></span>

- <span data-ttu-id="3c48c-105">**Местоположения на съдържание и условия за търсене**: Уверете се, че сте избрали правилните местоположения и условия за търсене на съдържание.</span><span class="sxs-lookup"><span data-stu-id="3c48c-105">**Content locations and search conditions**: Make sure you have selected the proper content locations and search conditions.</span></span> <span data-ttu-id="3c48c-106">Ако сте стартирали голямо търсене (с много местоположения), обмислете разделянето му на няколко търсения.</span><span class="sxs-lookup"><span data-stu-id="3c48c-106">If you ran a large search (with many locations), consider splitting it into multiple searches.</span></span>

- <span data-ttu-id="3c48c-107">**Частично индексирани елементи**:  [частично индексираните елементи](https://docs.microsoft.com/microsoft-365/compliance/partially-indexed-items-in-content-search) от пощенските кутии се включват в прогнозните резултати от търсенето.</span><span class="sxs-lookup"><span data-stu-id="3c48c-107">**Partially indexed items**:  [Partially indexed items](https://docs.microsoft.com/microsoft-365/compliance/partially-indexed-items-in-content-search) from mailboxes are included in the estimated search results.</span></span> <span data-ttu-id="3c48c-108">Обаче частично индексираните елементи от сайтове в SharePoint и OneDrive не се включват в прогнозната стойност на търсенето.</span><span class="sxs-lookup"><span data-stu-id="3c48c-108">However, partially indexed items from sites in SharePoint and OneDrive aren't included in the search estimate.</span></span>

- <span data-ttu-id="3c48c-109">**Неизправности при търсене**: когато се търсят голям брой пощенски кутии (над 100 000 пощенски кутии), може да получите грешки при търсенето с кодове на грешки, като например CS008-009 и CS012-002).</span><span class="sxs-lookup"><span data-stu-id="3c48c-109">**Search failures**: When searching a large number of mailboxes (over 100,000 mailboxes), you may get search errors, with error codes such as CS008-009 and CS012-002).</span></span> <span data-ttu-id="3c48c-110">В този случай Повторете търсенето само за местоположенията с неуспешно съдържание.</span><span class="sxs-lookup"><span data-stu-id="3c48c-110">In this case, retry the search only for the failed content locations.</span></span> <span data-ttu-id="3c48c-111">Вижте  [тази статия](https://docs.microsoft.com/microsoft-365/compliance/retry-failed-content-search) за повече информация.</span><span class="sxs-lookup"><span data-stu-id="3c48c-111">See  [this article](https://docs.microsoft.com/microsoft-365/compliance/retry-failed-content-search) for more information.</span></span>
