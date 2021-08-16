---
title: Условен достъп с Intune
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: aecba7c5-e86d-4ec8-9d44-679f5a3d659d
ms.openlocfilehash: c24451fba8b8ab8fe7a1778bb292dec6678e1ef487076d27458c9aeb4963c683
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: bg-BG
ms.lasthandoff: 08/05/2021
ms.locfileid: "54069701"
---
# <a name="conditional-access-with-intune"></a>Условен достъп с Intune

Използването  **на условен**  достъп с Intune изисква 3 стъпки:

- Създайте **правила за съответствие** ([Android](https://docs.microsoft.com/intune/compliance-policy-create-android), [iOS](https://docs.microsoft.com/intune/compliance-policy-create-ios), [Windows](https://docs.microsoft.com//intune/compliance-policy-create-windows)), за да дефинирате настройките, които трябва да бъдат изпълнени, преди устройството да се счита за съвместимо. Например устройството трябва да има пин с най-малко 6 цифри, преди да се счита за съвместимо.
- Създайте **правила за условен**  достъп, които определят какви ресурси са защитени, и какви условия трябва да бъдат изпълнени, за да получите достъп до тези ресурси.  [Например устройството трябва](https://docs.microsoft.com/intune/tutorial-protect-email-on-unmanaged-devices#create-conditional-access-policies)  да отговаря на изискванията, преди да получите достъп до корпоративния имейл.
- Уверете се, **че правилата за**  съответствие и правилата  **за**  условен достъп са насочени към желаните групи потребители. Това може да изисква създаването на определени групи потребители в Azure Active Directory.

**Полезни връзки:**

[Общ преглед на съответствието на устройствата](https://docs.microsoft.com/intune/device-compliance-get-started)

[Отстраняване на неизправности в CA](https://docs.microsoft.com/intune/troubleshoot-conditional-access)

[Правила за отстраняване на неизправности](https://docs.microsoft.com/troubleshoot/mem/intune/troubleshoot-policies-in-microsoft-intune)

За да защитите имейла (Exchange онлайн) от достъп от несложени устройства, трябва да се следват и двата документа:

1. [Защита на достъпа до имейл от устройства с помощта на EAS](https://docs.microsoft.com/intune/tutorial-protect-email-on-unmanaged-devices)
2. [Защита на имейл достъпа от устройства с помощта на съвременни клиенти за удостоверяване, Outlook](https://docs.microsoft.com/intune/tutorial-protect-email-on-enrolled-devices)