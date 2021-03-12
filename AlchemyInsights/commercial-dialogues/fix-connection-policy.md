---
title: Коригиране на правила за връзки
ms.author: v-jmathew
author: v-jmathew
manager: dansimp
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000760"
- "7391"
ms.openlocfilehash: 0b6286350e706e493f6d30b7978aacedc02daff5
ms.sourcegitcommit: 6312ee31561db36104f32282d019d069ede69174
ms.translationtype: MT
ms.contentlocale: bg-BG
ms.lasthandoff: 03/11/2021
ms.locfileid: "50743866"
---
# <a name="fix-connection-policy"></a><span data-ttu-id="d4eaa-102">Коригиране на правила за връзки</span><span class="sxs-lookup"><span data-stu-id="d4eaa-102">Fix connection policy</span></span>

<span data-ttu-id="d4eaa-103">Имейлът е маркиран като безопасен и е предоставен към папката "Входящи" на потребителя, тъй като IP адресът за изпращане е отбелязан като безопасен в правилата за филтриране на връзката.</span><span class="sxs-lookup"><span data-stu-id="d4eaa-103">The email was marked safe and delivered to the user's inbox because the sending IP address was marked safe in the Connection Filter policy.</span></span> <span data-ttu-id="d4eaa-104">За да прегледате правилата, направете следното:</span><span class="sxs-lookup"><span data-stu-id="d4eaa-104">To review the policy, do the following:</span></span>

1. <span data-ttu-id="d4eaa-105">Отидете в центъра за администриране на [& на Office 365](https://go.microsoft.com/fwlink/p/?linkid=2077143)и след това отидете в раздела за правила за **управление на заплахите**  >    >  [](https://go.microsoft.com/fwlink/?linkid=2101518).</span><span class="sxs-lookup"><span data-stu-id="d4eaa-105">Go to the [Office 365 Security & Compliance Center](https://go.microsoft.com/fwlink/p/?linkid=2077143), and then go to **Threat management** > **Policy** > [Anti-spam](https://go.microsoft.com/fwlink/?linkid=2101518).</span></span>
2. <span data-ttu-id="d4eaa-106">В раздела по **избор** изберете правилата за **филтриране на връзката** и след това изберете **Редактиране на правила**.</span><span class="sxs-lookup"><span data-stu-id="d4eaa-106">On the **Custom** tab, select the **Connection filter policy**, and then select **Edit policy**.</span></span>
3. <span data-ttu-id="d4eaa-107">Преглед на списъка с **разрешени IP адреси** .</span><span class="sxs-lookup"><span data-stu-id="d4eaa-107">Review the **IP Allow** list.</span></span> <span data-ttu-id="d4eaa-108">Вижте дали е разрешен **безопасен списък** .</span><span class="sxs-lookup"><span data-stu-id="d4eaa-108">See if **Safe list** is enabled.</span></span>

    > [!NOTE]
    > <span data-ttu-id="d4eaa-109">Microsoft се присъединява към други източници на надеждни податели.</span><span class="sxs-lookup"><span data-stu-id="d4eaa-109">Microsoft subscribes to third-party sources of trusted senders.</span></span> <span data-ttu-id="d4eaa-110">Ако е разрешен **безопасен списък** , тези надеждни податели не са маркирани по погрешка като нежелана поща.</span><span class="sxs-lookup"><span data-stu-id="d4eaa-110">If **Safe list** is enabled, these trusted senders aren't mistakenly marked as spam.</span></span> <span data-ttu-id="d4eaa-111">Препоръчвам избирането на тази опция, тъй като това ще намали броя на неверните положителни резултати (хубава поща, която е класифицирана като спам), която получавате.</span><span class="sxs-lookup"><span data-stu-id="d4eaa-111">I recommend selecting this option, because it will reduce the number of false positives (good mail that's classified as spam) that you receive.</span></span>
