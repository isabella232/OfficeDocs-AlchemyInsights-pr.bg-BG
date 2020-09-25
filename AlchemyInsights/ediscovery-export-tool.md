---
title: инструмент за експортиране на откриването на електронни данни
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "263"
- "928"
- "1100001"
- "3100022"
ms.assetid: b16d310d-1134-4959-be68-d1c0ad463930
ms.openlocfilehash: 67e59182a5053111a08f5fb2be814931a1aa815d
ms.sourcegitcommit: fbe6925797cab0b38172386f1b059dc122e452a4
ms.translationtype: MT
ms.contentlocale: bg-BG
ms.lasthandoff: 09/25/2020
ms.locfileid: "48277927"
---
# <a name="cant-install-or-run-the-ediscovery-export-tool"></a><span data-ttu-id="48469-102">Не можете да инсталирате или да изпълните инструмента за експортиране на откриването на електронни данни?</span><span class="sxs-lookup"><span data-stu-id="48469-102">Can't install or run the eDiscovery Export Tool?</span></span>

<span data-ttu-id="48469-103">Ако не можете да инсталирате или да изпълните инструмента за експортиране на откриването на електронни данни, за да изтеглите резултатите от търсенето, проверете следните неща:</span><span class="sxs-lookup"><span data-stu-id="48469-103">If you can't install or run the eDiscovery Export Tool to download search results, check the following things:</span></span>
  
- <span data-ttu-id="48469-104">Компютърът, който използвате, отговаря на тези предварителни изисквания:</span><span class="sxs-lookup"><span data-stu-id="48469-104">The computer you're using meets these pre-requisites:</span></span>

  - <span data-ttu-id="48469-105">32-или 64-битова версия на Windows 7 и по-нови версии</span><span class="sxs-lookup"><span data-stu-id="48469-105">32- or 64-bit versions of Windows 7 and later versions</span></span>

  - <span data-ttu-id="48469-106">Microsoft .NET Framework 4.7</span><span class="sxs-lookup"><span data-stu-id="48469-106">Microsoft .NET Framework 4.7</span></span>

  - <span data-ttu-id="48469-107">Поддържан браузър:</span><span class="sxs-lookup"><span data-stu-id="48469-107">A supported browser:</span></span>

  - <span data-ttu-id="48469-108">Microsoft Edge</span><span class="sxs-lookup"><span data-stu-id="48469-108">Microsoft Edge</span></span>

    <span data-ttu-id="48469-109">Или</span><span class="sxs-lookup"><span data-stu-id="48469-109">Or</span></span>

  - <span data-ttu-id="48469-110">Internet Explorer 10 и по-нови версии</span><span class="sxs-lookup"><span data-stu-id="48469-110">Internet Explorer 10 and later versions</span></span>

    <span data-ttu-id="48469-111">Други браузъри, като например Google Chrome и Mozilla Firefox, не се поддържат.</span><span class="sxs-lookup"><span data-stu-id="48469-111">Other browsers, such as Google Chrome and Mozilla Firefox aren't supported.</span></span>

- <span data-ttu-id="48469-112">Вашата организация може да се свърже с крайната точка в Azure, която е \*\* \* . blob.Core.Windows.net\*\* (Заместващият символ представлява уникален идентификатор за вашето задание за експортиране).</span><span class="sxs-lookup"><span data-stu-id="48469-112">Your organization can connect to the endpoint in Azure, which is **\*.blob.core.windows.net** (the wildcard represents a unique identifier for your export job).</span></span>

- <span data-ttu-id="48469-113">Присвоявате ви роля за експортиране в центъра за съответствие на защитата на Microsoft 365 &amp; .</span><span class="sxs-lookup"><span data-stu-id="48469-113">You're assigned the Export role in the Microsoft 365 Security &amp; Compliance Center.</span></span> <span data-ttu-id="48469-114">По подразбиране тази роля се присвоява само към ролевата група "Диспечер за откриване на електронни данни".</span><span class="sxs-lookup"><span data-stu-id="48469-114">By default, this role is only assigned to the eDiscovery Manager role group.</span></span> <span data-ttu-id="48469-115">Вижте даване на [разрешения за откриване](https://docs.microsoft.com/microsoft-365/compliance/assign-ediscovery-permissions)на електронни данни.</span><span class="sxs-lookup"><span data-stu-id="48469-115">See [Assign eDiscovery permissions](https://docs.microsoft.com/microsoft-365/compliance/assign-ediscovery-permissions).</span></span>

<span data-ttu-id="48469-116">За повече информация вижте [експортиране на резултати от търсене на съдържание](https://docs.microsoft.com/microsoft-365/compliance/export-search-results).</span><span class="sxs-lookup"><span data-stu-id="48469-116">For more information, see [Export Content Search results](https://docs.microsoft.com/microsoft-365/compliance/export-search-results).</span></span>

<span data-ttu-id="48469-117">Ако експортирате повече от 100K пощенски кутии, ще трябва да използвате следния PowerShell, за да изтеглите резултатите от износа:  [експортиране на резултати от повече от 100k пощенски кутии](https://docs.microsoft.com/microsoft-365/compliance/export-search-results?view=o365-worldwide%23exporting-results-from-more-than-100000-mailboxes).</span><span class="sxs-lookup"><span data-stu-id="48469-117">If you are exporting more than 100K mailboxes, you will need to use the following Powershell to download the Export results:  [Exporting results from more than 100K mailboxes](https://docs.microsoft.com/microsoft-365/compliance/export-search-results?view=o365-worldwide%23exporting-results-from-more-than-100000-mailboxes).</span></span>