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
ms.openlocfilehash: 4683a71438ec31f9e9211404a9c66c4e45e0e1df
ms.sourcegitcommit: 1d98db8acb9959aba3b5e308a567ade6b62da56c
ms.translationtype: MT
ms.contentlocale: bg-BG
ms.lasthandoff: 08/22/2019
ms.locfileid: "36540890"
---
# <a name="how-to-disable-external-groups"></a><span data-ttu-id="79699-102">Как да забраните външни групи</span><span class="sxs-lookup"><span data-stu-id="79699-102">How to disable External Groups</span></span>

<span data-ttu-id="79699-103">Хленча външни съобщения се прилага обмен транспортни правила (ETRs) набор от проактивни контрол, за да предотвратите компанията информация се споделя.</span><span class="sxs-lookup"><span data-stu-id="79699-103">Yammer external messaging applies Exchange Transport Rules (ETRs), a set of proactive controls to prevent company information from being shared.</span></span> <span data-ttu-id="79699-104">За да ограничите потребителите да създават външни групи, трябва да конфигурирате борса транспортно правило (ЕТП) и след това да конфигурирате вайкам да използвате Exchange транспортното правило да блокира външни съобщения.</span><span class="sxs-lookup"><span data-stu-id="79699-104">In order to restrict users from creating external groups, you need to configure an Exchange transport rule (ETR), and then configure Yammer to use the Exchange Transport rule to block external messaging.</span></span>
  
<span data-ttu-id="79699-105">След като сте създали правило в центъра за администриране на Exchange Online, следвайте тези стъпки, за да зададете ETR да приложите в вайкам:</span><span class="sxs-lookup"><span data-stu-id="79699-105">Once you have created a rule in Exchange Online admin center, follow these steps to set ETR to apply in Yammer:</span></span>
  
- <span data-ttu-id="79699-106">Влезте в вайкам като проверени администратор и в **хленча център за администриране**, преминете към C **съдържание и сигурност \> сигурност настройки.**</span><span class="sxs-lookup"><span data-stu-id="79699-106">Log on to Yammer as a verified admin, and in the **Yammer admin center**, go to C **Content and Security \> Security Settings.**</span></span>

- <span data-ttu-id="79699-107">Под **Външни съобщения**, изберете **прилага правилата за транспорт на онлайн бюро вашия Exchange (ETRs) в вайкам.**</span><span class="sxs-lookup"><span data-stu-id="79699-107">Under **External Messaging**, select **Enforce your Exchange Online Exchange Transport Rules (ETRs) in Yammer.**</span></span>

- <span data-ttu-id="79699-108">Изберете **Запиши**.</span><span class="sxs-lookup"><span data-stu-id="79699-108">Choose **Save**.</span></span>

<span data-ttu-id="79699-109">За повече информация вижте [контрол външни съобщения в вайкам мрежа с обмен транспортни правила](https://support.office.com/article/Control-external-messaging-in-a-Yammer-network-with-Exchange-Transport-Rules-f8fd6403-c8f3-4307-9230-65304d6000d9)</span><span class="sxs-lookup"><span data-stu-id="79699-109">For more information, see [Control external messaging in a Yammer network with Exchange Transport rules](https://support.office.com/article/Control-external-messaging-in-a-Yammer-network-with-Exchange-Transport-Rules-f8fd6403-c8f3-4307-9230-65304d6000d9)</span></span>
  