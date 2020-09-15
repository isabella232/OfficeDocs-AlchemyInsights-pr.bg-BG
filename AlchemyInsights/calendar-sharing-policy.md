---
title: Правила за споделяне на календар в 618
ms.author: chrisda
author: chrisda
manager: scotv
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "618"
- "899"
- "3800014"
ms.assetid: bc3db17b-87f8-4e50-b3ee-8b105b70d67a
ms.openlocfilehash: d2511183d068330cdcfb4e08b08df4f18625c822
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: bg-BG
ms.lasthandoff: 09/14/2020
ms.locfileid: "47684219"
---
# <a name="policy-error-when-sharing-a-calendar"></a><span data-ttu-id="3aeb7-102">Грешка в правилата при споделяне на календар</span><span class="sxs-lookup"><span data-stu-id="3aeb7-102">Policy error when sharing a calendar</span></span>

1. <span data-ttu-id="3aeb7-103">Направете едно от следните неща, както е подходящо за вашата ситуация:</span><span class="sxs-lookup"><span data-stu-id="3aeb7-103">Do one of the following, as appropriate for your situation:</span></span>
    - <span data-ttu-id="3aeb7-104">Свържете се с Exchange Online, като използвате отдалечен PowerShell.</span><span class="sxs-lookup"><span data-stu-id="3aeb7-104">Connect to Exchange Online by using Remote PowerShell.</span></span> <span data-ttu-id="3aeb7-105">За повече информация вижте [Свързване към Exchange Online чрез отдалечен PowerShell](https://technet.microsoft.com/library/jj984289%28v=exchg.160%29.aspx).</span><span class="sxs-lookup"><span data-stu-id="3aeb7-105">For more information, see [Connect to Exchange Online using Remote PowerShell](https://technet.microsoft.com/library/jj984289%28v=exchg.160%29.aspx).</span></span>
    - <span data-ttu-id="3aeb7-106">В локалния сървър Отворете обвивката за управление на Exchange.</span><span class="sxs-lookup"><span data-stu-id="3aeb7-106">On the on-premises server, open the Exchange Management Shell.</span></span>
2. <span data-ttu-id="3aeb7-107">Определяне на правилата за споделяне, присвоени на потребителя.</span><span class="sxs-lookup"><span data-stu-id="3aeb7-107">Determine the sharing policy that's assigned to the user.</span></span> <span data-ttu-id="3aeb7-108">За да направите това, изпълнете следната команда и имайте предвид, че върнатите правила:</span><span class="sxs-lookup"><span data-stu-id="3aeb7-108">To do this, run the following command and note the policy returned:</span></span>

    `
    Get-Mailbox User1 | fl *sharing*
    `

3. <span data-ttu-id="3aeb7-109">Актуализиране на правилата за споделяне за потребителя.</span><span class="sxs-lookup"><span data-stu-id="3aeb7-109">Update the sharing policy for the user.</span></span> <span data-ttu-id="3aeb7-110">За да направите това, изпълнете следните стъпки:</span><span class="sxs-lookup"><span data-stu-id="3aeb7-110">To do this, follow these steps:</span></span>
    - <span data-ttu-id="3aeb7-111">Отворете центъра за администриране на Exchange.</span><span class="sxs-lookup"><span data-stu-id="3aeb7-111">Open the Exchange admin center.</span></span>
    - <span data-ttu-id="3aeb7-112">Щракнете върху **организация**и след това щракнете двукратно върху правилото, което е присвоено на потребителя под **индивидуално споделяне**.</span><span class="sxs-lookup"><span data-stu-id="3aeb7-112">Click **Organization**, and then double-click the policy that's assigned to the user under **Individual Sharing**.</span></span> <span data-ttu-id="3aeb7-113">Това е правилото, което е върнато в стъпка 2.</span><span class="sxs-lookup"><span data-stu-id="3aeb7-113">This is the policy that was returned in step 2.</span></span>
    - <span data-ttu-id="3aeb7-114">На страницата правило за споделяне изберете ниво на споделяне на календара, което искате да разрешите под **Задаване каква информация искате да споделите**; щракнете върху **Запиши**.</span><span class="sxs-lookup"><span data-stu-id="3aeb7-114">On the Sharing Rule page, select the calendar sharing level that you want to allow under **Specify what information you want to share**; click **Save**.</span></span>

<span data-ttu-id="3aeb7-115">За повече информация вижте: ["правилата не позволяват даване на разрешения на това ниво на една или повече от тези получатели", когато потребителят се опитва да сподели календар](https://docs.microsoft.com/exchange/troubleshoot/calendar-sharing/policy-permissions-issue).</span><span class="sxs-lookup"><span data-stu-id="3aeb7-115">For more information see: ["Policy does not allow granting permissions at this level to one or more of the recipient(s)" error when user tries to share calendar](https://docs.microsoft.com/exchange/troubleshoot/calendar-sharing/policy-permissions-issue).</span></span>
