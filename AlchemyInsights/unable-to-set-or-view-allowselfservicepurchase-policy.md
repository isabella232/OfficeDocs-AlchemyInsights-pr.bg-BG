---
title: Правилата allowSelfServicePurchase не могат да се задават или преглеждат
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9001212"
- "3526"
ms.openlocfilehash: 8dac2bdc20905cf37fc30317d9b371bfd755f452
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: bg-BG
ms.lasthandoff: 04/15/2021
ms.locfileid: "51826080"
---
# <a name="unable-to-set-or-view-the-allowselfservicepurchase-policy"></a><span data-ttu-id="3c646-102">Правилата allowSelfServicePurchase не могат да се задават или преглеждат</span><span class="sxs-lookup"><span data-stu-id="3c646-102">Unable to set or view the AllowSelfServicePurchase policy</span></span>

<span data-ttu-id="3c646-103">Когато се опитвате да зададете или прегледате правилата allowSelfServicePurchase, получавате следното съобщение за грешка:</span><span class="sxs-lookup"><span data-stu-id="3c646-103">When attempting to set or view the AllowSelfServicePurchase policy, you receive the following error message:</span></span>

<span data-ttu-id="3c646-104">*МанипулаторError: Неуспешно извличане на продуктови правила с PolicyId "AllowSelfServicePurchase", ErrorMessage – базовата връзка е затворена: Възникна неочаквана грешка при изпращане.*</span><span class="sxs-lookup"><span data-stu-id="3c646-104">*HandleError : Failed to retrieve product policy with PolicyId 'AllowSelfServicePurchase', ErrorMessage - The underlying connection was closed: An unexpected error occurred on a send.*</span></span>

<span data-ttu-id="3c646-105">Това може да се дължи на по-стара версия на защитата на транспортния слой (TLS).</span><span class="sxs-lookup"><span data-stu-id="3c646-105">This may be due to an older version of Transport Layer Security (TLS).</span></span> <span data-ttu-id="3c646-106">За да свържете услугата MSCommerce, трябва да използвате TLS 1.2 или по-нова версия.</span><span class="sxs-lookup"><span data-stu-id="3c646-106">To connect the MSCommerce service, you need to use TLS 1.2 or greater.</span></span>  

<span data-ttu-id="3c646-107">Опитайте следните стъпки, за да разрешите/зададете TLS протокола на 1.2, проверете и опитайте отново.</span><span class="sxs-lookup"><span data-stu-id="3c646-107">Try the following steps to enable/set the TLS protocol to 1.2, verify, and retry.</span></span>
 1. <span data-ttu-id="3c646-108">В командния прозорец на PowerShell (PS C: \) въведете следната команда, за да зададете TLS протокола на версия 1.2:</span><span class="sxs-lookup"><span data-stu-id="3c646-108">At the PowerShell command prompt (PS C:\) enter the following command to set the TLS protocol to version 1.2:</span></span>

    `[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12`

2. <span data-ttu-id="3c646-109">Проверете използвания(те) TLS протокол(и) със следната команда:</span><span class="sxs-lookup"><span data-stu-id="3c646-109">Verify the TLS protocol(s) in use, with the following command:</span></span>

    `[Net.ServicePointManager]::SecurityProtocol` 

3. <span data-ttu-id="3c646-110">Опитайте отново командите Получаване или Актуализиране, ако е необходимо.</span><span class="sxs-lookup"><span data-stu-id="3c646-110">Retry the Get or Update commands as needed.</span></span>

