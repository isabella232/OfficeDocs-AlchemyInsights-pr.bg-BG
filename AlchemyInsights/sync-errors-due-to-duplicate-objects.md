---
title: 902 (грешки при синхронизиране поради дублиращи се обекти)
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom: 902
ms.assetid: 9d9277a5-c825-4512-8d54-7138b2ee0c40
ms.openlocfilehash: 6ea833e0c4aebe72bc5c02e3dc10c1edc4136dcc
ms.sourcegitcommit: 631cbb5f03e5371f0995e976536d24e9d13746c3
ms.translationtype: MT
ms.contentlocale: bg-BG
ms.lasthandoff: 04/22/2020
ms.locfileid: "43767104"
---
# <a name="sync-errors-due-to-duplicate-objects"></a><span data-ttu-id="13e0f-102">Грешки при синхронизиране поради дублиращи се обекти</span><span class="sxs-lookup"><span data-stu-id="13e0f-102">Sync errors due to duplicate objects</span></span>

<span data-ttu-id="13e0f-103">Може да получите едно от следните съобщения за грешка при синхронизиране на директории в Microsoft 365:</span><span class="sxs-lookup"><span data-stu-id="13e0f-103">You might receive one of the following error messages when directory synchronization finishes in Microsoft 365:</span></span>

- <span data-ttu-id="13e0f-104">Не може да актуализира този обект в онлайн услугите на Microsoft, защото следните атрибути, свързани с този обект, имат стойности, които вече могат да са свързани с друг обект във вашата локална директория.</span><span class="sxs-lookup"><span data-stu-id="13e0f-104">Unable to update this object in Microsoft Online Services because the following attributes associated with this object have values that may already be associated with another object in your local directory.</span></span>

- <span data-ttu-id="13e0f-105">Синхронизиран обект със същия прокси адрес вече съществува във вашата директория на онлайн услугите на Microsoft.</span><span class="sxs-lookup"><span data-stu-id="13e0f-105">A synchronized object with the same proxy address already exists in your Microsoft Online Services directory.</span></span>

- <span data-ttu-id="13e0f-106">Не може да актуализира този обект, защото следните атрибути, свързани с този обект, имат стойности, които вече могат да бъдат свързани с друг обект във вашата локална справочна услуга: UserPrincipalName.</span><span class="sxs-lookup"><span data-stu-id="13e0f-106">Unable to update this object because the following attributes associated with this object have values that may already be associated with another object in your local directory services: UserPrincipalName.</span></span>

<span data-ttu-id="13e0f-107">За да идентифицирате и решите проблема, изтеглете и изпълнете инструмента за отстраняване на [грешки IdFix DirSync.](https://www.microsoft.com/download/details.aspx?id=36832)</span><span class="sxs-lookup"><span data-stu-id="13e0f-107">To identify and fix the issue, download and run the [IdFix DirSync Error Remediation Tool](https://www.microsoft.com/download/details.aspx?id=36832).</span></span>

<span data-ttu-id="13e0f-108">За повече информация вижте [KB2647098](https://support.microsoft.com/help/2647098/duplicate-or-invalid-attributes-prevent-directory-synchronization-in-o).</span><span class="sxs-lookup"><span data-stu-id="13e0f-108">For more information, see [KB2647098](https://support.microsoft.com/help/2647098/duplicate-or-invalid-attributes-prevent-directory-synchronization-in-o).</span></span>
