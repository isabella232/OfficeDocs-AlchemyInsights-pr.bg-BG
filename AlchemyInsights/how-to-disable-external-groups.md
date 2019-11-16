---
title: Как да забраните външни групи
ms.author: pebaum
author: pebaum
ms.date: 12/17/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "966"
- "6000006"
ms.assetid: 4e429507-039b-410e-a994-54b443d4e91e
ms.openlocfilehash: b2328ea85d3ff6ec722cc56d8a46395d8438f79c
ms.sourcegitcommit: b43f77221f47b50c41197a448a9c26c423ce1ad5
ms.translationtype: MT
ms.contentlocale: bg-BG
ms.lasthandoff: 11/15/2019
ms.locfileid: "36739482"
---
# <a name="how-to-disable-external-groups"></a><span data-ttu-id="a2aa3-102">Как да забраните външни групи</span><span class="sxs-lookup"><span data-stu-id="a2aa3-102">How to disable External Groups</span></span>

<span data-ttu-id="a2aa3-103">Yammer външни съобщения се прилага Exchange транспортни правила (ETRs), набор от проактивни контроли за предотвратяване на споделяне на фирмени информация.</span><span class="sxs-lookup"><span data-stu-id="a2aa3-103">Yammer external messaging applies Exchange Transport Rules (ETRs), a set of proactive controls to prevent company information from being shared.</span></span> <span data-ttu-id="a2aa3-104">За да ограничите потребителите от създаване на външни групи, трябва да конфигурирате транспорт правило за Exchange (ETR) и след това конфигурирайте Yammer да използвате Exchange транспорт правило за блокиране на външни съобщения.</span><span class="sxs-lookup"><span data-stu-id="a2aa3-104">In order to restrict users from creating external groups, you need to configure an Exchange transport rule (ETR), and then configure Yammer to use the Exchange Transport rule to block external messaging.</span></span>
  
<span data-ttu-id="a2aa3-105">След като сте създали правило в центъра за администриране на Exchange Online, изпълнете следните стъпки, за да зададете ETR да приложите в Yammer:</span><span class="sxs-lookup"><span data-stu-id="a2aa3-105">Once you have created a rule in Exchange Online admin center, follow these steps to set ETR to apply in Yammer:</span></span>
  
- <span data-ttu-id="a2aa3-106">Влезте в Yammer като проверен администратор и в центъра за администриране на **yammer**отидете на C **съдържание и настройките за защита на \> защитата.**</span><span class="sxs-lookup"><span data-stu-id="a2aa3-106">Log on to Yammer as a verified admin, and in the **Yammer admin center**, go to C **Content and Security \> Security Settings.**</span></span>

- <span data-ttu-id="a2aa3-107">Под **външни съобщения**изберете **прилагане на Exchange Online Exchange правила за транспорт (etrs) в Yammer.**</span><span class="sxs-lookup"><span data-stu-id="a2aa3-107">Under **External Messaging**, select **Enforce your Exchange Online Exchange Transport Rules (ETRs) in Yammer.**</span></span>

- <span data-ttu-id="a2aa3-108">Изберете **Запиши**.</span><span class="sxs-lookup"><span data-stu-id="a2aa3-108">Choose **Save**.</span></span>

<span data-ttu-id="a2aa3-109">За повече информация вижте [забраняване на външни съобщения в Yammer мрежа](https://docs.microsoft.com/yammer/work-with-external-users/disable-external-messaging).</span><span class="sxs-lookup"><span data-stu-id="a2aa3-109">For more information, see [Disable external messaging in a Yammer network](https://docs.microsoft.com/yammer/work-with-external-users/disable-external-messaging).</span></span>
  