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
ms.openlocfilehash: 5eec5982118b4f0246afadf2af219b2d5f32f95c
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: bg-BG
ms.lasthandoff: 09/15/2020
ms.locfileid: "47807648"
---
# <a name="conditional-access-with-intune"></a>Условен достъп с настройки

Използването на  **условен достъп**  с помощта на функцията изисква три стъпки:

- Създайте  **правила за съответствие**  ([Android](https://docs.microsoft.com/intune/compliance-policy-create-android),  [IOS](https://docs.microsoft.com/intune/compliance-policy-create-ios),  [Windows](https://docs.microsoft.com//intune/compliance-policy-create-windows)), за да дефинирате настройки, които трябва да бъдат изпълнени, преди устройството да бъде счетено за съвместимо. Например устройството трябва да има ПИН код най-малко 6 цифри, преди да бъде счетен за съвместим.
- Създайте **правила за условен достъп**  , които определят какви ресурси са защитени, и какви условия трябва да бъдат изпълнени, за да получат достъп до тези ресурси.  [Например](https://docs.microsoft.com/intune/tutorial-protect-email-on-unmanaged-devices#create-conditional-access-policies)  устройството трябва да е съвместимо, преди да осъществите достъп до корпоративна поща.
- Уверете се, че **правилата за съответствие**  и  **правилата за условен достъп**  се насочват към желаните групи потребители. Това може да изисква създаването на определени групи от потребители в Azure Active Directory.

**Полезни връзки:**

[Общ преглед на съответствието на устройството](https://docs.microsoft.com/intune/device-compliance-get-started)

[Отстраняване на неизправности при CA](https://docs.microsoft.com/intune/troubleshoot-conditional-access)

[Правила за отстраняване на неизправности](https://docs.microsoft.com/intune/troubleshoot-policies-in-microsoft-intune)

За да защитите имейла (Exchange Online) от Access от несъвместими устройства, трябва да бъдат следвани и двата документа:

1. [Защита на имейл достъпа от устройства, използващи EAS](https://docs.microsoft.com/intune/tutorial-protect-email-on-unmanaged-devices)
2. [Защита на имейл достъпа от устройства, използващи модерни клиенти за удостоверяване като Outlook](https://docs.microsoft.com/intune/tutorial-protect-email-on-enrolled-devices)