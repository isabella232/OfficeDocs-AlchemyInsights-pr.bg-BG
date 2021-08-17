---
title: Прехвърляне на собствеността на Azure фактуриране
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9003560"
- "6849"
ms.openlocfilehash: 803d0105ad2bbaf2b18cea6aa556b6af5e09cb2d41812d4747aa703e6e7d7780
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: bg-BG
ms.lasthandoff: 08/05/2021
ms.locfileid: "54036085"
---
# <a name="transfer-azure-billing-ownership"></a>Прехвърляне на собствеността на Azure фактуриране

Влезте в портала на [Azure](https://portal.azure.com/) като администратор на акаунта за фактуриране с абонамента, който искате да прехвърлите. Ако не сте сигурни дали сте администратор, или ако трябва да определите кой е, вижте [Определяне на администратора на фактурирането на акаунта](https://docs.microsoft.com/azure/cost-management-billing/understand/subscription-transfer#whoisaa).

1. Търсене в _Управление на разходите + Фактуриране_.
1. Изберете **Абонаменти** от левия екран. В зависимост от достъпа може да се наложи да изберете обхват на фактуриране и след това **Абонаменти** или **Абонаменти за Azure**.
1. Изберете **Прехвърляне на собствеността за фактуриране** за абонамента, който искате да прехвърлите.
1. Въведете имейл адреса на потребител, който е администратор на фактуриране на акаунта и ще бъде новият собственик за абонамента, след което изберете **Изпращане на искане за прехвърляне**.
1. Потребителят получава имейл с инструкции как да прегледа вашето искане за прехвърляне. За да одобри искането за прехвърляне, потребителят избира връзката в имейла и следва инструкциите.

Обърнете внимание, че ако прехвърлите собствеността за фактуриране на вашия абонамент на потребителски акаунт в друг клиент на Azure AD, всички възложени задачи [за управление на достъпа, базирано на роли (RBAC)](https://docs.microsoft.com/azure/role-based-access-control/overview?WT.mc_id=Portal-Microsoft_Azure_Support) за управление на ресурси в абонамента се премахват завинаги. Само новият собственик ще има достъп за управление на ресурси в абонамента. За повече информация как да промените указателя за абонамент, вижте [Прехвърляне на абонамент за потребител в друг клиент на Azure AD](https://docs.microsoft.com/azure/active-directory/managed-identities-azure-resources/known-issues?WT.mc_id=Portal-Microsoft_Azure_Support).

_**Важно въздействие върху вашите фактури**_: Ако сте прехвърлили собствеността за фактуриране за абонамент за Azure, вашите такси ще бъдат изчислявани пропорционално. Ще можете да получите достъп до фактурите по следния начин:  

1. Изберете абонамента си от  [Страницата абонаменти за](https://portal.azure.com/#blade/Microsoft_Azure_Billing/SubscriptionsBlade) в портала на Azure като [потребител с достъп до фактурите](https://docs.microsoft.com/azure/cost-management-billing/manage/manage-billing-access?WT.mc_id=Portal-Microsoft_Azure_Support), след което изберете **Фактури**.
1. Щракнете върху **Изтегляне на фактура** , за да прегледате копие на вашата фактура в PDF формат. Ако се появи съобщение _Не е налична_, вижте [Защо не виждам фактура за последния период на фактуриране?](https://docs.microsoft.com/azure/cost-management-billing/manage/download-azure-invoice-daily-usage-date?WT.mc_id=Portal-Microsoft_Azure_Support#noinvoice).
1. Можете също да видите ежедневната си употреба като щракнете върху **Период на фактуриране**, за да получите фактурата си като PDF файл, както и копие на вашия подробен файл за ежедневното използване (.CSV). За повече информация вижте [Получаване на фактурата и данни за употребата](https://docs.microsoft.com/azure/cost-management-billing/manage/download-azure-invoice-daily-usage-date?WT.mc_id=Portal-Microsoft_Azure_Support).

**Препоръчителни документи**

- [Прехвърляне на собствеността за фактуриране на абонамент за Azure към друг акаунт](https://docs.microsoft.com/azure/cost-management-billing/manage/billing-subscription-transfer)
- [За прехвърлянето на собствеността за фактуриране на абонамент за Azure](https://docs.microsoft.com//azure/cost-management-billing/understand/subscription-transfer)
- [Прехвърляне на абонаменти устройства/тестване на Visual Studio, Мрежа от партньори на Microsoft (MPN) и предплатена услуга](https://docs.microsoft.com/azure/billing/billing-subscription-transfer?WT.mc_id=Portal-Microsoft_Azure_Support#transferring-visual-studio-microsoft-partner-network-mpn-and-pay-as-you-go-devtest-subscriptions)
- [Често задавани въпроси за прехвърлянето на собствеността](https://docs.microsoft.com/azure/billing/billing-subscription-transfer?WT.mc_id=Portal-Microsoft_Azure_Support#frequently-asked-questions-faq-for-senders)
- [Отстраняване на проблеми със прехвърлянето на собствеността](https://docs.microsoft.com/azure/billing/billing-subscription-transfer?WT.mc_id=Portal-Microsoft_Azure_Support#troubleshooting)
