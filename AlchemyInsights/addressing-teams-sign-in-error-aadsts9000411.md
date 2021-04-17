---
title: Адресиране на грешка при влизане в Teams AADSTS9000411
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9000744"
- "5689"
ms.openlocfilehash: 7b0e90e3fea716df649ec906ad8b3008386684be
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: bg-BG
ms.lasthandoff: 04/15/2021
ms.locfileid: "51821976"
---
# <a name="addressing-teams-sign-in-error-aadsts9000411"></a><span data-ttu-id="16195-102">Адресиране на грешка при влизане в Teams AADSTS9000411</span><span class="sxs-lookup"><span data-stu-id="16195-102">Addressing Teams sign-in error AADSTS9000411</span></span>

<span data-ttu-id="16195-103">Когато влезете в Microsoft Teams, може да получите грешката: За съжаление, имаме проблеми с влизането ви в **AADSTS9000411: Искането не е форматирано правилно. Параметърът "login_hint" е дублиран.**</span><span class="sxs-lookup"><span data-stu-id="16195-103">When signing in to Microsoft Teams, you may receive the error: **Sorry, but we're having trouble with signing you in AADSTS9000411: The request is not properly formatted. The parameter "login_hint" is duplicated.**</span></span>

<span data-ttu-id="16195-104">За да решите този проблем, уверете се, че вашите клиенти на Microsoft Teams са актуализирани.</span><span class="sxs-lookup"><span data-stu-id="16195-104">To address this issue, please ensure your Microsoft Teams clients are updated.</span></span> <span data-ttu-id="16195-105">За повече информация относно актуализирането на вашия клиент вижте [Актуализиране на Microsoft Teams](https://support.office.com/article/Update-Microsoft-Teams-535a8e4b-45f0-4f6c-8b3d-91bca7a51db1).</span><span class="sxs-lookup"><span data-stu-id="16195-105">For more information on updating your client, see [Update Microsoft Teams](https://support.office.com/article/Update-Microsoft-Teams-535a8e4b-45f0-4f6c-8b3d-91bca7a51db1).</span></span>

<span data-ttu-id="16195-106">Ако по някаква причина не можете да актуализирате клиента си, излизането от клиента ще изчисти повечето кеширани данни.</span><span class="sxs-lookup"><span data-stu-id="16195-106">If you cannot update your client for some reason, logging off the client will clear most cached data.</span></span> <span data-ttu-id="16195-107">Ако обаче все още имате проблеми след излизане/влизане, излезте от Teams и изчистете кеша на клиента, като направите следното:</span><span class="sxs-lookup"><span data-stu-id="16195-107">However, if you still have issues after logoff/logon, quit Teams and please clear your client cache by doing the following:</span></span>
1. <span data-ttu-id="16195-108">Затворете Microsoft Teams.</span><span class="sxs-lookup"><span data-stu-id="16195-108">Close Microsoft Teams.</span></span>
2. <span data-ttu-id="16195-109">Отидете на: %appdata%\microsoft\teams и изтрийте всички файлове.</span><span class="sxs-lookup"><span data-stu-id="16195-109">Go to: %appdata%\microsoft\teams and delete all the files.</span></span>
3. <span data-ttu-id="16195-110">Отворете отново Microsoft Teams.</span><span class="sxs-lookup"><span data-stu-id="16195-110">Reopen Microsoft Teams.</span></span>
