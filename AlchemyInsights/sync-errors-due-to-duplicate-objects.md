---
title: 902 (грешки при синхронизиране поради дублирани обекти)
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom: 902
ms.assetid: 9d9277a5-c825-4512-8d54-7138b2ee0c40
ms.openlocfilehash: 75b684c5c6b4a594af069d8ed668df95726e1b31
ms.sourcegitcommit: 0eb4f9bde53395b5fd4b5cd4ffc56ca96db91298
ms.translationtype: MT
ms.contentlocale: bg-BG
ms.lasthandoff: 03/10/2021
ms.locfileid: "50708051"
---
# <a name="sync-errors-due-to-duplicate-objects"></a><span data-ttu-id="b3301-102">Грешки при синхронизиране поради дублирани обекти</span><span class="sxs-lookup"><span data-stu-id="b3301-102">Sync errors due to duplicate objects</span></span>

<span data-ttu-id="b3301-103">Възможно е да получите едно от следните съобщения за грешка, когато синхронизирането на справочен указател завърши в Microsoft 365:</span><span class="sxs-lookup"><span data-stu-id="b3301-103">You might receive one of the following error messages when directory synchronization finishes in Microsoft 365:</span></span>

- <span data-ttu-id="b3301-104">Не можете да актуализирате този обект в Microsoft Online Services, тъй като следните атрибути, свързани с този обект, имат стойности, които вече може да са свързани с друг обект в локалния указател.</span><span class="sxs-lookup"><span data-stu-id="b3301-104">Unable to update this object in Microsoft Online Services because the following attributes associated with this object have values that may already be associated with another object in your local directory.</span></span>

- <span data-ttu-id="b3301-105">Синхронизиран обект със същия адрес за прокси сървър вече съществува във вашия указател на Microsoft Online Services.</span><span class="sxs-lookup"><span data-stu-id="b3301-105">A synchronized object with the same proxy address already exists in your Microsoft Online Services directory.</span></span>

- <span data-ttu-id="b3301-106">Не можете да актуализирате този обект, тъй като следните атрибути, свързани с този обект, имат стойности, които вече може да са свързани с други обекти във вашите локални справочни услуги: UserPrincipalName.</span><span class="sxs-lookup"><span data-stu-id="b3301-106">Unable to update this object because the following attributes associated with this object have values that may already be associated with another object in your local directory services: UserPrincipalName.</span></span>

<span data-ttu-id="b3301-107">За да идентифицирате и коригирате проблема, изтеглете и изпълнете [инструмента за отстраняване на грешки в IdFix](https://github.com/Microsoft/idfix).</span><span class="sxs-lookup"><span data-stu-id="b3301-107">To identify and fix the issue, download and run the [IdFix DirSync Error Remediation Tool](https://github.com/Microsoft/idfix).</span></span>

<span data-ttu-id="b3301-108">За повече информация вижте [KB2647098](https://support.microsoft.com/help/2647098/duplicate-or-invalid-attributes-prevent-directory-synchronization-in-o).</span><span class="sxs-lookup"><span data-stu-id="b3301-108">For more information, see [KB2647098](https://support.microsoft.com/help/2647098/duplicate-or-invalid-attributes-prevent-directory-synchronization-in-o).</span></span>
