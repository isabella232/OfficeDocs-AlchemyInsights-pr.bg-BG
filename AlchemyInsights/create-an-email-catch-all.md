---
title: Създаване на имейл за улова на всички
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
- "9001524"
- "3732"
ms.openlocfilehash: 262d2c6a7181d94094f3d840c4ba3ebd07000cf4
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: bg-BG
ms.lasthandoff: 09/14/2020
ms.locfileid: "47712975"
---
# <a name="create-an-email-catch-all"></a><span data-ttu-id="3a0af-102">Създаване на имейл за улова на всички</span><span class="sxs-lookup"><span data-stu-id="3a0af-102">Create an email catch all</span></span>

<span data-ttu-id="3a0af-103">Употребата на даден улов е силно обезкуражени.</span><span class="sxs-lookup"><span data-stu-id="3a0af-103">Use of a catch all is strongly discouraged.</span></span> <span data-ttu-id="3a0af-104">По-добре е да осигурите прескачане обратно към подателите, отдаващи съобщение, че съобщението не може да бъде доставено като адресирано, така че да могат да предприемат действия.</span><span class="sxs-lookup"><span data-stu-id="3a0af-104">It is better to provide a bounce back to the sender letting senders know their message could not be delivered as addressed so they can take action.</span></span> <span data-ttu-id="3a0af-105">Можете също да ограничите наблюдаваната пощенска кутия само за да улови преди това валидни имейл адреси.</span><span class="sxs-lookup"><span data-stu-id="3a0af-105">You can also limit the monitored mailbox to only catch formerly valid email addresses.</span></span> 

<span data-ttu-id="3a0af-106">Всеки улов на цялата пощенска кутия ще получи добра сделка за нежелана поща и евентуално може да се запълни, ако не се следи внимателно.</span><span class="sxs-lookup"><span data-stu-id="3a0af-106">Any catch all mailbox will receive a good deal of spam and may eventually fill if not closely monitored.</span></span> <span data-ttu-id="3a0af-107">(Има ограничения за получаване.)</span><span class="sxs-lookup"><span data-stu-id="3a0af-107">(There are receiving limits.)</span></span> 

<span data-ttu-id="3a0af-108">Ако решите да продължите, изпълнете следните стъпки:</span><span class="sxs-lookup"><span data-stu-id="3a0af-108">If you decide to proceed, follow these steps:</span></span>

1. <span data-ttu-id="3a0af-109">Създаване на динамична група за разпространение & включване на "всички типове получатели".</span><span class="sxs-lookup"><span data-stu-id="3a0af-109">Create a Dynamic Distribution Group & include "All Recipient Types."</span></span>

2. <span data-ttu-id="3a0af-110">Създайте специална пощенска кутия, за да уловите имейли, например catchall@domain.com.</span><span class="sxs-lookup"><span data-stu-id="3a0af-110">Create a dedicated Mailbox to catch emails, for example, catchall@domain.com.</span></span>

3. <span data-ttu-id="3a0af-111">За конкретен домейн Настройте DomainType на "InternalRelay".</span><span class="sxs-lookup"><span data-stu-id="3a0af-111">For the specific domain, set the DomainType to “InternalRelay”.</span></span> <span data-ttu-id="3a0af-112">Ако по-късно премахнете улова за всички, не забравяйте да зададете домейна да се върне към достоверен.</span><span class="sxs-lookup"><span data-stu-id="3a0af-112">If you later remove the catch all, be sure to set the domain back to Authoritative.</span></span>

4. <span data-ttu-id="3a0af-113">Създайте инструмента транспортно правило по следния начин:</span><span class="sxs-lookup"><span data-stu-id="3a0af-113">Create a Mailflow Transport Rule as follows:</span></span>

    - <span data-ttu-id="3a0af-114">Ако подателят е "извън организацията"</span><span class="sxs-lookup"><span data-stu-id="3a0af-114">If the Sender is "Outside the Organization"</span></span>
    - <span data-ttu-id="3a0af-115">Пренасочване на съобщението към Catchall@domain.com</span><span class="sxs-lookup"><span data-stu-id="3a0af-115">Redirect the message to Catchall@domain.com</span></span>
    - <span data-ttu-id="3a0af-116">Освен ако получателят е член на allusers@domain.com (групата за разпространение съдържа всички членове)</span><span class="sxs-lookup"><span data-stu-id="3a0af-116">Except if the recipient is a member of allusers@domain.com (Distribution Group contains all members)</span></span>
    - <span data-ttu-id="3a0af-117">Уверете се, че за да проверите дали новите пощенски кутии са добавени към динамичната група за разпространение</span><span class="sxs-lookup"><span data-stu-id="3a0af-117">Ensure to validate that new mailboxes are added into the Dynamic Distribution Group</span></span>
