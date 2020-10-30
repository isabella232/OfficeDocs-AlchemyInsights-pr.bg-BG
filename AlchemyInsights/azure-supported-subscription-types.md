---
title: Поддържани типове абонаменти
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
- "6675"
ms.openlocfilehash: 46bc60435c3f8477e9f274d90c39d0f1c6a523c6
ms.sourcegitcommit: f8b41ecda6db0b8f64fe0c51f1e8e6619f504d61
ms.translationtype: MT
ms.contentlocale: bg-BG
ms.lasthandoff: 10/28/2020
ms.locfileid: "48807248"
---
# <a name="supported-subscription-types"></a>Поддържани типове абонаменти

Моля, прегледайте поддържаните типове абонаменти, за да продължите по-нататък.

[Поддържани типове абонаменти](https://docs.microsoft.com/azure/billing/billing-subscription-transfer?WT.mc_id=Portal-Microsoft_Azure_Support#supported-subscription-types)

**Прехвърляне на собствеността върху плащане**

Портал на Azure като [администратор на акаунт](https://ms.portal.azure.com/) за акаунт за фактуриране, който има абонамента, който искате да прехвърлите

- Извършете търсене по **управление на разходите + плащане** . Изберете " **абонаменти** " от левия екран. В зависимост от достъпа може да се наложи да изберете обхват на фактуриране **и след това абонаменти** или **Azure абонаменти** .
- Изберете "прехвърляне на собствеността върху плащането за абонамента, който искате да прехвърлите"
- Въведете имейл адреса на потребител, който е администратор на фактуриране на акаунта, който ще бъде новият собственик за абонамента, и след това изберете **Изпращане на искане за прехвърляне**
- Потребителят получава имейл с инструкции, за да прегледа вашата заявка за прехвърляне. За да одобри заявката за прехвърляне, потребителят избира връзката в имейла и следва инструкциите.

Забележка: Ако прехвърлите собствеността за плащане на абонамента си за акаунт на потребител в друг клиент на Azure AD, всички присвоени задачи за управление на [достъп (RBAC) за ролите](https://docs.microsoft.com/azure/role-based-access-control/overview?WT.mc_id=Portal-Microsoft_Azure_Support) , за да управлявате ресурсите в абонамента, се премахват трайно. Само новият собственик ще има достъп до управление на ресурсите в абонамента. За повече информация вижте [прехвърляне на абонамент за потребител в друг клиент на AZURE ad](https://docs.microsoft.com/azure/active-directory/managed-identities-azure-resources/known-issues?WT.mc_id=Portal-Microsoft_Azure_Support).

**Прехвърляне на собствеността върху абонамент**

Функция за прехвърляне на собствеността върху абонамент, базирано на роли (RBAC) за управление на ресурси в абонамента, загубват достъпа си. За повече информация относно добавянето на съществуващ абонамент към клиент вижте [свързване или добавяне на абонамент за Azure към Azure Active Directory](https://docs.microsoft.com/azure/active-directory/fundamentals/active-directory-how-subscriptions-associated-directory?WT.mc_id=Portal-Microsoft_Azure_Support).

- Прехвърлянето на абонамент със съществуваща недължима сума от текущия цикъл на фактуриране няма да бъде прехвърлено към новия инструмент за плащане в новия акаунт. Единствената налична информация за потребителите в новия акаунт е разходите за последния месец за абонамента ви. Останалата част от хронологията на използването и фактурирането не се прехвърля с абонамента.
- Прехвърляне на собствеността върху абонамент за корпоративно споразумение (EA) в момента се поддържа само в портала за корпоративно споразумение
- Прехвърлянето на абонамент за кредит, като например Visual Studio, BizSpark, партньорската мрежа на Microsoft към нов потребител изисква да има лиценз за партньор на Visual Studio/Microsoft, за да приеме искането за прехвърляне
- Всички ресурси, като например виртуални машини, дискове и прехвърляне на уеб сайтове, ще бъдат прехвърлени успешно към новия акаунт. Следните ресурси могат да бъдат засегнати при прехвърляне на абонамент за кръстосани наематели:

**Услуги за домейни на Azure AD**

Трезори за ключове на Azure

- Възможно е [свързаните с SQL потребители и бази данни](https://docs.microsoft.com/azure/sql-database/sql-database-aad-authentication-configure?WT.mc_id=Portal-Microsoft_Azure_Support) да бъдат засегнати, особено ако клиентът използва удостоверяване, свързано с Azure Active Directory
- **Услугите за приложения** , конфигурирани с удостоверяване на Azure Active Directory, могат да бъдат повлияни
- **Екип на Visual Studio** Акаунтите за услуги, свързани с абонаменти за Azure, може временно да загубят достъп, когато се анулира свързаният в момента договор за Azure

**Препоръчвани документи**

Стъпки след приемането на собствеността за фактуриране:

- За да запазите собствеността за фактуриране, но да промените типа на вашия абонамент, вижте препращане на [вашия абонамент за Azure към друго предложение](https://docs.microsoft.com/azure/billing/billing-how-to-switch-azure-offer?WT.mc_id=Portal-Microsoft_Azure_Support) .
- [Прехвърляне на Visual Studio, партньорска мрежа на Microsoft (MPN) и плащане като отидете на Dev/Test абонаменти](https://docs.microsoft.com/azure/billing/billing-subscription-transfer?WT.mc_id=Portal-Microsoft_Azure_Support#transferring-visual-studio-microsoft-partner-network-mpn-and-pay-as-you-go-devtest-subscriptions)
- [Прехвърляне на собствеността върху плащане на абонаменти за корпоративно споразумение (EA)](https://docs.microsoft.com/azure/billing/billing-subscription-transfer?WT.mc_id=Portal-Microsoft_Azure_Support#transfer-billing-ownership-of-enterprise-agreement-ea-subscriptions)
- [Често задавани въпроси за собствеността върху прехвърляне](https://docs.microsoft.com/azure/billing/billing-subscription-transfer?WT.mc_id=Portal-Microsoft_Azure_Support#frequently-asked-questions-faq-for-senders)
- [Отстраняване на проблеми с собствеността при прехвърляне](https://docs.microsoft.com/azure/billing/billing-subscription-transfer?WT.mc_id=Portal-Microsoft_Azure_Support#troubleshooting)