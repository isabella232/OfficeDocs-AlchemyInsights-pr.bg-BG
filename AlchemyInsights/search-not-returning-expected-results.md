---
title: 1491-Search-not-returning-Expected-results
ms.author: markjjo
author: markjjo
manager: lauraw
ms.date: ''
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "1491"
- "3200003"
ms.assetid: ''
ms.openlocfilehash: d25c1ef2e0e746432472a436cb11d25b5db5596c
ms.sourcegitcommit: 5fb7a4b28859690020efdea630d03e70cc0e6334
ms.translationtype: MT
ms.contentlocale: bg-BG
ms.lasthandoff: 06/28/2019
ms.locfileid: "35355866"
---
# <a name="content-search-not-returning-expected-results"></a><span data-ttu-id="bda00-102">Съдържание за търсене не връщат очакваните резултати</span><span class="sxs-lookup"><span data-stu-id="bda00-102">Content Search not returning expected results</span></span>

<span data-ttu-id="bda00-103">Когато изпълнява съдържание търсения от Office 365 сигурност & съответствие център, можете да получите неочаквани резултати.</span><span class="sxs-lookup"><span data-stu-id="bda00-103">When running Content Searches from the Office 365 Security & Compliance Center, you may receive unexpected search results.</span></span> <span data-ttu-id="bda00-104">Помислете за следните неща, които може да повлияе резултатите от вашето търсене:</span><span class="sxs-lookup"><span data-stu-id="bda00-104">Consider the following things that can affect your search results:</span></span>

- <span data-ttu-id="bda00-105">**Съдържание места и условия за търсене**: Уверете се, че сте избрали правилното съдържание места и условия за търсене.</span><span class="sxs-lookup"><span data-stu-id="bda00-105">**Content locations and search conditions**: Make sure you have selected the proper content locations and search conditions.</span></span> <span data-ttu-id="bda00-106">Ако сте стартирали голям търсене (с много места), помислете за това разделяне на няколко търсения.</span><span class="sxs-lookup"><span data-stu-id="bda00-106">If you ran a large search (with many locations), consider splitting it into multiple searches.</span></span>

- <span data-ttu-id="bda00-107">**Частично индексирани елементи**: [частично индексирани елементи](https://docs.microsoft.com/office365/securitycompliance/partially-indexed-items-in-content-search) от пощенските кутии са включени в очакваните резултати.</span><span class="sxs-lookup"><span data-stu-id="bda00-107">**Partially indexed items**:  [Partially indexed items](https://docs.microsoft.com/office365/securitycompliance/partially-indexed-items-in-content-search) from mailboxes are included in the estimated search results.</span></span> <span data-ttu-id="bda00-108">Въпреки това частично индексирани елементи от сайтове на SharePoint и OneDrive не са включени в търсене прогноза.</span><span class="sxs-lookup"><span data-stu-id="bda00-108">However, partially indexed items from sites in SharePoint and OneDrive aren't included in the search estimate.</span></span>

- <span data-ttu-id="bda00-109">**Търсене повреди**: при търсене на голям брой пощенски кутии (над 100 000 кутии), може да получите търсене грешки, с кодове за грешка CS008-009 и CS012-002).</span><span class="sxs-lookup"><span data-stu-id="bda00-109">**Search failures**: When searching a large number of mailboxes (over 100,000 mailboxes), you may get search errors, with error codes such as CS008-009 and CS012-002).</span></span> <span data-ttu-id="bda00-110">В този случай опитайте отново търсене само за неуспешни местонахождения на съдържание.</span><span class="sxs-lookup"><span data-stu-id="bda00-110">In this case, retry the search only for the failed content locations.</span></span> <span data-ttu-id="bda00-111">Вижте [тази статия](https://docs.microsoft.com/office365/securitycompliance/retry-failed-content-search) за повече информация.</span><span class="sxs-lookup"><span data-stu-id="bda00-111">See  [this article](https://docs.microsoft.com/office365/securitycompliance/retry-failed-content-search) for more information.</span></span>
