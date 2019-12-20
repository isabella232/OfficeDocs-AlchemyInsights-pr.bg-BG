---
title: Грешка в екипите 4c7
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3472"
- "9001211"
ms.openlocfilehash: 0945a341c6456ee4178c0485f3bfb9232fa78a11
ms.sourcegitcommit: 802537a54ef8bde1bdd758ee9a60b6c19d37d6e1
ms.translationtype: MT
ms.contentlocale: bg-BG
ms.lasthandoff: 12/19/2019
ms.locfileid: "40795960"
---
# <a name="4c7-error-in-microsoft-teams"></a><span data-ttu-id="28c30-102">4c7 грешка в екипите на Microsoft</span><span class="sxs-lookup"><span data-stu-id="28c30-102">4c7 error in Microsoft Teams</span></span>

<span data-ttu-id="28c30-103">Тази грешка възниква, защото екипите на Microsoft изисква удостоверяване на формуляри.</span><span class="sxs-lookup"><span data-stu-id="28c30-103">This error occurs because Microsoft Teams requires Forms Authentication.</span></span> <span data-ttu-id="28c30-104">Когато разположите федерация услуги на Active Directory (AD FS), удостоверяване на формуляри не е разрешена за интранет по подразбиране.</span><span class="sxs-lookup"><span data-stu-id="28c30-104">When you deploy Active Directory Federation Services (AD FS), Forms Authentication is not enabled for the intranet by default.</span></span> <span data-ttu-id="28c30-105">Ако интегрирано Windows удостоверяване е неуспешно, получавате подкана да влезете с помощта на удостоверяване на формуляри.</span><span class="sxs-lookup"><span data-stu-id="28c30-105">If Windows Integrated Authentication fails, you are prompted to sign in by using Forms Authentication.</span></span>

<span data-ttu-id="28c30-106">За да разрешите този проблем, разрешете удостоверяване на формуляри чрез конзолната добавка AD FS конзолата на Microsoft за управление (MMC) на компютъра с локалното копие на Active Directory.</span><span class="sxs-lookup"><span data-stu-id="28c30-106">To resolve this issue, enable Forms Authentication by using the AD FS Microsoft Management Console (MMC) snap-in on the computer that has the local copy of Active Directory.</span></span> <span data-ttu-id="28c30-107">За да направите това, изпълнете следните стъпки:</span><span class="sxs-lookup"><span data-stu-id="28c30-107">To do this, follow these steps:</span></span> 

1. <span data-ttu-id="28c30-108">В навигационния екран прегледайте **правила за удостоверяване**.</span><span class="sxs-lookup"><span data-stu-id="28c30-108">In the navigation pane, browse to **Authentication Policies**.</span></span>
2. <span data-ttu-id="28c30-109">Под **действия** в екрана с подробни данни изберете **Редактиране на глобално първично удостоверяване**.</span><span class="sxs-lookup"><span data-stu-id="28c30-109">Under **Actions** in the details pane, select **Edit Global Primary Authentication**.</span></span>
3. <span data-ttu-id="28c30-110">В раздела **интранет** изберете удостоверяване на **формуляри**.</span><span class="sxs-lookup"><span data-stu-id="28c30-110">On the **Intranet** tab, select **Forms Authentication**.</span></span>
4. <span data-ttu-id="28c30-111">Изберете **OK** (или **Приложете**).</span><span class="sxs-lookup"><span data-stu-id="28c30-111">Select **OK** (or **Apply**).</span></span>