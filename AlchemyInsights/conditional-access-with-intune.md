---
title: Условен достъп с настройки
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: aecba7c5-e86d-4ec8-9d44-679f5a3d659d
ms.openlocfilehash: 20ef8205431aad821419f2559be3402c8228d838
ms.sourcegitcommit: 0eb4f9bde53395b5fd4b5cd4ffc56ca96db91298
ms.translationtype: MT
ms.contentlocale: bg-BG
ms.lasthandoff: 03/10/2021
ms.locfileid: "50704775"
---
# <a name="conditional-access-with-intune"></a><span data-ttu-id="12d72-102">Условен достъп с настройки</span><span class="sxs-lookup"><span data-stu-id="12d72-102">Conditional Access with Intune</span></span>

<span data-ttu-id="12d72-103">Използването на  **условен достъп**  с помощта на функцията изисква три стъпки:</span><span class="sxs-lookup"><span data-stu-id="12d72-103">Using  **Conditional Access**  with Intune requires 3 steps:</span></span>

- <span data-ttu-id="12d72-104">Създайте  **правила за съответствие**  ([Android](https://docs.microsoft.com/intune/compliance-policy-create-android),  [IOS](https://docs.microsoft.com/intune/compliance-policy-create-ios),  [Windows](https://docs.microsoft.com//intune/compliance-policy-create-windows)), за да дефинирате настройки, които трябва да бъдат изпълнени, преди устройството да бъде счетено за съвместимо.</span><span class="sxs-lookup"><span data-stu-id="12d72-104">Create a  **Compliance Policy**  ([Android](https://docs.microsoft.com/intune/compliance-policy-create-android),  [iOS](https://docs.microsoft.com/intune/compliance-policy-create-ios),  [Windows](https://docs.microsoft.com//intune/compliance-policy-create-windows)) to define settings that must be met before the device is considered compliant.</span></span> <span data-ttu-id="12d72-105">Например устройството трябва да има ПИН код най-малко 6 цифри, преди да бъде счетен за съвместим.</span><span class="sxs-lookup"><span data-stu-id="12d72-105">For example, a device must have a pin of at least 6 digits before it is considered compliant.</span></span>
- <span data-ttu-id="12d72-106">Създайте **правила за условен достъп**  , които определят какви ресурси са защитени, и какви условия трябва да бъдат изпълнени, за да получат достъп до тези ресурси.</span><span class="sxs-lookup"><span data-stu-id="12d72-106">Create a **Conditional Access Policy**  that defines what resources are being protected, and what conditions need to be met to access those resources.</span></span>  <span data-ttu-id="12d72-107">[Например](https://docs.microsoft.com/intune/tutorial-protect-email-on-unmanaged-devices#create-conditional-access-policies)  устройството трябва да е съвместимо, преди да осъществите достъп до корпоративна поща.</span><span class="sxs-lookup"><span data-stu-id="12d72-107">[For example,](https://docs.microsoft.com/intune/tutorial-protect-email-on-unmanaged-devices#create-conditional-access-policies)  a device must be compliant before accessing corporate email.</span></span>
- <span data-ttu-id="12d72-108">Уверете се, че **правилата за съответствие**  и  **правилата за условен достъп**  се насочват към желаните групи потребители.</span><span class="sxs-lookup"><span data-stu-id="12d72-108">Ensure both **Compliance Policies**  and  **Conditional Access Policies**  are targeted to the desired groups of users.</span></span> <span data-ttu-id="12d72-109">Това може да изисква създаването на определени групи от потребители в Azure Active Directory.</span><span class="sxs-lookup"><span data-stu-id="12d72-109">This may require creating specific groups of users in Azure Active Directory.</span></span>

<span data-ttu-id="12d72-110">**Полезни връзки:**</span><span class="sxs-lookup"><span data-stu-id="12d72-110">**Helpful links:**</span></span>

[<span data-ttu-id="12d72-111">Общ преглед на съответствието на устройството</span><span class="sxs-lookup"><span data-stu-id="12d72-111">Device compliance overview</span></span>](https://docs.microsoft.com/intune/device-compliance-get-started)

[<span data-ttu-id="12d72-112">Отстраняване на неизправности при CA</span><span class="sxs-lookup"><span data-stu-id="12d72-112">Troubleshooting CA</span></span>](https://docs.microsoft.com/intune/troubleshoot-conditional-access)

[<span data-ttu-id="12d72-113">Правила за отстраняване на неизправности</span><span class="sxs-lookup"><span data-stu-id="12d72-113">Troubleshooting policy</span></span>](https://docs.microsoft.com/troubleshoot/mem/intune/troubleshoot-policies-in-microsoft-intune)

<span data-ttu-id="12d72-114">За да защитите имейла (Exchange Online) от Access от несъвместими устройства, трябва да бъдат следвани и двата документа:</span><span class="sxs-lookup"><span data-stu-id="12d72-114">To protect Email (Exchange online) from access by noncompliant devices, both documents must be followed:</span></span>

1. [<span data-ttu-id="12d72-115">Защита на имейл достъпа от устройства, използващи EAS</span><span class="sxs-lookup"><span data-stu-id="12d72-115">Protect email access from devices using EAS</span></span>](https://docs.microsoft.com/intune/tutorial-protect-email-on-unmanaged-devices)
2. [<span data-ttu-id="12d72-116">Защита на имейл достъпа от устройства, използващи модерни клиенти за удостоверяване като Outlook</span><span class="sxs-lookup"><span data-stu-id="12d72-116">Protect email access from devices using modern authentication clients like Outlook</span></span>](https://docs.microsoft.com/intune/tutorial-protect-email-on-enrolled-devices)