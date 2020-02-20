---
title: Не може да се зададе или да се визуализира правилата на AllowSelfServicePurchase
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9001212"
- "3526"
ms.openlocfilehash: 587a05cccbc71a970d4bd7723bff0df0c3b64ccc
ms.sourcegitcommit: 2a9d059262c07c33f9a740b3da4e6e3366b2f925
ms.translationtype: MT
ms.contentlocale: bg-BG
ms.lasthandoff: 02/20/2020
ms.locfileid: "42158548"
---
# <a name="unable-to-set-or-view-the-allowselfservicepurchase-policy"></a><span data-ttu-id="85e61-102">Не може да се зададе или да се визуализира правилата на AllowSelfServicePurchase</span><span class="sxs-lookup"><span data-stu-id="85e61-102">Unable to set or view the AllowSelfServicePurchase policy</span></span>

<span data-ttu-id="85e61-103">При опит за задаване или преглед на AllowSelfServicePurchase политика, получавате следното съобщение за грешка:</span><span class="sxs-lookup"><span data-stu-id="85e61-103">When attempting to set or view the AllowSelfServicePurchase policy, you receive the following error message:</span></span>

<span data-ttu-id="85e61-104">*HandleError: Неуспешно извличане на продуктови правила с PolicyId "AllowSelfServicePurchase", съобщение за грешка - основната връзка е прекъсната: възникна неочаквана грешка при изпращане.*</span><span class="sxs-lookup"><span data-stu-id="85e61-104">*HandleError : Failed to retrieve product policy with PolicyId 'AllowSelfServicePurchase', ErrorMessage - The underlying connection was closed: An unexpected error occurred on a send.*</span></span>

<span data-ttu-id="85e61-105">Това може да се дължи на по-стара версия на защита на транспортния слой (TLS).</span><span class="sxs-lookup"><span data-stu-id="85e61-105">This may be due to an older version of Transport Layer Security (TLS).</span></span> <span data-ttu-id="85e61-106">За да свържете MSCommerce услугата, трябва да използвате TLS 1.2 или по-нова версия.</span><span class="sxs-lookup"><span data-stu-id="85e61-106">To connect the MSCommerce service, you need to use TLS 1.2 or greater.</span></span>  

<span data-ttu-id="85e61-107">Опитайте следните стъпки, за да разрешите/зададете TLS протокола 1.2, проверете и опитайте отново.</span><span class="sxs-lookup"><span data-stu-id="85e61-107">Try the following steps to enable/set the TLS protocol to 1.2, verify, and retry.</span></span>
 1. <span data-ttu-id="85e61-108">В командния ред на PowerShell\) (PS C: въведете следната команда, за да зададете протокола TLS версия 1.2:</span><span class="sxs-lookup"><span data-stu-id="85e61-108">At the PowerShell command prompt (PS C:\) enter the following command to set the TLS protocol to version 1.2:</span></span>

    `[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12`

2. <span data-ttu-id="85e61-109">Проверете TLS протокола, които се използват, със следната команда:</span><span class="sxs-lookup"><span data-stu-id="85e61-109">Verify the TLS protocol(s) in use, with the following command:</span></span>

    `[Net.ServicePointManager]::SecurityProtocol` 

3. <span data-ttu-id="85e61-110">Опитайте отново да получите или актуализирате командите, ако е необходимо.</span><span class="sxs-lookup"><span data-stu-id="85e61-110">Retry the Get or Update commands as needed.</span></span>

