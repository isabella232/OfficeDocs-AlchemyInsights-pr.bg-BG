---
title: Поддържани типове абонаменти
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
- "6675"
ms.openlocfilehash: f11eabdc18f708e34a6a10c67bc3e7416330cbf34aec20209b42252ffa0ab018
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: bg-BG
ms.lasthandoff: 08/05/2021
ms.locfileid: "54072149"
---
# <a name="supported-subscription-types"></a>Поддържани типове абонаменти

Прегледайте поддържаните типове абонаменти, за да продължите по-нататък.

[Поддържани типове абонаменти](https://docs.microsoft.com/azure/billing/billing-subscription-transfer?WT.mc_id=Portal-Microsoft_Azure_Support#supported-subscription-types)

**Прехвърляне на собствеността на фактуриране**

Влезте в портала на [Azure](https://ms.portal.azure.com/) като администратор на акаунта за фактуриране, в който е абонаментът, който искате да прехвърлите.

- Потърсете **Управление на разходите + Фактуриране**. Изберете **Абонаменти** от левия екран. В зависимост от достъпа, може да се наложи да изберете обхват на фактуриране и след това **Абонаменти** или **Абонаменти за Azure**.
- Изберете "Прехвърляне на собствеността на фактуриране" за абонамента, който искате да прехвърлите.
- Въведете имейл адреса на потребител, който е администратор на фактуриране на акаунта и ще бъде новият собственик за абонамента, след което изберете **Изпращане на искане за прехвърляне**.
- Потребителят получава имейл с инструкции как да прегледа вашето искане за прехвърляне. За да одобри искането за прехвърляне, потребителят избира връзката в имейла и следва инструкциите.

Забележка: Обърнете внимание, че ако прехвърлите собствеността за фактуриране на вашия абонамент на потребителски акаунт в друг клиент на Azure AD, всички възложени задачи [за управление на достъпа, базирано на роли (RBAC)](https://docs.microsoft.com/azure/role-based-access-control/overview?WT.mc_id=Portal-Microsoft_Azure_Support) за управление на ресурси в абонамента се премахват завинаги. Само новият собственик ще има достъп за управление на ресурси в абонамента. За повече информация вижте [Прехвърляне на абонамент към потребител в друг клиент на Azure AD](https://docs.microsoft.com/azure/active-directory/managed-identities-azure-resources/known-issues?WT.mc_id=Portal-Microsoft_Azure_Support).

**Прехвърляне на собствеността върху абонамента**

"Прехвърляне на собствеността на абонамента" изисква достъп, базиран на роли (RBAC), за да управлявате ресурсите, ако абонаментът загуби достъпа до тях. За повече информация за добавянето на съществуващ абонамент към клиент вижте [Свързване или добавяне на абонамент за Azure към Azure Active Directory](https://docs.microsoft.com/azure/active-directory/fundamentals/active-directory-how-subscriptions-associated-directory?WT.mc_id=Portal-Microsoft_Azure_Support).

- Прехвърлянето на абонамент със съществуваща дължима сума от текущия цикъл на фактуриране няма да премине към новия инструмент за плащане в новия акаунт. Единствената информация, налична за потребителите в новия акаунт, е цената за последния месец за вашия абонамент. Останалата част от използването и хронологията на фактуриране не се прехвърля с абонамента.
- Прехвърлянето на собствеността върху фактурирането на абонаменти за корпоративно споразумение (EA) в момента се поддържа само в портала за корпоративни споразумения
- Прехвърлянето на абонамент, ориентиран към кредит, като Visual Studio, BizSpark, мрежата от партньори на Microsoft към нов потребител изисква да имате мрежов лиценз на партньор на Visual Studio/Microsoft, за да приемете искането за прехвърляне
- Всички ресурси, като виртуални машини, дискове и уеб сайтове, се прехвърлят успешно към новия акаунт. Следните ресурси могат да бъдат засегнати при прехвърляне на абонамент между различни клиенти:

**Домейнови услуги на Azure AD**

Хранилища за ключове на Azure

- Възможно е да бъдат засегнати [свързани с SQL потребители и бази данни](https://docs.microsoft.com/azure/sql-database/sql-database-aad-authentication-configure?WT.mc_id=Portal-Microsoft_Azure_Support), особено ако клиентът използва удостоверяване, свързано с Azure Active Directory
- Възможно е да бъдат засегнати **услугите за приложения**, конфигурирани с удостоверяване на Azure Active Directory
- Акаунтите за услуги на **екип на Visual Studio**, свързани с абонаменти за Azure, може временно да загубят достъп, когато свързаният абонамент за Azure бъде отменен

**Препоръчителни документи**

Стъпки след приемане на собствеността върху фактурирането:

- За да запазите собствеността върху фактурирането, но да промените типа на абонамента си, вижте: [Превключване на абонамента ви за Azure към друго предложение](https://docs.microsoft.com/azure/billing/billing-how-to-switch-azure-offer?WT.mc_id=Portal-Microsoft_Azure_Support)
- [Прехвърляне на абонаменти устройства/тестване на Visual Studio, мрежа от партньори на Microsoft (MPN) и предплатена услуга](https://docs.microsoft.com/azure/billing/billing-subscription-transfer?WT.mc_id=Portal-Microsoft_Azure_Support#transferring-visual-studio-microsoft-partner-network-mpn-and-pay-as-you-go-devtest-subscriptions)
- [Прехвърляне на собствеността върху фактурирането на абонаменти за корпоративно споразумение (EA)](https://docs.microsoft.com/azure/billing/billing-subscription-transfer?WT.mc_id=Portal-Microsoft_Azure_Support#transfer-billing-ownership-of-enterprise-agreement-ea-subscriptions)
- [Често задавани въпроси за прехвърлянето на собствеността](https://docs.microsoft.com/azure/billing/billing-subscription-transfer?WT.mc_id=Portal-Microsoft_Azure_Support#frequently-asked-questions-faq-for-senders)
- [Отстраняване на проблеми със прехвърлянето на собствеността](https://docs.microsoft.com/azure/billing/billing-subscription-transfer?WT.mc_id=Portal-Microsoft_Azure_Support#troubleshooting)