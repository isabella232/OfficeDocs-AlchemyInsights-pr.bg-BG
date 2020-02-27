---
title: Създайте имейл улов на всички
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9001524"
- "3732"
ms.openlocfilehash: 35f31c1662547d57c2fc9978ffb495ac29abcc01
ms.sourcegitcommit: 67015549afcbe05f3b77ea314e2ef7e0e439f9f2
ms.translationtype: MT
ms.contentlocale: bg-BG
ms.lasthandoff: 02/26/2020
ms.locfileid: "42286033"
---
# <a name="create-an-email-catch-all"></a><span data-ttu-id="c887c-102">Създайте имейл улов на всички</span><span class="sxs-lookup"><span data-stu-id="c887c-102">Create an email catch all</span></span>

<span data-ttu-id="c887c-103">Използването на улов е силно обезкуражено.</span><span class="sxs-lookup"><span data-stu-id="c887c-103">Use of a catch all is strongly discouraged.</span></span> <span data-ttu-id="c887c-104">По-добре е да се осигури отпадане на подателя, което позволява на изпращачите да знаят, че съобщението им не може да бъде доставено като адресирано, така че те могат да предприемат действия.</span><span class="sxs-lookup"><span data-stu-id="c887c-104">It is better to provide a bounce back to the sender letting senders know their message could not be delivered as addressed so they can take action.</span></span> <span data-ttu-id="c887c-105">Можете също да ограничите наблюдава пощенска кутия само улов а преди валидни имейл адреси.</span><span class="sxs-lookup"><span data-stu-id="c887c-105">You can also limit the monitored mailbox to only catch formerly valid email addresses.</span></span> 

<span data-ttu-id="c887c-106">Всяка уловка всички пощенски кутии ще получи добра сделка спам и евентуално може да запълни, ако не се следи отблизо.</span><span class="sxs-lookup"><span data-stu-id="c887c-106">Any catch all mailbox will receive a good deal of spam and may eventually fill if not closely monitored.</span></span> <span data-ttu-id="c887c-107">(Има граници за получаване.)</span><span class="sxs-lookup"><span data-stu-id="c887c-107">(There are receiving limits.)</span></span> 

<span data-ttu-id="c887c-108">Ако решите да продължите, изпълнете следните стъпки:</span><span class="sxs-lookup"><span data-stu-id="c887c-108">If you decide to proceed, follow these steps:</span></span>

1. <span data-ttu-id="c887c-109">Създаване на динамична група за разпространение & включват "Всички типове получатели".</span><span class="sxs-lookup"><span data-stu-id="c887c-109">Create a Dynamic Distribution Group & include "All Recipient Types."</span></span>

2. <span data-ttu-id="c887c-110">Създаване на специална пощенска кутия за улавяне на имейли, например catchall@domain.com.</span><span class="sxs-lookup"><span data-stu-id="c887c-110">Create a dedicated Mailbox to catch emails, for example, catchall@domain.com.</span></span>

3. <span data-ttu-id="c887c-111">За конкретен домейн Задайте тип domainType на "InternalRelay".</span><span class="sxs-lookup"><span data-stu-id="c887c-111">For the specific domain, set the DomainType to “InternalRelay”.</span></span> <span data-ttu-id="c887c-112">Ако по-късно премахнете улов всички, не забравяйте да зададете домейна на авторитетни.</span><span class="sxs-lookup"><span data-stu-id="c887c-112">If you later remove the catch all, be sure to set the domain back to Authoritative.</span></span>

4. <span data-ttu-id="c887c-113">Създайте правило за транспортиране на поща, както следва:</span><span class="sxs-lookup"><span data-stu-id="c887c-113">Create a Mailflow Transport Rule as follows:</span></span>

    - <span data-ttu-id="c887c-114">Ако подателят е "Извън организацията"</span><span class="sxs-lookup"><span data-stu-id="c887c-114">If the Sender is "Outside the Organization"</span></span>
    - <span data-ttu-id="c887c-115">Пренасочване на съобщението към Catchall@domain.com</span><span class="sxs-lookup"><span data-stu-id="c887c-115">Redirect the message to Catchall@domain.com</span></span>
    - <span data-ttu-id="c887c-116">Освен ако получателят е член на allusers@domain.com (Distribution Group съдържа всички членове)</span><span class="sxs-lookup"><span data-stu-id="c887c-116">Except if the recipient is a member of allusers@domain.com (Distribution Group contains all members)</span></span>
    - <span data-ttu-id="c887c-117">Уверете се, че да проверите дали новите пощенски кутии се добавят в динамична група за разпространение</span><span class="sxs-lookup"><span data-stu-id="c887c-117">Ensure to validate that new mailboxes are added into the Dynamic Distribution Group</span></span>
