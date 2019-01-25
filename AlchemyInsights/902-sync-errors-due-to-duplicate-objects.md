---
title: 902 (синхронизиране грешки поради дублиращи обекти)
ms.author: chrisda
author: chrisda
manager: serdars
ms.date: 5/30/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.assetid: 9d9277a5-c825-4512-8d54-7138b2ee0c40
ms.openlocfilehash: f8db233167a5e2b2ef7290438b8e6d92d0dccb1e
ms.sourcegitcommit: e2864efcfb493b6e46b662b746661a61232bdba7
ms.translationtype: MT
ms.contentlocale: bg-BG
ms.lasthandoff: 01/24/2019
ms.locfileid: "29458719"
---
# <a name="sync-errors-due-to-duplicate-objects"></a><span data-ttu-id="ee299-102">Грешките при синхронизиране поради дублиращи се обекти</span><span class="sxs-lookup"><span data-stu-id="ee299-102">Sync errors due to duplicate objects</span></span>

<span data-ttu-id="ee299-103">Може да се появи едно от следните съобщения за грешка при синхронизиране на директории завършва:</span><span class="sxs-lookup"><span data-stu-id="ee299-103">You might receive one of the following error messages when directory synchronization finishes:</span></span>
  
- <span data-ttu-id="ee299-104">Не може да актуализира този обект в онлайн услугите на Microsoft, защото следните атрибути, свързани с този обект имат стойности, които вече са свързани с друг обект в местна директория.</span><span class="sxs-lookup"><span data-stu-id="ee299-104">Unable to update this object in Microsoft Online Services because the following attributes associated with this object have values that may already be associated with another object in your local directory.</span></span>
    
- <span data-ttu-id="ee299-105">Синхронизиран обект със същия прокси адрес вече съществува в директорията си онлайн услугите на Microsoft.</span><span class="sxs-lookup"><span data-stu-id="ee299-105">A synchronized object with the same proxy address already exists in your Microsoft Online Services directory.</span></span>
    
- <span data-ttu-id="ee299-106">Не може да актуализира този обект, защото следните атрибути, свързани с този обект имат стойности, които вече са свързани с друг обект в вашата местен справочни услуги: UserPrincipalName.</span><span class="sxs-lookup"><span data-stu-id="ee299-106">Unable to update this object because the following attributes associated with this object have values that may already be associated with another object in your local directory services: UserPrincipalName.</span></span>
    
<span data-ttu-id="ee299-107">За да идентифицирате и отстраните проблема, изтеглете и изпълнете [IdFix DirSync грешка отстраняване инструмент](https://www.microsoft.com/download/details.aspx?id=36832).</span><span class="sxs-lookup"><span data-stu-id="ee299-107">To identify and fix the issue, download and run the [IdFix DirSync Error Remediation Tool](https://www.microsoft.com/download/details.aspx?id=36832).</span></span>
  
<span data-ttu-id="ee299-108">За повече информация вижте [KB2647098](https://support.microsoft.com/help/2647098/duplicate-or-invalid-attributes-prevent-directory-synchronization-in-o).</span><span class="sxs-lookup"><span data-stu-id="ee299-108">For more information, see [KB2647098](https://support.microsoft.com/help/2647098/duplicate-or-invalid-attributes-prevent-directory-synchronization-in-o).</span></span>
  

