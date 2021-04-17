---
title: Създаване на улов на имейл до всички
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
- "9001524"
- "3732"
ms.openlocfilehash: 2b9131a620139a93ddb844fd49d8fa2ed68e52c2
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: bg-BG
ms.lasthandoff: 04/15/2021
ms.locfileid: "51816189"
---
# <a name="create-an-email-catch-all"></a><span data-ttu-id="3ad29-102">Създаване на улов на имейл до всички</span><span class="sxs-lookup"><span data-stu-id="3ad29-102">Create an email catch all</span></span>

<span data-ttu-id="3ad29-103">Използването на уловка е силно обезкуражено.</span><span class="sxs-lookup"><span data-stu-id="3ad29-103">Use of a catch all is strongly discouraged.</span></span> <span data-ttu-id="3ad29-104">По-добре е да предоставите отпадане обратно на подателя, което позволява на подателите да знаят, че съобщението им не може да бъде доставено като адресирано, така че те да могат да предприемат действия.</span><span class="sxs-lookup"><span data-stu-id="3ad29-104">It is better to provide a bounce back to the sender letting senders know their message could not be delivered as addressed so they can take action.</span></span> <span data-ttu-id="3ad29-105">Можете също да ограничите наблюдаваната пощенска кутия, за да хванете само бивши валидни имейл адреси.</span><span class="sxs-lookup"><span data-stu-id="3ad29-105">You can also limit the monitored mailbox to only catch formerly valid email addresses.</span></span> 

<span data-ttu-id="3ad29-106">Всяка уловка на всички пощенски кутии ще получи добра сделка със спам и в крайна сметка може да запълни, ако не се следи отблизо.</span><span class="sxs-lookup"><span data-stu-id="3ad29-106">Any catch all mailbox will receive a good deal of spam and may eventually fill if not closely monitored.</span></span> <span data-ttu-id="3ad29-107">(Има ограничения за получаване.)</span><span class="sxs-lookup"><span data-stu-id="3ad29-107">(There are receiving limits.)</span></span> 

<span data-ttu-id="3ad29-108">Ако решите да продължите, изпълнете следните стъпки:</span><span class="sxs-lookup"><span data-stu-id="3ad29-108">If you decide to proceed, follow these steps:</span></span>

1. <span data-ttu-id="3ad29-109">Създаване на динамична група за & включва "Всички типове получатели".</span><span class="sxs-lookup"><span data-stu-id="3ad29-109">Create a Dynamic Distribution Group & include "All Recipient Types."</span></span>

2. <span data-ttu-id="3ad29-110">Създайте специална пощенска кутия, за да уловите имейли, например catchall@domain.com.</span><span class="sxs-lookup"><span data-stu-id="3ad29-110">Create a dedicated Mailbox to catch emails, for example, catchall@domain.com.</span></span>

3. <span data-ttu-id="3ad29-111">За конкретния домейн задайте DomainType на "InternalRelay".</span><span class="sxs-lookup"><span data-stu-id="3ad29-111">For the specific domain, set the DomainType to “InternalRelay”.</span></span> <span data-ttu-id="3ad29-112">Ако по-късно премахнете всички уловки, не забравяйте да зададете домейна обратно на Достовителен.</span><span class="sxs-lookup"><span data-stu-id="3ad29-112">If you later remove the catch all, be sure to set the domain back to Authoritative.</span></span>

4. <span data-ttu-id="3ad29-113">Създаване на транспортно правило за пощенски поток по следния начин:</span><span class="sxs-lookup"><span data-stu-id="3ad29-113">Create a Mailflow Transport Rule as follows:</span></span>

    - <span data-ttu-id="3ad29-114">Ако подателят е "Извън организацията"</span><span class="sxs-lookup"><span data-stu-id="3ad29-114">If the Sender is "Outside the Organization"</span></span>
    - <span data-ttu-id="3ad29-115">Пренасочване на съобщението към Catchall@domain.com</span><span class="sxs-lookup"><span data-stu-id="3ad29-115">Redirect the message to Catchall@domain.com</span></span>
    - <span data-ttu-id="3ad29-116">Освен ако получателят е член на allusers@domain.com (групата за разпространение съдържа всички членове)</span><span class="sxs-lookup"><span data-stu-id="3ad29-116">Except if the recipient is a member of allusers@domain.com (Distribution Group contains all members)</span></span>
    - <span data-ttu-id="3ad29-117">Уверете се, че сте проверили, че новите пощенски кутии са добавени в динамичната група за разпространение</span><span class="sxs-lookup"><span data-stu-id="3ad29-117">Ensure to validate that new mailboxes are added into the Dynamic Distribution Group</span></span>
