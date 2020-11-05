---
title: Прехвърляне на собствеността на Azure за фактуриране
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9003560"
- "6849"
ms.openlocfilehash: e9a1e74b321e2c2dda5f7a4f69681a0acf0635d5
ms.sourcegitcommit: a5ba4dc8c349ed79147f67b62bde544281f7c106
ms.translationtype: MT
ms.contentlocale: bg-BG
ms.lasthandoff: 11/03/2020
ms.locfileid: "48922004"
---
# <a name="transfer-azure-billing-ownership"></a>Прехвърляне на собствеността на Azure за фактуриране

Влезте в портала на [Azure](https://portal.azure.com/) като администратор на акаунт за фактуриране, който има абонамента, който искате да прехвърлите. Ако не сте сигурни дали сте администратор, или ако трябва да определите кой е, вижте определяне на администратор на [фактуриране на акаунт](https://docs.microsoft.com/azure/cost-management-billing/understand/subscription-transfer#whoisaa).

- Извършете търсене по **управление на разходите + плащане**.
- Изберете " **абонаменти** " от левия екран. В зависимост от достъпа може да се наложи да изберете обхват на фактуриране **и след това абонаменти** или **Azure абонаменти**.
- Изберете " **прехвърляне на собствеността върху плащането** за абонамента, който искате да прехвърлите"
- Въведете имейл адреса на потребител, който е администратор на фактуриране на акаунта, който ще бъде новият собственик за абонамента, и след това изберете **Изпращане на искане за прехвърляне**
- Потребителят получава имейл с инструкции, за да прегледа вашата заявка за прехвърляне. За да одобри заявката за прехвърляне, потребителят избира връзката в имейла и следва инструкциите.

**Забележка** : Ако прехвърлите собствеността за плащане на абонамента си за акаунт на потребител в друг клиент на Azure ad, всички присвоени задачи за управление на [достъп (RBAC) за ролите](https://docs.microsoft.com/azure/role-based-access-control/overview?WT.mc_id=Portal-Microsoft_Azure_Support), за да управлявате ресурсите в абонамента, се премахват трайно. Само новият собственик ще има достъп до управление на ресурсите в абонамента. За повече информация вижте [прехвърляне на абонамент за потребител в друг клиент на AZURE ad](https://docs.microsoft.com/azure/active-directory/managed-identities-azure-resources/known-issues?WT.mc_id=Portal-Microsoft_Azure_Support).

**Препоръчвани документи**

- [Прехвърляне на собствеността на абонамента за Azure към друг акаунт](https://docs.microsoft.com/azure/cost-management-billing/manage/billing-subscription-transfer)
- [За прехвърляне на собствеността върху плащане за Azure абонамент](https://docs.microsoft.com//azure/cost-management-billing/understand/subscription-transfer)
- [Прехвърляне на Visual Studio, партньорска мрежа на Microsoft (MPN) и плащане като отидете на Dev/Test абонаменти](https://docs.microsoft.com/azure/billing/billing-subscription-transfer?WT.mc_id=Portal-Microsoft_Azure_Support#transferring-visual-studio-microsoft-partner-network-mpn-and-pay-as-you-go-devtest-subscriptions)
- [Често задавани въпроси за собствеността върху прехвърляне](https://docs.microsoft.com/azure/billing/billing-subscription-transfer?WT.mc_id=Portal-Microsoft_Azure_Support#frequently-asked-questions-faq-for-senders)
- [Отстраняване на проблеми с собствеността при прехвърляне](https://docs.microsoft.com/azure/billing/billing-subscription-transfer?WT.mc_id=Portal-Microsoft_Azure_Support#troubleshooting)
