---
title: Правила за пароли
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 03/11/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004595"
- "9277"
ms.openlocfilehash: 826e266d08aa68c0d4213d8058a0244f404fe965
ms.sourcegitcommit: 186281d0b87d67f041c127d4334faa937da9a48a
ms.translationtype: MT
ms.contentlocale: bg-BG
ms.lasthandoff: 03/11/2021
ms.locfileid: "50743182"
---
# <a name="password-policies"></a>Правила за пароли

**Имам проблеми с правилата за парола за потребител**

- Правилата за пароли за един потребител зависят от това дали потребителят е само в облака, или локален.
- Само в облака потребителите трябва да изберат парола, която отговаря на изискванията в тази статия: [правила за пароли, приложими само за потребителските акаунти в облака](https://docs.microsoft.com/azure/active-directory/authentication/concept-sspr-policy?WT.mc_id=Portal-Microsoft_Azure_Support#password-policies-that-only-apply-to-cloud-user-accounts)
- Локалните потребители трябва да изберат парола, която отговаря на локалните изисквания. Ако локален потребител не е в състояние да зададе паролата си, проверете локалните изисквания.

**Не знам как да задам или да проверя правилата за изтичане на парола**

- Можете да зададете и да проверите правилата за изтичане на срока за потребители в облака в своя клиент с помощта на PowerShell. Следвайте инструкциите в тази статия: [Задаване или проверка на правилата за пароли с помощта на PowerShell](https://docs.microsoft.com/azure/active-directory/authentication/concept-sspr-policy?WT.mc_id=Portal-Microsoft_Azure_Support#set-or-check-the-password-policies-by-using-powershell)
- Правилата за изтичане на парола за локални потребители се задават във вашата локална реклама.

**Други полезни връзки:**
- [Първи стъпки в нулирането на паролата](https://docs.microsoft.com/azure/active-directory/authentication/concept-sspr-policy?WT.mc_id=Portal-Microsoft_Azure_Support#set-or-check-the-password-policies-by-using-powershell)
- [Отстраняване на неизправности при нулиране на паролата на администратор](https://docs.microsoft.com/azure/active-directory/active-directory-passwords-troubleshoot?WT.mc_id=Portal-Microsoft_Azure_Support#troubleshoot-the-password-reset-portal)
