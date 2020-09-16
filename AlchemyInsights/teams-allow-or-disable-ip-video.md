---
title: Teams позволяване или забраняване на IP видео
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
- "9002537"
- "5617"
ms.openlocfilehash: cf2d67170f846db1d5d2f1ca8c8b50902e200e45
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: bg-BG
ms.lasthandoff: 09/14/2020
ms.locfileid: "47670173"
---
# <a name="teams-allow-or-disable-ip-video"></a><span data-ttu-id="6b99f-102">Teams позволяване или забраняване на IP видео</span><span class="sxs-lookup"><span data-stu-id="6b99f-102">Teams allow or disable IP video</span></span>

<span data-ttu-id="6b99f-103">**Промяна или създаване на правила за събрание**</span><span class="sxs-lookup"><span data-stu-id="6b99f-103">**Change or create a meeting policy**</span></span>

<span data-ttu-id="6b99f-104">За да промените или създадете правила за събрание, отидете в **центъра за администриране на Microsoft teams > събрания > правилата за събранието**.</span><span class="sxs-lookup"><span data-stu-id="6b99f-104">To change or create a meeting policy, go to the **Microsoft Teams admin center > Meetings > Meeting policies**.</span></span> <span data-ttu-id="6b99f-105">Изберете правило от списъка или изберете **Добави**.</span><span class="sxs-lookup"><span data-stu-id="6b99f-105">Select a policy from the list or click **Add**.</span></span> <span data-ttu-id="6b99f-106">Ако създавате нови правила, добавете име и описание.</span><span class="sxs-lookup"><span data-stu-id="6b99f-106">If you're creating a new policy, add a name and description.</span></span> <span data-ttu-id="6b99f-107">Името не може да съдържа специални знаци или да бъде по-дълго от 64 знака.</span><span class="sxs-lookup"><span data-stu-id="6b99f-107">The name can't contain special characters or be longer than 64 characters.</span></span> <span data-ttu-id="6b99f-108">Изберете настройките и след това щракнете върху **Запиши**.</span><span class="sxs-lookup"><span data-stu-id="6b99f-108">Choose your settings, and then click **Save**.</span></span>

<span data-ttu-id="6b99f-109">Например да речем, че имате много потребители и искате да ограничите количеството пропускателна способност, което ще изисква тяхното събрание.</span><span class="sxs-lookup"><span data-stu-id="6b99f-109">For example, say you have many users and you want to limit the amount of bandwidth that their meeting would require.</span></span> <span data-ttu-id="6b99f-110">Можете да създадете нови правила по избор с име "Ограничена пропускателна способност" и да забраните следните настройки:</span><span class="sxs-lookup"><span data-stu-id="6b99f-110">You would create a new custom policy named "Limited bandwidth" and disable the following settings:</span></span>

<span data-ttu-id="6b99f-111">Под **Аудио и видео**:</span><span class="sxs-lookup"><span data-stu-id="6b99f-111">Under **Audio & video**:</span></span>

- <span data-ttu-id="6b99f-112">Изключете разрешаване на записването в облака.</span><span class="sxs-lookup"><span data-stu-id="6b99f-112">Turn off Allow cloud recording.</span></span>
- <span data-ttu-id="6b99f-113">Изключете разрешаване на IP видео.</span><span class="sxs-lookup"><span data-stu-id="6b99f-113">Turn off Allow IP video.</span></span>

<span data-ttu-id="6b99f-114">След това задайте правилата на потребителите.</span><span class="sxs-lookup"><span data-stu-id="6b99f-114">Then assign the policy to the users.</span></span>

<span data-ttu-id="6b99f-115">**Задаване на правила за събрание на потребители**</span><span class="sxs-lookup"><span data-stu-id="6b99f-115">**Assign a meeting policy to users**</span></span>

1. <span data-ttu-id="6b99f-116">В лявата навигация на центъра за администриране на Microsoft Teams отидете на **Потребители**и след това щракнете върху потребителя.</span><span class="sxs-lookup"><span data-stu-id="6b99f-116">In the left navigation of the Microsoft Teams admin center, go to **Users**, and then click the user.</span></span>
2. <span data-ttu-id="6b99f-117">Изберете потребителя, като щракнете вляво от потребителското име и след това щракнете върху **Редактиране на настройките**.</span><span class="sxs-lookup"><span data-stu-id="6b99f-117">Select the user by clicking to the left of the user name, and then click **Edit settings**.</span></span>
3. <span data-ttu-id="6b99f-118">Под **правила за събранието**изберете правилата, които искате да дадете, и след това щракнете върху **Приложи**.</span><span class="sxs-lookup"><span data-stu-id="6b99f-118">Under **Meeting policy**, select the policy you want to assign and then click **Apply**.</span></span>

<span data-ttu-id="6b99f-119">За повече информация вижте [управление на правилата за събрания в Teams](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams).</span><span class="sxs-lookup"><span data-stu-id="6b99f-119">For more information, see [Manage meeting policies in Teams](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams).</span></span>
