---
title: Условен достъп с Intune
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: aecba7c5-e86d-4ec8-9d44-679f5a3d659d
ms.openlocfilehash: f852d3646b8e5b2c0fce15055daf59c801fb8240
ms.sourcegitcommit: 7a1ff0314df06e386f32a2439fe060baa480e8f8
ms.translationtype: MT
ms.contentlocale: bg-BG
ms.lasthandoff: 06/30/2020
ms.locfileid: "44931419"
---
# <a name="conditional-access-with-intune"></a><span data-ttu-id="36bc7-102">Условен достъп с Intune</span><span class="sxs-lookup"><span data-stu-id="36bc7-102">Conditional Access with Intune</span></span>

<span data-ttu-id="36bc7-103">Използването на **условен достъп** с Intune изисква 3 стъпки:</span><span class="sxs-lookup"><span data-stu-id="36bc7-103">Using  **Conditional Access**  with Intune requires 3 steps:</span></span>

- <span data-ttu-id="36bc7-104">Създаване на **правила за съответствие** ([Андроид](https://docs.microsoft.com/intune/compliance-policy-create-android), [iOS](https://docs.microsoft.com/intune/compliance-policy-create-ios), [Windows](https://docs.microsoft.com//intune/compliance-policy-create-windows)), за да определите настройки, които трябва да бъдат изпълнени, преди устройството да се счита за съвместимо.</span><span class="sxs-lookup"><span data-stu-id="36bc7-104">Create a  **Compliance Policy**  ([Android](https://docs.microsoft.com/intune/compliance-policy-create-android),  [iOS](https://docs.microsoft.com/intune/compliance-policy-create-ios),  [Windows](https://docs.microsoft.com//intune/compliance-policy-create-windows)) to define settings that must be met before the device is considered compliant.</span></span> <span data-ttu-id="36bc7-105">Например, преди да се приеме, че е съвместимо, устройството трябва да има щифт с най-малко 6 цифри.</span><span class="sxs-lookup"><span data-stu-id="36bc7-105">For example, a device must have a pin of at least 6 digits before it is considered compliant.</span></span>
- <span data-ttu-id="36bc7-106">Създаване на **правила за условен достъп,** който определя кои ресурси се защитават и какви условия трябва да бъдат изпълнени за достъп до тези ресурси.</span><span class="sxs-lookup"><span data-stu-id="36bc7-106">Create a **Conditional Access Policy**  that defines what resources are being protected, and what conditions need to be met to access those resources.</span></span>  <span data-ttu-id="36bc7-107">[Например,](https://docs.microsoft.com/intune/tutorial-protect-email-on-unmanaged-devices#create-conditional-access-policies) дадено устройство трябва да е съвместимо преди да получи достъп до корпоративен имейл.</span><span class="sxs-lookup"><span data-stu-id="36bc7-107">[For example,](https://docs.microsoft.com/intune/tutorial-protect-email-on-unmanaged-devices#create-conditional-access-policies)  a device must be compliant before accessing corporate email.</span></span>
- <span data-ttu-id="36bc7-108">Уверете се, че **както правилата за съответствие,** така и **правилата за условен достъп** са насочени към желаните групи потребители.</span><span class="sxs-lookup"><span data-stu-id="36bc7-108">Ensure both **Compliance Policies**  and  **Conditional Access Policies**  are targeted to the desired groups of users.</span></span> <span data-ttu-id="36bc7-109">Това може да изисква създаване на специфични групи от потребители в Azure Active Directory.</span><span class="sxs-lookup"><span data-stu-id="36bc7-109">This may require creating specific groups of users in Azure Active Directory.</span></span>

<span data-ttu-id="36bc7-110">**Полезни връзки:**</span><span class="sxs-lookup"><span data-stu-id="36bc7-110">**Helpful links:**</span></span>

[<span data-ttu-id="36bc7-111">Преглед на съответствието на устройството</span><span class="sxs-lookup"><span data-stu-id="36bc7-111">Device compliance overview</span></span>](https://docs.microsoft.com/intune/device-compliance-get-started)

[<span data-ttu-id="36bc7-112">Отстраняване на неизправности</span><span class="sxs-lookup"><span data-stu-id="36bc7-112">Troubleshooting CA</span></span>](https://docs.microsoft.com/intune/troubleshoot-conditional-access)

[<span data-ttu-id="36bc7-113">Правила за отстраняване на неизправности</span><span class="sxs-lookup"><span data-stu-id="36bc7-113">Troubleshooting policy</span></span>](https://docs.microsoft.com/intune/troubleshoot-policies-in-microsoft-intune)

<span data-ttu-id="36bc7-114">За да защитите имейл (Exchange online) от достъп с несъответстващи устройства, трябва да се следват и двата документа:</span><span class="sxs-lookup"><span data-stu-id="36bc7-114">To protect Email (Exchange online) from access by noncompliant devices, both documents must be followed:</span></span>

1. [<span data-ttu-id="36bc7-115">Защита на достъпа до имейл от устройства, използващи EAS</span><span class="sxs-lookup"><span data-stu-id="36bc7-115">Protect email access from devices using EAS</span></span>](https://docs.microsoft.com/intune/tutorial-protect-email-on-unmanaged-devices)
2. [<span data-ttu-id="36bc7-116">Защита на имейл достъп от устройства, използващи съвременни клиенти за удостоверяване като Outlook</span><span class="sxs-lookup"><span data-stu-id="36bc7-116">Protect email access from devices using modern authentication clients like Outlook</span></span>](https://docs.microsoft.com/intune/tutorial-protect-email-on-enrolled-devices)