---
title: Проблеми с производителността – SharePoint или OneDrive
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 9225ec0f-771f-4d7a-8157-e188953107aa
ms.openlocfilehash: 39ec9b746c47414f1cfaad1342491b8f33a47d6f
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: bg-BG
ms.lasthandoff: 09/15/2020
ms.locfileid: "47771233"
---
# <a name="sharepoint-or-onedrive-slow-inaccessible-or-unavailable-for-multiple-users"></a><span data-ttu-id="8a2b5-102">SharePoint или OneDrive – бавен, недостъпен или недостъпен за множество потребители</span><span class="sxs-lookup"><span data-stu-id="8a2b5-102">SharePoint or OneDrive Slow, Inaccessible or Unavailable for Multiple Users</span></span>

<span data-ttu-id="8a2b5-103">Ако даден сайт на OneDrive или SharePoint не е достъпен за множество потребители, които преди това са имали достъп, е възможно да има временен проблем с услугата.</span><span class="sxs-lookup"><span data-stu-id="8a2b5-103">If a OneDrive or SharePoint site is not available to multiple users who previously had access, there may be a temporary service issue.</span></span> <span data-ttu-id="8a2b5-104">[Проверете таблото за изправност на услугите](https://portal.office.com/adminportal/home#/servicehealth).</span><span class="sxs-lookup"><span data-stu-id="8a2b5-104">[Check the service health dashboard](https://portal.office.com/adminportal/home#/servicehealth).</span></span>

<span data-ttu-id="8a2b5-105">**Добавяне и лицензиране на потребителя**</span><span class="sxs-lookup"><span data-stu-id="8a2b5-105">**Add and license the user**</span></span>

<span data-ttu-id="8a2b5-106">Уверете се, че [присвоявате лицензи на потребители в Microsoft 365 за бизнеса](https://docs.microsoft.com/microsoft-365/admin/add-users/add-users).</span><span class="sxs-lookup"><span data-stu-id="8a2b5-106">Ensure that you [Assign licenses to users in Microsoft 365 for business](https://docs.microsoft.com/microsoft-365/admin/add-users/add-users).</span></span>


<span data-ttu-id="8a2b5-107">**Присвояване на разрешения**</span><span class="sxs-lookup"><span data-stu-id="8a2b5-107">**Assign Permissions**</span></span>

<span data-ttu-id="8a2b5-108">Ако на потребителя е даден лиценз за SharePoint и все още получава съобщение за отказан достъп, трябва да се уверите, че има присвоено [подходящо ниво на разрешение](https://docs.microsoft.com/sharepoint/understanding-permission-levels) .</span><span class="sxs-lookup"><span data-stu-id="8a2b5-108">If the user has been assigned a Sharepoint license and is still receiving an access denied message, please ensure they have the [appropriate permission level](https://docs.microsoft.com/sharepoint/understanding-permission-levels) assigned.</span></span>

<span data-ttu-id="8a2b5-109">**Помислете за използване на функцията за искане на достъп**</span><span class="sxs-lookup"><span data-stu-id="8a2b5-109">**Consider using the access request feature**</span></span>

<span data-ttu-id="8a2b5-110">[Функцията за искане на достъп](https://support.office.com/article/Set-up-and-manage-access-requests-94B26E0B-2822-49D4-929A-8455698654B3) позволява на хората да искат достъп до съдържание, което в момента няма разрешение да виждат.</span><span class="sxs-lookup"><span data-stu-id="8a2b5-110">The [access request feature](https://support.office.com/article/Set-up-and-manage-access-requests-94B26E0B-2822-49D4-929A-8455698654B3) allows people to request access to content that they do not currently have permission to see.</span></span>

<span data-ttu-id="8a2b5-111">**Разрешаване на скрипт по избор може да доведе до проблеми с отказан достъп**</span><span class="sxs-lookup"><span data-stu-id="8a2b5-111">**Allow custom script may cause access denied issues**</span></span>

<span data-ttu-id="8a2b5-112">Има някои сценарии, при които функцията за *Разрешаване на скрипт по избор* може да Появява отказан достъп.</span><span class="sxs-lookup"><span data-stu-id="8a2b5-112">There are certain scenarios where the *Allow custom script* feature may be presenting an access denied.</span></span> <span data-ttu-id="8a2b5-113">За списък на засегнатите функции, съображения за защитата и възможност за Дезактивиране на функцията.</span><span class="sxs-lookup"><span data-stu-id="8a2b5-113">For a list of features affected, security considerations and the ability to disable the feature.</span></span> <span data-ttu-id="8a2b5-114">Моля [, посетете разрешаване или забраняване на скрипт по избор](https://docs.microsoft.com/sharepoint/allow-or-prevent-custom-script).</span><span class="sxs-lookup"><span data-stu-id="8a2b5-114">Please visit [Allow or prevent custom script](https://docs.microsoft.com/sharepoint/allow-or-prevent-custom-script).</span></span>

