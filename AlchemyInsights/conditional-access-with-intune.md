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
# <a name="conditional-access-with-intune"></a>Условен достъп с Intune

Използването на **условен достъп** с Intune изисква 3 стъпки:

- Създаване на **правила за съответствие** ([Андроид](https://docs.microsoft.com/intune/compliance-policy-create-android), [iOS](https://docs.microsoft.com/intune/compliance-policy-create-ios), [Windows](https://docs.microsoft.com//intune/compliance-policy-create-windows)), за да определите настройки, които трябва да бъдат изпълнени, преди устройството да се счита за съвместимо. Например, преди да се приеме, че е съвместимо, устройството трябва да има щифт с най-малко 6 цифри.
- Създаване на **правила за условен достъп,** който определя кои ресурси се защитават и какви условия трябва да бъдат изпълнени за достъп до тези ресурси.  [Например,](https://docs.microsoft.com/intune/tutorial-protect-email-on-unmanaged-devices#create-conditional-access-policies) дадено устройство трябва да е съвместимо преди да получи достъп до корпоративен имейл.
- Уверете се, че **както правилата за съответствие,** така и **правилата за условен достъп** са насочени към желаните групи потребители. Това може да изисква създаване на специфични групи от потребители в Azure Active Directory.

**Полезни връзки:**

[Преглед на съответствието на устройството](https://docs.microsoft.com/intune/device-compliance-get-started)

[Отстраняване на неизправности](https://docs.microsoft.com/intune/troubleshoot-conditional-access)

[Правила за отстраняване на неизправности](https://docs.microsoft.com/intune/troubleshoot-policies-in-microsoft-intune)

За да защитите имейл (Exchange online) от достъп с несъответстващи устройства, трябва да се следват и двата документа:

1. [Защита на достъпа до имейл от устройства, използващи EAS](https://docs.microsoft.com/intune/tutorial-protect-email-on-unmanaged-devices)
2. [Защита на имейл достъп от устройства, използващи съвременни клиенти за удостоверяване като Outlook](https://docs.microsoft.com/intune/tutorial-protect-email-on-enrolled-devices)