---
title: Какво да направите, ако функциите на Azure не работят правилно в Microsoft Edge
ms.author: v-jmathew
author: v-jmathew
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004128"
- "7206"
ms.openlocfilehash: 463236bcd9ff480471604c992aa1ed1ed4ac2987
ms.sourcegitcommit: 2e4a5153e530bf15744a52e982eeb0d99757e9d2
ms.translationtype: MT
ms.contentlocale: bg-BG
ms.lasthandoff: 12/04/2020
ms.locfileid: "49583189"
---
# <a name="what-to-do-if-azure-features-dont-work-properly-in-microsoft-edge"></a><span data-ttu-id="4e30a-102">Какво да направите, ако функциите на Azure не работят правилно в Microsoft Edge</span><span class="sxs-lookup"><span data-stu-id="4e30a-102">What to do if Azure features don't work properly in Microsoft Edge</span></span>

<span data-ttu-id="4e30a-103">Microsoft Edge има [известни проблеми](https://go.microsoft.com/fwlink/?linkid=2140608) , които са свързани със зоните за защита, и може да засегне как потребителите на Azure влизат в центъра за администриране на Windows.</span><span class="sxs-lookup"><span data-stu-id="4e30a-103">Microsoft Edge has [known issues](https://go.microsoft.com/fwlink/?linkid=2140608) that are related to security zones and might affect how Azure users log in to Windows Admin Center.</span></span> <span data-ttu-id="4e30a-104">Ако имате проблеми с използването на функциите на Azure с Microsoft Edge, изпробвайте следните стъпки:</span><span class="sxs-lookup"><span data-stu-id="4e30a-104">If you're having trouble using Azure features with Microsoft Edge, try the following steps:</span></span>

1. <span data-ttu-id="4e30a-105">В менюто **Старт** Потърсете **Опции за интернет** и го изберете.</span><span class="sxs-lookup"><span data-stu-id="4e30a-105">In the **Start** menu, search for **Internet Options** and select it.</span></span>
2. <span data-ttu-id="4e30a-106">В диалоговия прозорец **свойства на интернет** отидете на раздела **защита** .</span><span class="sxs-lookup"><span data-stu-id="4e30a-106">In the **Internet Properties** dialog box, go to the **Security** tab.</span></span>
3. <span data-ttu-id="4e30a-107">Изберете зоната **надеждни сайтове** и след това изберете бутона **сайтове** .</span><span class="sxs-lookup"><span data-stu-id="4e30a-107">Select the **Trusted sites** zone and then select the **Sites** button.</span></span>
4. <span data-ttu-id="4e30a-108">В диалоговия прозорец **надеждни сайтове** Добавете URL адреса на шлюза, както [https://login.microsoftonline.com](https://login.microsoftonline.com) и и [https://login.live.com](https://login.live.com) след това изберете **Затвори**.</span><span class="sxs-lookup"><span data-stu-id="4e30a-108">In the **Trusted sites** dialog box, add your gateway URL as well as [https://login.microsoftonline.com](https://login.microsoftonline.com) and [https://login.live.com](https://login.live.com), and then select **Close**.</span></span>
5. <span data-ttu-id="4e30a-109">В диалоговия прозорец **свойства на интернет** отидете на раздела **поверителност** .</span><span class="sxs-lookup"><span data-stu-id="4e30a-109">In the **Internet Properties** dialog box, go to the **Privacy** tab.</span></span>
6. <span data-ttu-id="4e30a-110">В секцията за **блокиране на изскачащи** съобщения изберете **Настройки**.</span><span class="sxs-lookup"><span data-stu-id="4e30a-110">In the **Pop-up Blocker** section, select **Settings**.</span></span> <span data-ttu-id="4e30a-111">В диалоговия прозорец, който се отваря, добавете URL адреса на шлюза, както [https://login.microsoftonline.com](https://login.microsoftonline.com) и и [https://login.live.com](https://login.live.com) след това изберете **Затвори**.</span><span class="sxs-lookup"><span data-stu-id="4e30a-111">In the dialog box that opens, add your gateway URL as well as [https://login.microsoftonline.com](https://login.microsoftonline.com) and [https://login.live.com](https://login.live.com), and then select **Close**.</span></span>
