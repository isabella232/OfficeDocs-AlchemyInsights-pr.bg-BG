---
title: Не можете да задавате или преглеждате правилата за AllowSelfServicePurchase
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
- "9001212"
- "3526"
ms.openlocfilehash: 5ec16b3071f95ef52af2771e95137116222a3c5b
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: bg-BG
ms.lasthandoff: 09/14/2020
ms.locfileid: "47735188"
---
# <a name="unable-to-set-or-view-the-allowselfservicepurchase-policy"></a><span data-ttu-id="0e590-102">Не можете да задавате или преглеждате правилата за AllowSelfServicePurchase</span><span class="sxs-lookup"><span data-stu-id="0e590-102">Unable to set or view the AllowSelfServicePurchase policy</span></span>

<span data-ttu-id="0e590-103">Когато се опитвате да зададете или видите правилата за AllowSelfServicePurchase, получавате следното съобщение за грешка:</span><span class="sxs-lookup"><span data-stu-id="0e590-103">When attempting to set or view the AllowSelfServicePurchase policy, you receive the following error message:</span></span>

<span data-ttu-id="0e590-104">*HandleError: неуспех при извличане на правилата за продукти с PolicyId "AllowSelfServicePurchase", ErrorMessage – основната връзка е затворена: неочаквана грешка при изпращане.*</span><span class="sxs-lookup"><span data-stu-id="0e590-104">*HandleError : Failed to retrieve product policy with PolicyId 'AllowSelfServicePurchase', ErrorMessage - The underlying connection was closed: An unexpected error occurred on a send.*</span></span>

<span data-ttu-id="0e590-105">Това може да се дължи на по-стара версия на защитата на транспортния слой (TLS).</span><span class="sxs-lookup"><span data-stu-id="0e590-105">This may be due to an older version of Transport Layer Security (TLS).</span></span> <span data-ttu-id="0e590-106">За да свържете услугата MSCommerce, трябва да използвате TLS 1,2 или по-нова версия.</span><span class="sxs-lookup"><span data-stu-id="0e590-106">To connect the MSCommerce service, you need to use TLS 1.2 or greater.</span></span>  

<span data-ttu-id="0e590-107">Изпробвайте следните стъпки, за да разрешите/зададете TLS протокола към 1,2, проверете и опитайте отново.</span><span class="sxs-lookup"><span data-stu-id="0e590-107">Try the following steps to enable/set the TLS protocol to 1.2, verify, and retry.</span></span>
 1. <span data-ttu-id="0e590-108">В командния прозорец на PowerShell (PS C: \) Въведете следната команда, за да зададете ПРОТОКОЛА TLS към версия 1,2:</span><span class="sxs-lookup"><span data-stu-id="0e590-108">At the PowerShell command prompt (PS C:\) enter the following command to set the TLS protocol to version 1.2:</span></span>

    `[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12`

2. <span data-ttu-id="0e590-109">Проверете използвания TLS протокол (и) със следната команда:</span><span class="sxs-lookup"><span data-stu-id="0e590-109">Verify the TLS protocol(s) in use, with the following command:</span></span>

    `[Net.ServicePointManager]::SecurityProtocol` 

3. <span data-ttu-id="0e590-110">Опитайте отново с командите получаване или актуализиране, ако е необходимо.</span><span class="sxs-lookup"><span data-stu-id="0e590-110">Retry the Get or Update commands as needed.</span></span>

