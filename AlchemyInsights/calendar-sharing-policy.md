---
title: 618 Правила за споделяне на календар
ms.author: chrisda
author: chrisda
manager: scotv
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "618"
- "899"
- "3800014"
ms.assetid: bc3db17b-87f8-4e50-b3ee-8b105b70d67a
ms.openlocfilehash: cc5827975eff10a119281541622224d0e37f08a7
ms.sourcegitcommit: 2afad0b107d03cd8c4de0b85b5bee38a13a7960d
ms.translationtype: MT
ms.contentlocale: bg-BG
ms.lasthandoff: 05/26/2020
ms.locfileid: "44372988"
---
# <a name="policy-error-when-sharing-a-calendar"></a><span data-ttu-id="32392-102">Грешка при споделяне на календар</span><span class="sxs-lookup"><span data-stu-id="32392-102">Policy error when sharing a calendar</span></span>

1. <span data-ttu-id="32392-103">Направете едно от следните неща, според вашата ситуация:</span><span class="sxs-lookup"><span data-stu-id="32392-103">Do one of the following, as appropriate for your situation:</span></span>
    - <span data-ttu-id="32392-104">Свързване с Exchange Online чрез отдалечен PowerShell.</span><span class="sxs-lookup"><span data-stu-id="32392-104">Connect to Exchange Online by using Remote PowerShell.</span></span> <span data-ttu-id="32392-105">За повече информация вижте [Свързване към Exchange Online чрез отдалечен PowerShell](https://technet.microsoft.com/library/jj984289%28v=exchg.160%29.aspx).</span><span class="sxs-lookup"><span data-stu-id="32392-105">For more information, see [Connect to Exchange Online using Remote PowerShell](https://technet.microsoft.com/library/jj984289%28v=exchg.160%29.aspx).</span></span>
    - <span data-ttu-id="32392-106">На локалния сървър отворете обвивката на Exchange за управление.</span><span class="sxs-lookup"><span data-stu-id="32392-106">On the on-premises server, open the Exchange Management Shell.</span></span>
2. <span data-ttu-id="32392-107">Определете правилата за споделяне, които са присвоени на потребителя.</span><span class="sxs-lookup"><span data-stu-id="32392-107">Determine the sharing policy that's assigned to the user.</span></span> <span data-ttu-id="32392-108">За да направите това, изпълнете следната команда и забележете правилата, върнати:</span><span class="sxs-lookup"><span data-stu-id="32392-108">To do this, run the following command and note the policy returned:</span></span>

    `
    Get-Mailbox User1 | fl *sharing*
    `

3. <span data-ttu-id="32392-109">Актуализирайте правилата за споделяне на потребителя.</span><span class="sxs-lookup"><span data-stu-id="32392-109">Update the sharing policy for the user.</span></span> <span data-ttu-id="32392-110">За да направите това, изпълнете следните стъпки:</span><span class="sxs-lookup"><span data-stu-id="32392-110">To do this, follow these steps:</span></span>
    - <span data-ttu-id="32392-111">Отворете центъра за администриране на Exchange.</span><span class="sxs-lookup"><span data-stu-id="32392-111">Open the Exchange admin center.</span></span>
    - <span data-ttu-id="32392-112">Щракнете върху **организация**, след което щракнете двукратно върху правилата, които се присвояват на потребителя в **разделно споделяне**.</span><span class="sxs-lookup"><span data-stu-id="32392-112">Click **Organization**, and then double-click the policy that's assigned to the user under **Individual Sharing**.</span></span> <span data-ttu-id="32392-113">Това е политиката, която е върната в стъпка 2.</span><span class="sxs-lookup"><span data-stu-id="32392-113">This is the policy that was returned in step 2.</span></span>
    - <span data-ttu-id="32392-114">На страницата Правило за споделяне изберете нивото на споделяне на календара, което искате да разрешите под **Посочете каква информация искате да споделите;** щракнете върху **Запиши**.</span><span class="sxs-lookup"><span data-stu-id="32392-114">On the Sharing Rule page, select the calendar sharing level that you want to allow under **Specify what information you want to share**; click **Save**.</span></span>

<span data-ttu-id="32392-115">За повече информация вижте: ["Правилата не позволяват предоставяне то разрешения на това ниво на един или повече от получателите" грешка при опит за споделяне на календар](https://docs.microsoft.com/exchange/troubleshoot/calendar-sharing/policy-permissions-issue).</span><span class="sxs-lookup"><span data-stu-id="32392-115">For more information see: ["Policy does not allow granting permissions at this level to one or more of the recipient(s)" error when user tries to share calendar](https://docs.microsoft.com/exchange/troubleshoot/calendar-sharing/policy-permissions-issue).</span></span>
