---
title: Използване на условен достъп с Intune
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
ms.openlocfilehash: 23afea21668191093d612d68ca6e9ab2a844f4a14977631d33f4fd956fc3c4e7
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: bg-BG
ms.lasthandoff: 08/05/2021
ms.locfileid: "54005763"
---
# <a name="using-conditional-access-with-intune"></a>Използване на условен достъп с Intune

Използването на условен достъп с Intune изисква 3 стъпки:

- [Създайте правила за съответствие, за да дефинирате настройки, които трябва да бъдат изпълнени, преди устройството да се счита за съвместимо. Например устройството трябва да има пин с най-малко 6 цифри, преди да се счита за съвместимо.](https://docs.microsoft.com/mem/intune/protect/create-compliance-policy)
- [Създайте правила за условен достъп, които определят какви ресурси са защитени, и какви условия трябва да бъдат изпълнени, за да получите достъп до тези ресурси. Например устройството трябва да отговаря на изискванията, преди да получите достъп до корпоративния имейл.](https://docs.microsoft.com/mem/intune/protect/tutorial-protect-email-on-unmanaged-devices#create-conditional-access-policies)
- [Уверете се, че правилата за съответствие и правилата за условен достъп са насочени към желаните групи потребители. Това може да изисква създаването на определени групи потребители в Azure Active Directory.](https://docs.microsoft.com/troubleshoot/mem/intune/troubleshoot-conditional-access)

[Прочетете повече...](https://docs.microsoft.com/mem/intune/protect/device-compliance-get-started)
