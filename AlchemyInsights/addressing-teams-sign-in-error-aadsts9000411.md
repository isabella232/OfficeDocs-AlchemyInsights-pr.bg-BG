---
title: Отстраняване на грешки при влизане в AADSTS9000411
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9000744"
- "5689"
ms.openlocfilehash: 8ca3793b8cd12b7ad2510ca0b3be58c32a61c14c
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: bg-BG
ms.lasthandoff: 09/14/2020
ms.locfileid: "47687027"
---
# <a name="addressing-teams-sign-in-error-aadsts9000411"></a><span data-ttu-id="4fd9b-102">Отстраняване на грешки при влизане в AADSTS9000411</span><span class="sxs-lookup"><span data-stu-id="4fd9b-102">Addressing Teams sign-in error AADSTS9000411</span></span>

<span data-ttu-id="4fd9b-103">Когато влизате в Microsoft Teams, е възможно да получите грешката: **Съжаляваме, но имаме проблеми с влизането ви в AADSTS9000411: заявката не е правилно форматирана. Параметърът "login_hint" е дублиран.**</span><span class="sxs-lookup"><span data-stu-id="4fd9b-103">When signing in to Microsoft Teams, you may receive the error: **Sorry, but we're having trouble with signing you in AADSTS9000411: The request is not properly formatted. The parameter "login_hint" is duplicated.**</span></span>

<span data-ttu-id="4fd9b-104">За да адресирате този проблем, уверете се, че вашите клиенти на Microsoft Teams се актуализират.</span><span class="sxs-lookup"><span data-stu-id="4fd9b-104">To address this issue, please ensure your Microsoft Teams clients are updated.</span></span> <span data-ttu-id="4fd9b-105">За повече информация за актуализирането на клиента вижте [актуализиране на Microsoft Teams](https://support.office.com/article/Update-Microsoft-Teams-535a8e4b-45f0-4f6c-8b3d-91bca7a51db1).</span><span class="sxs-lookup"><span data-stu-id="4fd9b-105">For more information on updating your client, see [Update Microsoft Teams](https://support.office.com/article/Update-Microsoft-Teams-535a8e4b-45f0-4f6c-8b3d-91bca7a51db1).</span></span>

<span data-ttu-id="4fd9b-106">Ако не можете да актуализирате своя клиент по някаква причина, излизането от клиента ще изчисти повечето кеширани данни.</span><span class="sxs-lookup"><span data-stu-id="4fd9b-106">If you cannot update your client for some reason, logging off the client will clear most cached data.</span></span> <span data-ttu-id="4fd9b-107">Ако обаче все още имате проблеми след излизане/влизане, излезте от Teams и моля, изчистете кеша на клиента си, като направите следното:</span><span class="sxs-lookup"><span data-stu-id="4fd9b-107">However, if you still have issues after logoff/logon, quit Teams and please clear your client cache by doing the following:</span></span>
1. <span data-ttu-id="4fd9b-108">Затворете Microsoft Teams.</span><span class="sxs-lookup"><span data-stu-id="4fd9b-108">Close Microsoft Teams.</span></span>
2. <span data-ttu-id="4fd9b-109">Отидете на:%AppData%\microsoft\teams и изтрийте всички файлове.</span><span class="sxs-lookup"><span data-stu-id="4fd9b-109">Go to: %appdata%\microsoft\teams and delete all the files.</span></span>
3. <span data-ttu-id="4fd9b-110">Отворете повторно Microsoft Teams.</span><span class="sxs-lookup"><span data-stu-id="4fd9b-110">Reopen Microsoft Teams.</span></span>
