---
title: Как да забраните външни групи
ms.author: pebaum
author: pebaum
ms.date: 12/17/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.assetid: 4e429507-039b-410e-a994-54b443d4e91e
ms.openlocfilehash: 09d8b134a4e99912301aa92c2e989fec9dd30a7b
ms.sourcegitcommit: 0ae6cbb8cf2836da98300767ed81b411d6551bee
ms.translationtype: MT
ms.contentlocale: bg-BG
ms.lasthandoff: 01/30/2019
ms.locfileid: "29656376"
---
# <a name="how-to-disable-external-groups"></a><span data-ttu-id="dc7e9-102">Как да забраните външни групи</span><span class="sxs-lookup"><span data-stu-id="dc7e9-102">How to disable External Groups</span></span>

<span data-ttu-id="dc7e9-p101">Хленча външни съобщения се прилага обмен транспортни правила (ETRs) набор от проактивни контрол, за да предотвратите компанията информация се споделя. За да ограничите потребителите да създават външни групи, трябва да конфигурирате борса транспортно правило (ЕТП) и след това да конфигурирате вайкам да използвате Exchange транспортното правило да блокира външни съобщения.</span><span class="sxs-lookup"><span data-stu-id="dc7e9-p101">Yammer external messaging applies Exchange Transport Rules (ETRs), a set of proactive controls to prevent company information from being shared. In order to restrict users from creating external groups, you need to configure an Exchange transport rule (ETR), and then configure Yammer to use the Exchange Transport rule to block external messaging.</span></span> 
  
<span data-ttu-id="dc7e9-105">След като сте създали правило в центъра за администриране на Exchange Online, следвайте тези стъпки, за да зададете ETR да приложите в вайкам:</span><span class="sxs-lookup"><span data-stu-id="dc7e9-105">Once you have created a rule in Exchange Online admin center, follow these steps to set ETR to apply in Yammer:</span></span>
  
- <span data-ttu-id="dc7e9-106">Влезте в вайкам като проверени администратор и в **хленча център за администриране**, преминете към C **ontent и сигурност \> сигурност настройки.**</span><span class="sxs-lookup"><span data-stu-id="dc7e9-106">Log on to Yammer as a verified admin, and in the **Yammer admin center**, go to C **ontent and Security \> Security Settings.**</span></span>
    
- <span data-ttu-id="dc7e9-107">Под **Външни съобщения**, изберете **прилага правилата за транспорт на онлайн бюро вашия Exchange (ETRs) в вайкам.**</span><span class="sxs-lookup"><span data-stu-id="dc7e9-107">Under **External Messaging**, select **Enforce your Exchange Online Exchange Transport Rules (ETRs) in Yammer.**</span></span>
    
- <span data-ttu-id="dc7e9-108">Изберете **Запиши**.</span><span class="sxs-lookup"><span data-stu-id="dc7e9-108">Choose **Save**.</span></span> 
    
<span data-ttu-id="dc7e9-109">За повече информация вижте [контрол външни съобщения в вайкам мрежа с обмен транспортни правила](https://support.office.com/article/Control-external-messaging-in-a-Yammer-network-with-Exchange-Transport-Rules-f8fd6403-c8f3-4307-9230-65304d6000d9)</span><span class="sxs-lookup"><span data-stu-id="dc7e9-109">For more information, see [Control external messaging in a Yammer network with Exchange Transport rules](https://support.office.com/article/Control-external-messaging-in-a-Yammer-network-with-Exchange-Transport-Rules-f8fd6403-c8f3-4307-9230-65304d6000d9)</span></span>
  

