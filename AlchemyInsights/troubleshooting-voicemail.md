---
title: 'Отстраняване на неизправности с гласовата поща '
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 12/09/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9002347"
- "7564"
ms.openlocfilehash: a2d26da512838ae112c352fe21366074b69fa224
ms.sourcegitcommit: 3802f2f4db4f53a408a360187db67f2296448c21
ms.translationtype: MT
ms.contentlocale: bg-BG
ms.lasthandoff: 12/09/2020
ms.locfileid: "49676857"
---
# <a name="troubleshooting-voicemail"></a><span data-ttu-id="757e2-102">Отстраняване на неизправности с гласовата поща</span><span class="sxs-lookup"><span data-stu-id="757e2-102">Troubleshooting Voicemail</span></span>

<span data-ttu-id="757e2-103">Уверете се, че функцията "заето при работа" е умишлено.</span><span class="sxs-lookup"><span data-stu-id="757e2-103">Ensure that the Busy on Busy feature is intentional.</span></span>

<span data-ttu-id="757e2-104">Ако тази функция не е необходима за този потребител:</span><span class="sxs-lookup"><span data-stu-id="757e2-104">If this feature is not needed on this user:</span></span>

1. <span data-ttu-id="757e2-105">Отидете в [центъра за администриране на Teams](https://admin.teams.microsoft.com/policies/calling).</span><span class="sxs-lookup"><span data-stu-id="757e2-105">Go to [Teams Admin center](https://admin.teams.microsoft.com/policies/calling).</span></span>
1. <span data-ttu-id="757e2-106">В навигационните правила за **гласови**  >  **разговори** в ляво  >  **управление Управлявайте правилата** за **правилата за обаждания**.</span><span class="sxs-lookup"><span data-stu-id="757e2-106">On the left rail navigate **Voice** > **Calling policies** > **Manage Policies** on the **Calling Policy**.</span></span>
1. <span data-ttu-id="757e2-107">Изберете **управление на потребители**.</span><span class="sxs-lookup"><span data-stu-id="757e2-107">Select **Manage Users**.</span></span>
1. <span data-ttu-id="757e2-108">Търсене на потребител и промяна на правилата за обаждания към този, който е **зает при работа, е наличен, когато сте в разговор** с **изкл**.</span><span class="sxs-lookup"><span data-stu-id="757e2-108">Search for user and change the Calling Policy to one that has **Busy on Busy is available when in a call** to **Off**.</span></span>
1. <span data-ttu-id="757e2-109">Щракнете върху **Приложи**.</span><span class="sxs-lookup"><span data-stu-id="757e2-109">Click **Apply**.</span></span>
> [!NOTE]
> <span data-ttu-id="757e2-110">Промените в правилата могат да са необходими до 24 часа, за да се копират.</span><span class="sxs-lookup"><span data-stu-id="757e2-110">Changes to policies can take up to 24 hours to replicate.</span></span>

<span data-ttu-id="757e2-111">За повече информация относно тази функция вижте: [зает по зает е наличен, докато сте в разговор](https://docs.microsoft.com/microsoftteams/teams-calling-policy#busy-on-busy-is-available-while-in-a-call).</span><span class="sxs-lookup"><span data-stu-id="757e2-111">For more information on this feature refer to: [Busy on Busy is available while in a call](https://docs.microsoft.com/microsoftteams/teams-calling-policy#busy-on-busy-is-available-while-in-a-call).</span></span>
