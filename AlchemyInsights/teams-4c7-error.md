---
title: Грешка в Teams 4c7
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
- "3472"
- "9001211"
ms.openlocfilehash: 08494b461a24eba8999a5edb99c89af7b17db9b3
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: bg-BG
ms.lasthandoff: 09/14/2020
ms.locfileid: "47700192"
---
# <a name="4c7-error-in-microsoft-teams"></a><span data-ttu-id="33741-102">грешка на 4c7 в Microsoft Teams</span><span class="sxs-lookup"><span data-stu-id="33741-102">4c7 error in Microsoft Teams</span></span>

<span data-ttu-id="33741-103">Тази грешка възниква, тъй като Microsoft Teams изисква удостоверяване на формуляри.</span><span class="sxs-lookup"><span data-stu-id="33741-103">This error occurs because Microsoft Teams requires Forms Authentication.</span></span> <span data-ttu-id="33741-104">Когато разположите услуги на Active Directory за федерацията (AD FS), удостоверяването на формуляри не е разрешено за интранет по подразбиране.</span><span class="sxs-lookup"><span data-stu-id="33741-104">When you deploy Active Directory Federation Services (AD FS), Forms Authentication is not enabled for the intranet by default.</span></span> <span data-ttu-id="33741-105">Ако интегрираното удостоверяване на Windows е неуспешно, получавате подкана да влезете с помощта на удостоверяване на формуляри.</span><span class="sxs-lookup"><span data-stu-id="33741-105">If Windows Integrated Authentication fails, you are prompted to sign in by using Forms Authentication.</span></span>

<span data-ttu-id="33741-106">За да отстраните този проблем, разрешете удостоверяване на формуляри с помощта на конзолната добавка за конзола за управление на Microsoft (MMC) на компютъра, на който е локалното копие на Active Directory.</span><span class="sxs-lookup"><span data-stu-id="33741-106">To resolve this issue, enable Forms Authentication by using the AD FS Microsoft Management Console (MMC) snap-in on the computer that has the local copy of Active Directory.</span></span> <span data-ttu-id="33741-107">За да направите това, изпълнете следните стъпки:</span><span class="sxs-lookup"><span data-stu-id="33741-107">To do this, follow these steps:</span></span> 

1. <span data-ttu-id="33741-108">В навигационния екран отидете на **правила за удостоверяване**.</span><span class="sxs-lookup"><span data-stu-id="33741-108">In the navigation pane, browse to **Authentication Policies**.</span></span>
2. <span data-ttu-id="33741-109">Под **действия** в екрана с подробни данни изберете **Редактиране на глобално основно удостоверяване**.</span><span class="sxs-lookup"><span data-stu-id="33741-109">Under **Actions** in the details pane, select **Edit Global Primary Authentication**.</span></span>
3. <span data-ttu-id="33741-110">В раздела **интранет** изберете удостоверяване на **формуляри**.</span><span class="sxs-lookup"><span data-stu-id="33741-110">On the **Intranet** tab, select **Forms Authentication**.</span></span>
4. <span data-ttu-id="33741-111">Изберете **OK** (или **Apply**).</span><span class="sxs-lookup"><span data-stu-id="33741-111">Select **OK** (or **Apply**).</span></span>