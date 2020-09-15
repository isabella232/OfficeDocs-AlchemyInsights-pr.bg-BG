---
title: Как да забраните външни групи
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "966"
- "6000006"
ms.assetid: 4e429507-039b-410e-a994-54b443d4e91e
ms.openlocfilehash: f7a1bbda3a54d2662bdfe21cda961c32456edb82
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: bg-BG
ms.lasthandoff: 09/14/2020
ms.locfileid: "47704117"
---
# <a name="how-to-disable-external-groups"></a><span data-ttu-id="710ba-102">Как да забраните външни групи</span><span class="sxs-lookup"><span data-stu-id="710ba-102">How to disable External Groups</span></span>

<span data-ttu-id="710ba-103">Във външните съобщения на Yammer се прилагат транспортни правила на Exchange (ETR) – набор от proactive контроли за предотвратяване на споделянето на информация за фирмата.</span><span class="sxs-lookup"><span data-stu-id="710ba-103">Yammer external messaging applies Exchange Transport Rules (ETRs), a set of proactive controls to prevent company information from being shared.</span></span> <span data-ttu-id="710ba-104">За да ограничите потребителите при създаването на външни групи, трябва да конфигурирате транспортно правило на Exchange (ETR) и след това да конфигурирате Yammer, за да използвате транспортното правило на Exchange, за да блокирате външни съобщения.</span><span class="sxs-lookup"><span data-stu-id="710ba-104">In order to restrict users from creating external groups, you need to configure an Exchange transport rule (ETR), and then configure Yammer to use the Exchange Transport rule to block external messaging.</span></span>
  
<span data-ttu-id="710ba-105">След като създадете правило в центъра за администриране на Exchange Online, изпълнете следните стъпки, за да зададете ETR, което да приложите в Yammer:</span><span class="sxs-lookup"><span data-stu-id="710ba-105">Once you have created a rule in Exchange Online admin center, follow these steps to set ETR to apply in Yammer:</span></span>
  
- <span data-ttu-id="710ba-106">Влезте в Yammer като проверен администратор и в центъра за администриране на **Yammer**отидете на настройки за защита на **съдържание и защита \> .**</span><span class="sxs-lookup"><span data-stu-id="710ba-106">Log on to Yammer as a verified admin, and in the **Yammer admin center**, go to C **Content and Security \> Security Settings.**</span></span>

- <span data-ttu-id="710ba-107">Под **външни съобщения**изберете **налагане на вашите транспортни правила на Exchange Online за транспорт (ETR) в Yammer.**</span><span class="sxs-lookup"><span data-stu-id="710ba-107">Under **External Messaging**, select **Enforce your Exchange Online Exchange Transport Rules (ETRs) in Yammer.**</span></span>

- <span data-ttu-id="710ba-108">Изберете **Запиши**.</span><span class="sxs-lookup"><span data-stu-id="710ba-108">Choose **Save**.</span></span>

<span data-ttu-id="710ba-109">За повече информация вижте [забраняване на външни съобщения в мрежа на Yammer](https://docs.microsoft.com/yammer/work-with-external-users/disable-external-messaging).</span><span class="sxs-lookup"><span data-stu-id="710ba-109">For more information, see [Disable external messaging in a Yammer network](https://docs.microsoft.com/yammer/work-with-external-users/disable-external-messaging).</span></span>
  