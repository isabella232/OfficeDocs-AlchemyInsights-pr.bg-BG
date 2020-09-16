---
title: Връщане към по-стара компилация на Office
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/24/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "1741"
- "9000140"
ms.openlocfilehash: 9f6a812def2b46bf32d836781d0336aea5ba3ed1
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: bg-BG
ms.lasthandoff: 09/14/2020
ms.locfileid: "47727808"
---
# <a name="roll-back-to-an-earlier-build-of-office"></a><span data-ttu-id="f12ec-102">Връщане към по-стара компилация на Office</span><span class="sxs-lookup"><span data-stu-id="f12ec-102">Roll back to an earlier build of Office</span></span>

<span data-ttu-id="f12ec-103">За да се върнете към по-стара компилация или версия на приложения на Microsoft 365, вижте [как да се върнете към по-стара версия на Office](https://support.microsoft.com/help/2770432/how-to-revert-to-an-earlier-version-of-office-2013-or-office-2016-clic).</span><span class="sxs-lookup"><span data-stu-id="f12ec-103">To revert to an earlier Microsoft 365 Apps build or version, see [How to revert to an earlier version of Office](https://support.microsoft.com/help/2770432/how-to-revert-to-an-earlier-version-of-office-2013-or-office-2016-clic).</span></span> <span data-ttu-id="f12ec-104">За да превключите от един абонамент за Microsoft 365 към друг, вижте  [Превключване към различен план на microsoft 365 за бизнеса](https://docs.microsoft.com/office365/admin/subscriptions-and-billing/switch-to-a-different-plan).</span><span class="sxs-lookup"><span data-stu-id="f12ec-104">To switch from one Microsoft 365 subscription to another, see  [Switch to a different Microsoft 365 for business plan](https://docs.microsoft.com/office365/admin/subscriptions-and-billing/switch-to-a-different-plan).</span></span>

- <span data-ttu-id="f12ec-105">За да намерите версията на Office, която използвате в момента, вижте [за Office: коя версия на Office използвам?](https://support.office.com/article/about-office-what-version-of-office-am-i-using-932788b8-a3ce-44bf-bb09-e334518b8b19).</span><span class="sxs-lookup"><span data-stu-id="f12ec-105">To find the version of Office you are currently using, see [About Office: What version of Office am I using?](https://support.office.com/article/about-office-what-version-of-office-am-i-using-932788b8-a3ce-44bf-bb09-e334518b8b19).</span></span>
- <span data-ttu-id="f12ec-106">За да определите компилацията, в която искате да се върнете, вижте [Хронология на актуализациите за приложенията на Microsoft 365 (подредени по дата)](https://docs.microsoft.com/officeupdates/update-history-office365-proplus-by-date?redirectSourcePath=%252fen-us%252farticle%252fae942449-1fca-4484-898b-a933ea23def7).</span><span class="sxs-lookup"><span data-stu-id="f12ec-106">To determine the build you want to roll back to, see [Update history for Microsoft 365 Apps (listed by date)](https://docs.microsoft.com/officeupdates/update-history-office365-proplus-by-date?redirectSourcePath=%252fen-us%252farticle%252fae942449-1fca-4484-898b-a933ea23def7).</span></span>
- <span data-ttu-id="f12ec-107">Конфигурирайте настройката **TargetVersion** , за да се върнете към предишната компилация, като използвате [как да се върнете към по-ранна версия на Office](https://support.microsoft.com/help/2770432/how-to-revert-to-an-earlier-version-of-office-2013-or-office-2016-clic) или да [забавите получаването на актуализациите на функциите от полу-годишен канал, когато използвате мрежата за доставяне на съдържание на Office (CDN)](https://docs.microsoft.com/deployoffice/delay-receiving-feature-updates-from-deferred-channel-for-office-365-proplus#delay-receiving-feature-updates-from-semi-annual-channel-when-using-the-office-content-delivery-network-cdn).</span><span class="sxs-lookup"><span data-stu-id="f12ec-107">Configure the **TargetVersion** setting to revert to the earlier build by using [How to revert to an earlier version of Office](https://support.microsoft.com/help/2770432/how-to-revert-to-an-earlier-version-of-office-2013-or-office-2016-clic) or [Delay receiving feature updates from Semi-Annual Channel when using the Office Content Delivery Network (CDN)](https://docs.microsoft.com/deployoffice/delay-receiving-feature-updates-from-deferred-channel-for-office-365-proplus#delay-receiving-feature-updates-from-semi-annual-channel-when-using-the-office-content-delivery-network-cdn).</span></span></br>
    <span data-ttu-id="f12ec-108">Когато целевата версия е зададена, Office актуализира тази версия следващия път, когато търси актуализации.</span><span class="sxs-lookup"><span data-stu-id="f12ec-108">When the target version is set, Office updates to that version the next time it looks for updates.</span></span>