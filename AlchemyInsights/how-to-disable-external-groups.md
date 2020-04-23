---
title: Как да забраните външни групи
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "966"
- "6000006"
ms.assetid: 4e429507-039b-410e-a994-54b443d4e91e
ms.openlocfilehash: 2159feb4aa3999072de57d76790a2959c7355976
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: bg-BG
ms.lasthandoff: 04/22/2020
ms.locfileid: "43720757"
---
# <a name="how-to-disable-external-groups"></a><span data-ttu-id="a2f0b-102">Как да забраните външни групи</span><span class="sxs-lookup"><span data-stu-id="a2f0b-102">How to disable External Groups</span></span>

<span data-ttu-id="a2f0b-103">Yammer външни съобщения прилага Exchange транспортни правила (ETRs), набор от проактивни контроли за предотвратяване на споделянето на информация за фирмата.</span><span class="sxs-lookup"><span data-stu-id="a2f0b-103">Yammer external messaging applies Exchange Transport Rules (ETRs), a set of proactive controls to prevent company information from being shared.</span></span> <span data-ttu-id="a2f0b-104">За да ограничите потребителите от създаване на външни групи, трябва да конфигурирате Exchange транспортно правило (ETR) и след това конфигурирате Yammer да използва Exchange транспорт правило за блокиране на външни съобщения.</span><span class="sxs-lookup"><span data-stu-id="a2f0b-104">In order to restrict users from creating external groups, you need to configure an Exchange transport rule (ETR), and then configure Yammer to use the Exchange Transport rule to block external messaging.</span></span>
  
<span data-ttu-id="a2f0b-105">След като сте създали правило в центъра за администриране на Exchange Online, изпълнете следните стъпки, за да зададете ETR да се прилагат в Yammer:</span><span class="sxs-lookup"><span data-stu-id="a2f0b-105">Once you have created a rule in Exchange Online admin center, follow these steps to set ETR to apply in Yammer:</span></span>
  
- <span data-ttu-id="a2f0b-106">Влезте в Yammer като проверен администратор и в центъра за администриране на **Yammer**отидете на C **съдържание и \> сигурност настройки.**</span><span class="sxs-lookup"><span data-stu-id="a2f0b-106">Log on to Yammer as a verified admin, and in the **Yammer admin center**, go to C **Content and Security \> Security Settings.**</span></span>

- <span data-ttu-id="a2f0b-107">Под **Външни съобщения**изберете Прилагане на exchange Online Exchange транспорт правила **(ETRs) в Yammer.**</span><span class="sxs-lookup"><span data-stu-id="a2f0b-107">Under **External Messaging**, select **Enforce your Exchange Online Exchange Transport Rules (ETRs) in Yammer.**</span></span>

- <span data-ttu-id="a2f0b-108">Изберете **Записване**.</span><span class="sxs-lookup"><span data-stu-id="a2f0b-108">Choose **Save**.</span></span>

<span data-ttu-id="a2f0b-109">За повече информация вижте [Забраняване на външни съобщения в yammer мрежа](https://docs.microsoft.com/yammer/work-with-external-users/disable-external-messaging).</span><span class="sxs-lookup"><span data-stu-id="a2f0b-109">For more information, see [Disable external messaging in a Yammer network](https://docs.microsoft.com/yammer/work-with-external-users/disable-external-messaging).</span></span>
  