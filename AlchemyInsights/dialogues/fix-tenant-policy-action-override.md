---
title: Коригиране на правила за клиент (отмяна на действие)
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
ms.openlocfilehash: bc7ad8acd86c9d5b2f99ffdc6fe8a8b53e1fcb8b
ms.sourcegitcommit: 60c504f3ac187eaf1141b3ba701d9e0633bdd968
ms.translationtype: MT
ms.contentlocale: bg-BG
ms.lasthandoff: 03/08/2021
ms.locfileid: "50692623"
---
# <a name="fix-tenant-policy-action-override"></a><span data-ttu-id="8291c-102">Коригиране на правила за клиент (отмяна на действие)</span><span class="sxs-lookup"><span data-stu-id="8291c-102">Fix Tenant policy (action override)</span></span>

<span data-ttu-id="8291c-103">Политиката за анти-спам във вашия клиент е засегнала това съобщение.</span><span class="sxs-lookup"><span data-stu-id="8291c-103">An anti-spam policy in your tenant affected this message.</span></span> <span data-ttu-id="8291c-104">За да прегледате правилата, направете следното:</span><span class="sxs-lookup"><span data-stu-id="8291c-104">To review the policy, do the following:</span></span>

1. <span data-ttu-id="8291c-105">Отидете в центъра за администриране на [& на Office 365](https://go.microsoft.com/fwlink/p/?linkid=2077143)и след това отидете в раздела за правила за **управление на заплахите**  >    >  [](https://go.microsoft.com/fwlink/?linkid=2101518).</span><span class="sxs-lookup"><span data-stu-id="8291c-105">Go to the [Office 365 Security & Compliance Center](https://go.microsoft.com/fwlink/p/?linkid=2077143), and then go to **Threat management** > **Policy** > [Anti-spam](https://go.microsoft.com/fwlink/?linkid=2101518).</span></span>
2. <span data-ttu-id="8291c-106">Проверете дали **Източникът на правилата** указва следното:  **Add-XHeader/ModifySubject/пренасочване/изтриване/без действие/СК съобщение**</span><span class="sxs-lookup"><span data-stu-id="8291c-106">Check to see if **Policy source** indicates the following:  **Add-Xheader/ModifySubject/Redirect/Delete/No action/ BCC message**</span></span>

    <span data-ttu-id="8291c-107">Ако е така, в раздела по **избор** Проверете настройките за правилата, които са засегнали съобщението.</span><span class="sxs-lookup"><span data-stu-id="8291c-107">If so, on the **Custom** tab, check the settings of the policy that affected the message.</span></span> <span data-ttu-id="8291c-108">Възможно е **стандартните настройки** , приложени към всички клиенти на Exchange Online Protection, да са засегнали съобщението.</span><span class="sxs-lookup"><span data-stu-id="8291c-108">It's possible that the **Standard settings** applied to all Exchange Online Protection customers affected the message.</span></span>

<span data-ttu-id="8291c-109">За повече информация за конфигурирането на правилата за филтриране на нежелана поща вижте [Конфигуриране на правилата за филтриране на нежелана поща](https://go.microsoft.com/fwlink/?linkid=2101431).</span><span class="sxs-lookup"><span data-stu-id="8291c-109">For more information on configuring spam filter policies, see [Configure your spam filter policies](https://go.microsoft.com/fwlink/?linkid=2101431).</span></span>
