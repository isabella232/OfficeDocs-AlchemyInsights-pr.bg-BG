---
title: Използване на условен достъп с настройки
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
- "6700002"
- "7680"
ms.openlocfilehash: 6e86c6b4c9c6adcbeac504acd5a10f2139d04237
ms.sourcegitcommit: 6312ee31561db36104f32282d019d069ede69174
ms.translationtype: MT
ms.contentlocale: bg-BG
ms.lasthandoff: 03/11/2021
ms.locfileid: "50743352"
---
# <a name="using-conditional-access-with-intune"></a><span data-ttu-id="d9f50-102">Използване на условен достъп с настройки</span><span class="sxs-lookup"><span data-stu-id="d9f50-102">Using Conditional Access with Intune</span></span>

<span data-ttu-id="d9f50-103">Използването на условен достъп с помощта на функцията изисква три стъпки:</span><span class="sxs-lookup"><span data-stu-id="d9f50-103">Using Conditional Access with Intune requires 3 steps:</span></span>

- [<span data-ttu-id="d9f50-104">Създайте правила за съответствие, за да дефинирате настройки, които трябва да бъдат изпълнени, преди устройството да бъде счетено за съвместимо. Например устройството трябва да има ПИН код най-малко 6 цифри, преди да бъде счетен за съвместим.</span><span class="sxs-lookup"><span data-stu-id="d9f50-104">Create a Compliance Policy to define settings that must be met before the device is considered compliant. For example, a device must have a pin of at least 6 digits before it is considered compliant.</span></span>](https://docs.microsoft.com/mem/intune/protect/create-compliance-policy)
- [<span data-ttu-id="d9f50-105">Създайте правила за условен достъп, които определят какви ресурси са защитени, и какви условия трябва да бъдат изпълнени, за да получат достъп до тези ресурси. Например устройството трябва да е съвместимо, преди да осъществите достъп до корпоративна поща.</span><span class="sxs-lookup"><span data-stu-id="d9f50-105">Create a Conditional Access Policy that defines what resources are being protected, and what conditions need to be met to access those resources. For example, a device must be compliant before accessing corporate email.</span></span>](https://docs.microsoft.com/mem/intune/protect/tutorial-protect-email-on-unmanaged-devices#create-conditional-access-policies)
- [<span data-ttu-id="d9f50-106">Уверете се, че правилата за съответствие и правилата за условен достъп се насочват към желаните групи потребители. Това може да изисква създаването на определени групи от потребители в Azure Active Directory.</span><span class="sxs-lookup"><span data-stu-id="d9f50-106">Ensure both Compliance Policies and Conditional Access Policies are targeted to the desired groups of users. This may require creating specific groups of users in Azure Active Directory.</span></span>](https://docs.microsoft.com/troubleshoot/mem/intune/troubleshoot-conditional-access)

[<span data-ttu-id="d9f50-107">Прочетете повече...</span><span class="sxs-lookup"><span data-stu-id="d9f50-107">Read more...</span></span>](https://docs.microsoft.com/mem/intune/protect/device-compliance-get-started)
