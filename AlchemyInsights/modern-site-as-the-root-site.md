---
title: Модерен сайт като главния сайт
ms.author: kirks
author: Techwriter40
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: ''
ms.openlocfilehash: 6166493f79379f44b1a9bbbaca6becfe624fe912
ms.sourcegitcommit: 22ce2315c8cf643137ab3420cdc1cda41433d44a
ms.translationtype: MT
ms.contentlocale: bg-BG
ms.lasthandoff: 05/14/2019
ms.locfileid: "34057671"
---
# <a name="modern-site-as-root-site"></a><span data-ttu-id="c2f6c-102">Модерен сайт като главния сайт</span><span class="sxs-lookup"><span data-stu-id="c2f6c-102">Modern site as root site</span></span>

<span data-ttu-id="c2f6c-103">[Целеви освобождаване](https://docs.microsoft.com/en-us/office365/admin/manage/release-options-in-office-365?view=o365-worldwide) клиенти вече могат да разрешат на съвременните комуникационни сайт опит на класически главния сайт на техните SharePoint наемател.</span><span class="sxs-lookup"><span data-stu-id="c2f6c-103">[Target Release](https://docs.microsoft.com/en-us/office365/admin/manage/release-options-in-office-365?view=o365-worldwide) customers can now enable the modern communication site experience at the classic root site of their SharePoint tenant.</span></span>

<span data-ttu-id="c2f6c-104">Тази функция може да се активира чрез провеждане на прост PowerShell cmdlet.</span><span class="sxs-lookup"><span data-stu-id="c2f6c-104">This feature can be activated by running a simple PowerShell cmdlet.</span></span> <span data-ttu-id="c2f6c-105">На успешното изпълнение на PowerShell (ите) Главният сайт ще има ново съобщение началната страница за сайт.</span><span class="sxs-lookup"><span data-stu-id="c2f6c-105">On the successful execution of the PowerShell command(s), the root site will have a new communication site home page.</span></span> <span data-ttu-id="c2f6c-106">Подробности за изискванията за PowerShell cmdlet и функция са достъпни в статията на [Разреши-SPOCommSite](https://docs.microsoft.com/en-us/powershell/module/sharepoint-online/Enable-SPOCommSite?view=sharepoint-ps).</span><span class="sxs-lookup"><span data-stu-id="c2f6c-106">Details about the PowerShell cmdlet and feature requirements are available in the article [Enable-SPOCommSite](https://docs.microsoft.com/en-us/powershell/module/sharepoint-online/Enable-SPOCommSite?view=sharepoint-ps).</span></span> 

<span data-ttu-id="c2f6c-107">Ние ще бъде постепенно подвижен този вън, на разстояние по подразбиране, за прицел освобождавам клиенти в началото май 2019 г и свитък вън ще бъда наличен световен до края на юни 2019.</span><span class="sxs-lookup"><span data-stu-id="c2f6c-107">We'll be gradually rolling this out, off by default, to Targeted Release customers in early May 2019, and the roll out will be available worldwide by the end of June 2019.</span></span> <span data-ttu-id="c2f6c-108">Продължи да се позова на [Съобщение център](https://admin.microsoft.com/AdminPortal/Home#/MessageCenter) за други нови функции с модерен.</span><span class="sxs-lookup"><span data-stu-id="c2f6c-108">Continue to refer to the [Message Center](https://admin.microsoft.com/AdminPortal/Home#/MessageCenter) for other new features with Modern.</span></span> 

<span data-ttu-id="c2f6c-109">**Важно**: не изтривайте сайта си класически корен да се създаде сайт на модерната комуникация.</span><span class="sxs-lookup"><span data-stu-id="c2f6c-109">**Important**: Do not delete your classic root site to create a modern Communication Site.</span></span> <span data-ttu-id="c2f6c-110">Това не се поддържа от Microsoft.</span><span class="sxs-lookup"><span data-stu-id="c2f6c-110">This is not supported by Microsoft.</span></span> <span data-ttu-id="c2f6c-111">Изтриването на главния сайт ще направи всички SharePoint сайтове във вашата организация недостъпни за всички потребители, докато възстанови сайта или създаване на нов сайт на същия URL адрес.</span><span class="sxs-lookup"><span data-stu-id="c2f6c-111">Deleting the root site will make all SharePoint sites in your organization inaccessible to all users, until you restore the site or create a new site at the same URL.</span></span> 
 
 