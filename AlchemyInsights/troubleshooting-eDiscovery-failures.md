---
title: 1490 – отстраняване на неизправности – откриването на електронни данни
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
- "1490"
- "3200003"
ms.assetid: ''
ms.openlocfilehash: ff28f96d64ec14980e9a47b630246b394faf4610
ms.sourcegitcommit: fbe6925797cab0b38172386f1b059dc122e452a4
ms.translationtype: MT
ms.contentlocale: bg-BG
ms.lasthandoff: 09/25/2020
ms.locfileid: "48277836"
---
# <a name="troubleshoot-content-search-errors"></a><span data-ttu-id="aed7f-102">Отстраняване на грешки при търсене на съдържание</span><span class="sxs-lookup"><span data-stu-id="aed7f-102">Troubleshoot Content Search errors</span></span>

<span data-ttu-id="aed7f-103">Изпитвате ли проблеми при търсене на съдържание или получавате неуспехи, когато експортирате резултати от търсенето?</span><span class="sxs-lookup"><span data-stu-id="aed7f-103">Are you experiencing problems with Content Search or getting failures when you export search results?</span></span>

<span data-ttu-id="aed7f-104">Например получавате ли следното, когато изпълнявате търсения?</span><span class="sxs-lookup"><span data-stu-id="aed7f-104">For example, are you receiving the following when running searches?</span></span>

- <span data-ttu-id="aed7f-105">CS008 или CS012 грешки</span><span class="sxs-lookup"><span data-stu-id="aed7f-105">CS008 or CS012 errors</span></span>

- <span data-ttu-id="aed7f-106">Грешки при изчакване на сървъра</span><span class="sxs-lookup"><span data-stu-id="aed7f-106">Server busy/timeout errors</span></span>

- <span data-ttu-id="aed7f-107">Възникна грешка в приложението</span><span class="sxs-lookup"><span data-stu-id="aed7f-107">Application error occurred</span></span>

<span data-ttu-id="aed7f-108">Или когато търсите или експортирате резултати от голям брой пощенски кутии (над 100 000 пощенски кутии), получавате ли грешки при експортиране?</span><span class="sxs-lookup"><span data-stu-id="aed7f-108">Or when searching or exporting results from a large number of mailboxes (over 100,000 mailboxes), are you getting export errors?</span></span>

<span data-ttu-id="aed7f-109">За тези типове грешки опитайте да повторите търсенето на местоположенията за съдържание, които са неуспешни.</span><span class="sxs-lookup"><span data-stu-id="aed7f-109">For these types of errors, retry the search for the content locations that have failed.</span></span> <span data-ttu-id="aed7f-110">Вижте  [тази статия](https://docs.microsoft.com/microsoft-365/compliance/retry-failed-content-search) за повече информация.</span><span class="sxs-lookup"><span data-stu-id="aed7f-110">See  [this article](https://docs.microsoft.com/microsoft-365/compliance/retry-failed-content-search) for more information.</span></span>

<span data-ttu-id="aed7f-111">Ако експортирате повече от 100K пощенски кутии, ще трябва да използвате следния PowerShell, за да изтеглите резултатите от износа:  [експортиране на резултати от повече от 100k пощенски кутии](https://docs.microsoft.com/microsoft-365/compliance/export-search-results?view=o365-worldwide%23exporting-results-from-more-than-100000-mailboxes).</span><span class="sxs-lookup"><span data-stu-id="aed7f-111">If you are exporting more than 100K mailboxes, you will need to use the following Powershell to download the Export results:  [Exporting results from more than 100K mailboxes](https://docs.microsoft.com/microsoft-365/compliance/export-search-results?view=o365-worldwide%23exporting-results-from-more-than-100000-mailboxes).</span></span>
