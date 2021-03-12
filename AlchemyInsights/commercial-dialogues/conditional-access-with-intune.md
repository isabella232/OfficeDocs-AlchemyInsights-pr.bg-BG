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
# <a name="using-conditional-access-with-intune"></a>Използване на условен достъп с настройки

Използването на условен достъп с помощта на функцията изисква три стъпки:

- [Създайте правила за съответствие, за да дефинирате настройки, които трябва да бъдат изпълнени, преди устройството да бъде счетено за съвместимо. Например устройството трябва да има ПИН код най-малко 6 цифри, преди да бъде счетен за съвместим.](https://docs.microsoft.com/mem/intune/protect/create-compliance-policy)
- [Създайте правила за условен достъп, които определят какви ресурси са защитени, и какви условия трябва да бъдат изпълнени, за да получат достъп до тези ресурси. Например устройството трябва да е съвместимо, преди да осъществите достъп до корпоративна поща.](https://docs.microsoft.com/mem/intune/protect/tutorial-protect-email-on-unmanaged-devices#create-conditional-access-policies)
- [Уверете се, че правилата за съответствие и правилата за условен достъп се насочват към желаните групи потребители. Това може да изисква създаването на определени групи от потребители в Azure Active Directory.](https://docs.microsoft.com/troubleshoot/mem/intune/troubleshoot-conditional-access)

[Прочетете повече...](https://docs.microsoft.com/mem/intune/protect/device-compliance-get-started)
