---
title: Грешка в Teams 4c7
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3472"
- "9001211"
ms.openlocfilehash: 51f2aa936e803b63bcbdf73b89959cd3a1757751
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: bg-BG
ms.lasthandoff: 04/15/2021
ms.locfileid: "51786658"
---
# <a name="4c7-error-in-microsoft-teams"></a><span data-ttu-id="e3e29-102">Грешка 4c7 в Microsoft Teams</span><span class="sxs-lookup"><span data-stu-id="e3e29-102">4c7 error in Microsoft Teams</span></span>

<span data-ttu-id="e3e29-103">Тази грешка възниква, защото Microsoft Teams изисква удостоверяване на формуляри.</span><span class="sxs-lookup"><span data-stu-id="e3e29-103">This error occurs because Microsoft Teams requires Forms Authentication.</span></span> <span data-ttu-id="e3e29-104">Когато разположите услугите за федериране на Active Directory (AD FS), удостоверяването на формуляри не е разрешено за интранет по подразбиране.</span><span class="sxs-lookup"><span data-stu-id="e3e29-104">When you deploy Active Directory Federation Services (AD FS), Forms Authentication is not enabled for the intranet by default.</span></span> <span data-ttu-id="e3e29-105">Ако интегрираното удостоверяване на Windows е неуспешно, ще получите подкана да влезете с помощта на удостоверяване на формуляри.</span><span class="sxs-lookup"><span data-stu-id="e3e29-105">If Windows Integrated Authentication fails, you are prompted to sign in by using Forms Authentication.</span></span>

<span data-ttu-id="e3e29-106">За да разрешите този проблем, разрешете удостоверяването на формуляри с помощта на конзолната добавка AD FS Microsoft Management Console (MMC) на компютъра, на който е локалното копие на Active Directory.</span><span class="sxs-lookup"><span data-stu-id="e3e29-106">To resolve this issue, enable Forms Authentication by using the AD FS Microsoft Management Console (MMC) snap-in on the computer that has the local copy of Active Directory.</span></span> <span data-ttu-id="e3e29-107">За да направите това, изпълнете следните стъпки:</span><span class="sxs-lookup"><span data-stu-id="e3e29-107">To do this, follow these steps:</span></span> 

1. <span data-ttu-id="e3e29-108">В навигационния екран отидете на Правила **за удостоверяване**.</span><span class="sxs-lookup"><span data-stu-id="e3e29-108">In the navigation pane, browse to **Authentication Policies**.</span></span>
2. <span data-ttu-id="e3e29-109">Под **Действия** в екрана с подробни данни изберете **Редактиране на глобално основно удостоверяване**.</span><span class="sxs-lookup"><span data-stu-id="e3e29-109">Under **Actions** in the details pane, select **Edit Global Primary Authentication**.</span></span>
3. <span data-ttu-id="e3e29-110">В раздела **Интранет** изберете Удостоверяване **на формуляри**.</span><span class="sxs-lookup"><span data-stu-id="e3e29-110">On the **Intranet** tab, select **Forms Authentication**.</span></span>
4. <span data-ttu-id="e3e29-111">Изберете **OK** (или **Приложи**).</span><span class="sxs-lookup"><span data-stu-id="e3e29-111">Select **OK** (or **Apply**).</span></span>